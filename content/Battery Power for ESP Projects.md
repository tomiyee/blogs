---
draft: true
tags:
  - tutorial
---

Not all ESP Projects need to be battery powered. 

Sometimes it is nice to have it not be tethered to the wall. 

This post is a guide to how to power an ESP project using batteries and which batteries to choose.
## How to Battery-Power an ESP Project
- The power source should be approximately 3.3v
- The project needs to be fairly light on power draw. This means no motors which introduce large loads.
- Take the battery's positive terminal and send that to the VIN pin of the ESP
- Take the battery's negative terminal and send that to the GND pin of the ESP. 
- You should now see that the LED of the ESP Development Board turns on. Success.
## Choosing the Power Source
- Now that we know how to use a voltage source to power the ESP development board, let's explore options for the voltage source and their trade-offs.
### Option 1 - Two AA Batteries
- AA Batteries are each 1.5v
- Two of them in series will create a 3.0v Battery.
- This is enough to power very light ESP Projects.
**Positives**
- Simplicity. Easy to replace the batteries.
- Casings are very cheap
**Weaknesses**
- Not conveniently rechargeable. 
- No built in power buttons or switches. You need to do this yourself
- Requires designing the device to be taken apart to allow replacing the batteries by the end user. This can add some complexity but tutorials exist

We can almost get around the weakness of not rechargable by using rechargable AA batteries. 
### Option 2 - 18650 Batteries and Battery Shield
- A single 18650 Battery 
- Battery shield can regulate the output voltage. 

**Positives**
- Battery Shield allows charging the battery while using it
- Because it's rechargable, the end user does not need to remove or replace AA batteries
**Weaknesses**
- Very bulky
- Potentially explosive?
### Option 3 - LiPO Batteries and TP4056 (Double check component)

**Strengths**
- Simultaneous charge and Discharge
- Much more compact form factor. 
**Weaknesses**
- Requires soldering to another component like the TP4056 for it to be rechargable..
- I still can't get it to work. 

## Conclusion

If you are making a prototype, two AA batteries in series should be sufficient. 

If you are handing off the product to someone and size is an important factor, the LiPO batteries are good. 

If the bulk does not matter, 18650 batteries and the battery shields come with a lot of convenient functionality out of the box. 