---
draft: true
tags:
  - note
---
An important concept in software engineering is the difference between hard links and symbolic links (or soft links or symlinks).

A lot of the information here came from [this blog post](https://linuxgazette.net/105/pitcher.html) from the Linux Gazette.

Before we can understand how hard links and symlinks work, it's important to understand how operating systems represent files under the hood. With that understanding we'll learn what a hard link is. Then, we'll compare that to a symlink.
# File Systems
---
I'll be focusing on file systems from two major classes of operating systems, Unix-like systems and Windows.
## Unix File Systems

To begin with, we'll talk about Unix-like operating systems, which includes both Linux and MacOS. Each OS name their file system differently (ext4 in Linux and HFS+ or APFS for MacOS). However, they all operate on the same basic principles.

Unix-like operating systems represent files as a directed-graph of inodes (short for "index nodes").

The actual data of a file is stored as an array somewhere in memory. 

An inode simply has an inode number and a pointer to where the file data begins. 

## Windows File Systems

The name of the file system used in Windows is New Technology File System (NTFS).

# Hard Links
- Links to something
- Data it links to must be in the same file system.

# Soft Links
- Simply a path to another file
- Can be outside of the file system
# Bonus: Windows' Shortcut File
- Neither a soft link or hard link
- Stores metadata



