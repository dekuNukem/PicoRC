# PicoPSU Adaptor for Macintosh SE & SE/30

[Purchase Link](https://www.tindie.com/products/29184/) | [Official Discord](https://discord.gg/HAuuh3pAmB) | [Table of Contents](#table-of-contents)

----

This adaptor lets you use **Pico ATX PSU** in Macintosh SE and SE/30.

![Alt text](photos/macse/three.jpeg)

It replaces the original bulky and unreliable PSU, and uses very common 12V power brick instead.

![Alt text](photos/macse/title.jpeg)

## Highlights

* **Non-destructive** and reversible

* **PC fan header** for more cooling

* Universal voltage with fused rails

* Low cost, efficient and reliable.

## Get One / Other Stuff

[Click me to get one!](https://www.tindie.com/products/29184/)

Also available for Mac 128K / Plus, Apple II, and more! [Check out the main page](./README.md) for details.

For more general-purpose diagnostics and retrofitting, check out the [full-fat ATX4VC](https://github.com/dekuNukem/ATX4VC)!

## Table of Contents

- [Getting a Pico PSU](#getting-a-pico-psu)

- [Kit Assembly](#kit-assembly)

- [Pre-flight Checks](#pre-flight-checks)

- [Installation](#installation)

- [Questions or Comments?](#questions-or-comments)

## Getting a Pico PSU

PicoPSU are tiny ATX power supplies for small PCs, but are perfect for retro computers as well.

![Alt text](photos/mac_plus/pico.jpg)

* [Official website](https://www.mini-box.com/DC-DC) and [distributors](https://www.mini-box.com/site/resellers.html). Even the cheapest 80W one should be plenty.

* Avoid generic clones. They over-rate and are of low quality.

* A power brick with **12V DC** and **center positive** 5.5x2.5mm barrel jack is needed.

* They are very popular and you might already have one. Make sure it has enough wattage.

Remember that this solution is **only as good as your PicoPSU and 12V Brick**, so don't skimp on them!

## Kit Assembly

**DON'T START YET!!!** Keep reading :)

Observe the parts:

![Alt text](photos/macse/parts1.png)

### Soldering Notes

Nothing too tricky in this kit, all basic through-hole stuff.

If this is your first time, a few tips:

* Make sure your soldering iron has **proper temperature control**. Try your local makerspace or university lab.

* Use **leaded solder** and plenty of flux, temperature around 320C / 600F.

* [This video](https://www.youtube.com/watch?v=AqvHogekDI4) covers the basics pretty well.

* Start from shortest to tallest. Solder **a single pin** first, and make sure the part is straight.

### Assembly

Solder the main PCB **as shown**, follow the notes and reference photos.

The **black 5x2 power connector** is installed on the **bottom side**, make sure the **notch faces the edge**!

![Alt text](photos/macse/notch.png)

Everything else is on top side:

![Alt text](photos/macse/note.png)

* Double check capacitor polarity!

* Black electrolytic cap: White stripe is **NEGATIVE**.

* Blue Tantalum cap: White stripe is **POSITIVE**.

* Yellow ceramic cap: No polarity.

![Alt text](photos/macse/ref.jpeg)

----

Push the power switch into the plate until it clicks in place.

Make sure the **hole is on top** and **legs faces down**.

![Alt text](photos/macse/swplate.jpeg)

Insert into power switch PCB, make sure it sits flat and level.

Then solder it and the right-angle pin header in place.

![Alt text](photos/macse/swpcb.jpeg)

### Cleaning

This is optional, but I like to clean off the flux with 90%+ isopropyl alcohol. Submerge and scrub with a toothbrush.

Make sure it is **completely dry** before proceeding.

### Inspection

* Compare with the reference photo and notes above. Make sure everything is in correct orientation.

* Solder joints should be **shiny and smooth**. If you see spikes, put on more flux and melt it again.

* There must be **no solder bridges**. If any, put on flux and melt it to remove.

![Alt text](photos/macse/bottom.jpeg)

## Board Features

Install two fuses as shown below:

![Alt text](photos/macse/feature.png)

### Fuse

* Use common car fuse RATED **5A OR LESS**

* Regular, Mini, and low-profile Mini all will work. Simply push into the holder.

* **DO NOT BYPASS FUSES**

### Power Switch

The pin header is connected to the ATX `PS_ON` pin.

Shorting them together turns on the PSU.

### PC Fan Header

* Any standard PC fan should work

## Pre-flight Checks

Use a multimeter to **check for dead shorts** between each power pin and GND:

![Alt text](photos/macse/voltage.png)

If all good, plug in Pico ATX PSU, short the two pins on the switch header, and plug in 12V power.

The PSU should turn on, **measure the voltage on each rail** and confirm they are within spec.

## Installation

We're going to take a rather large portion of the Macintosh apart, so make sure to **take plenty of photos** along the way! 

Snap a photo before removing a screw or unplugging a connector! It never hurts to have reference.

### Remove Back Cover

⚠️**Dangerous CRT voltage inside**! Make sure the computer is **unplugged for a few hours**! Or discharge the CRT yourself.

* You'll need a LONG **Torx T15 screwdriver**.

* Lay the Mac face down on a soft towel

* Loosen all the screws. Two near the ports, two in the handles.

* Take photos of which goes in where, the lower two has a thinner thread.

* Remove all the screws **apart from a single one inside the handle**.

![Alt text](photos/macse/back.jpeg)

* Put the screwdriver on that single loosened screw, grab the handle and try **gently** lifting up. The back cover should pop loose.

* Slowly **lift straight up** to remove the back cover.

![Alt text](photos/mac_plus/backoff.gif)

### Remove Old PSU

Further disassembly is needed to remove the old PSU.

* First, remove the screw for the green earth wire

![Alt text](photos/macse/earth.jpeg)

* Remove the expansion bracket if present

![Alt text](photos/macse/bracket.jpeg)

* Unplug the neck board by **gently lifting straight up**

![Alt text](photos/macse/neck.jpeg)

* Unplug the floppy and power cable from motherboard.

* **DO NOT YANK STRAIGHT OUT**, or you might break the CRT neck!

* Wiggle gently until loose, and carefully unplug.

![Alt text](photos/macse/ribbon.jpeg)

* Same with power connector, unlock the latch and gently wiggle it free. Careful with the CRT neck!

* If there's not enough space on SE/30, wait until motherboard is detached, then unplug.

![Alt text](photos/macse/mbpower.jpeg)

* Finally, the speaker wire, same thing.

![Alt text](photos/macse/speak.jpeg)

* Now you can remove the motherboard

* [**Mac SE**] Lift straight up along the rails.

* [**SE/30**] Lift up slightly, match the notch on the PCB to the notch on the right-hand-side rail, and it should release from the side.

* With motherboard out of the way, remove the 4 screws to release the drive cage

* Careful with CRT neck while lifting it out!

![Alt text](photos/macse/cage.jpeg)

* Unplug the Molex connector and 14-pin power connector

* Now we have enough room to remove the build-in PSU!

![Alt text](photos/macse/conn.jpeg)

* Remove the PSU screws, support it with your hand so it doesn't fall over.

![Alt text](photos/macse/psuscrew.jpeg)

* Try rotate the PSU free, unplug, and remove. Careful not to bump into CRT glass.

![Alt text](photos/macse/rot.jpeg)

That's it! The main culprit is out!

### While You're Here...

With everything apart, it might be a good idea to perform some maintenance.

Ideas include:

* [Clean and lube the floppy drive](https://www.youtube.com/watch?v=0pGhwtyFG2I)

* Check motherboard for corrosion and leakage

* [Re-cap the motherboard](https://www.youtube.com/watch?v=QArvemlZUJY) if not already done

* [Check analog board](https://www.youtube.com/watch?v=zC0qi5dQsWs) for cracked solder joints

* General cleaning / blow out dust

### Install PicoPSU

With maintenance done, time to install the new PSU!

* Insert two screws into the mounting holes near the edge, then install the standoffs from the other side

* Use 5mm socket bit to tighten.

![Alt text](photos/macse/edge.png)

* Plug PicoPSU into ATX connector

* Use jumper wire to connect the header between two PCBs

![Alt text](photos/macse/assy.jpeg)

* Undo the locking ring on the barrel jack, insert through the hole, reinstall the ring to fix it in place.

![Alt text](photos/macse/sw.jpeg)

* Plug the adaptor into the analog board as shown

* Make sure connector is lined up (NOT OFF-BY-ONE), and push firmly so it's all the way in.

* Install the power switch PCB on the standoffs, and install two more standoffs to hold in place.

![Alt text](photos/macse/new.jpeg)

* That's it! You're done!

### Putting it Back Together

Time to put everything back! Pretty much the opposite of disassembly!

* **Careful with CRT neck** AT ALL TIMES!

* Plug Molex and motherboard power connector back into analog board

* Reinstall drive cage

* Reinstall motherboard

* Plug in speaker wire, power connector, SCSI and floppy cable.

* Reinstall CRT neck board

* (If present) Reinstall expansion bracket

* Double check for short circuit if you want

If everything checks out, take a breath, plug it in and turn it on.

If your Mac was working before, hopefully it still does!

If the Mac is of unknown condition, now you'll find out!

![Alt text](photos/macse/half.jpeg)

And if it doesn't work, [check out the troubleshooting guide](#troubleshooting). 

### Adding a Fan

There's already a fan inside Mac SE, but you can add another one or replace it.

Any regular PC fan should work.

Make sure the fan is secured, nothing touches the blade, and air flow direction is correct.

**Don't mount the fan too close to the CRT**, or the picture might wobble from the motor's magnetic field.

### Blanking Plate

* Pull apart the nylon rivets

* Insert the "hollow tube" into a blanking plate

* Cover the hole from outside, then the other plate from inside, make sure the tube goes through both.

* Insert the "plunger" to fasten it together.

![Alt text](photos/macse/rivet.png)

## Congratulations!

Put the rear shell back on (**don't forget the paper insulation over the motherboard!**), and you're done!

With the new PSU, a fresh maintenance, and upgraded cooling, your Mac should continue to provide entertainment for years to come!

![Alt text](photos/macse/money.jpeg)

What's with the wireless keyboard and mouse? [Check out USB4VC!](https://github.com/dekuNukem/USB4VC/blob/master/README.md)

## Troubleshooting

This adaptor eliminates the PSU from the equation, but that's only part of the puzzle!

If something else is wrong, you still need to fix it.

### Nothing Happens / Garbled Screen

* Look for corrosion from battery / capacitor leakage on the motherboard.

* Mac SE/30 WILL have leaking caps, and you'll need to recap before it will work.

* Check for blown fuse, or shorts on power rails.

### CRT Geometry Messed Up

I had this happen with a knock-off generic PicoPSU, changing to another one fixed it.

### Screen Wobbles

* If it happens when floppy drive is active, try using a beefier power brick, or add more decoupling capacitors.

* If happens while idle, make sure the fan is not too close to the CRT.

### Other Failures

Other common issues include:

* Cracked solder joints

* Dirty contacts / Bad RAMs

I highly recommend watching [Adrian's Digital Basement Macintosh Repair-a-thon](https://www.youtube.com/watch?v=lKD65I86XGQ), where he covers a lot of those in detail.

The **power connector** and CRT **deflection capacitors** are notorious for cracking, here are some examples on mine:

![Alt text](photos/mac_plus/crack1.jpeg)

![Alt text](photos/mac_plus/crack2.jpeg)

It might be very difficult to see with naked eye, so use magnification!

Flux + new solder should fix it right up, if you find one crack might as well do the whole row.

## Questions or Comments?

Feel free to ask in official [Discord Chatroom](https://discord.gg/T9uuFudg7j), raise a [Github issue](https://github.com/dekuNukem/PicoRC/issues), or email `dekunukem` `gmail.com`!
