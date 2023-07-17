# PicoPSU Adaptor for Apricot PC

[Purchase Link](https://www.tindie.com/products/31080/) | [Official Discord](https://discord.gg/HAuuh3pAmB) | [Table of Contents](#table-of-contents)

----

This adaptor lets you use **Pico ATX PSU** on Apricot PC, PC XI and Apricot PC 286.

![Alt text](photos/apricot_pc/pcb.jpeg)

It replaces the original PSU, and uses very common **12V power brick** instead.

![Alt text](photos/apricot_pc/done.jpeg)

## Highlights

* **100% Non-destructive** and reversible

* **PC fan header** for added cooling

* Low cost, efficient and reliable.

## Get One / Other Stuff

[Click me to get one!](https://www.tindie.com/products/31080/)

Also available for [**Mac 128K, Mac SE, Apple II/IIGS, Osborne 1, Apricot PC, and more!**](./README.md)

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

* Generic clones are also available on eBay/Amazon/Aliexpress. They are pretty crap, so I strongly suggest using the high-quality official products.

* A power brick with **12V DC** and **center positive** 5.5x2.5mm barrel jack is needed.

* They are very popular and you might already have one. Make sure it has enough wattage.

Remember that this solution is **only as good as your PicoPSU and 12V Brick**, so don't skimp on them!

## Kit Assembly

**DON'T START YET!!!** Keep reading :)

### Required tools

* Soldering Iron

* Solder

* Flux

* Multimeter

* Pliers and flush cutter

### Parts

Observe the parts:

![Alt text](photos/apricot_pc/parts.png)

### Soldering Notes

Nothing too tricky in this kit, all basic through-hole stuff.

If this is your first time, a few tips:

* Make sure your soldering iron has **proper temperature control**. Try your local makerspace or university lab.

* Use **leaded solder** and plenty of flux, temperature around 320C / 600F.

* [This video](https://www.youtube.com/watch?v=AqvHogekDI4) covers the basics pretty well.

### Assembly

Solder the following components **as shown below**:

![Alt text](photos/apricot_pc/top.png)

* Double check capacitor polarity!

* Black electrolytic caps: White stripe is **NEGATIVE**.

* Blue Tantalum caps: White stripe is **POSITIVE**.

* Yellow ceramic caps: No polarity.

More reference photos:

![Alt text](photos/apricot_pc/ref1.jpeg)

![Alt text](photos/apricot_pc/ref2.jpeg)

### Cleaning

This is optional, but I like to clean off the flux with 90%+ isopropyl alcohol.

Submerge and scrub with a toothbrush.

Make sure it is **completely dry** before proceeding.

### Fuse

* Push in the fuses as shown.

* Use common **5-amp** automotive fuses 

* **DO NOT BYPASS FUSES**

![Alt text](photos/apricot_pc/fuse.jpeg)

### Inspection

* Compare with the reference photo and notes above. Make sure everything is in correct orientation.

* Solder joints should be **shiny and smooth**. If you see spikes, put on more flux and melt it again.

* There must be **no solder bridges**. If any, put on flux and melt it to remove.

![Alt text](photos/apricot_pc/bottom.jpeg)

## Pre-flight Checks

Use a multimeter to **check for dead shorts** between each power pin and GND:

![Alt text](photos/apricot_pc/rails.png)

## Installation

I'm using a new-to-me and untested Apricot PC for this guide, excuse the dust!

* Rest the PC on a soft towel.

* Remove the 3 screws from the back cover.

![Alt text](photos/apricot_pc/back.jpeg)

* Remove the top cover.

* Unplug / remove the connectors and grounding lugs shown below.

![Alt text](photos/apricot_pc/sep.jpeg)

* Separated the back assembly and put aside.

![Alt text](photos/apricot_pc/backremoved.jpeg)

* Unplug the power and data cable of floppy/hard drives.

* Remove the 4 screws shown

![Alt text](photos/apricot_pc/bridge.png)

* Now you can lift off the "bridge" assembly containing the drives. Put it aside.

* Remove the 4 screws shown.

![Alt text](photos/apricot_pc/nobridge.jpeg)

* Unplug motherboard power cable

* Unplug speaker cable

* Slide the metal plate backwards to remove it.

![Alt text](photos/apricot_pc/plate.jpeg)

* Flip it over, remove the four screws to release the old PSU.

* Put the screws back on the PSU casing, put it aside. Don't throw it away!

![Alt text](photos/apricot_pc/plateback.jpeg)

* Flip back again.

* Insert two screws from the bottom, then the washers, then the standoffs from top.

* Use 5mm socket bit to tighten.

![Alt text](photos/apricot_pc/standoff.jpeg)

* Install the adaptor, secure with two more screws.

![Alt text](photos/apricot_pc/installed.jpeg)

* Halfway there!

* Now reassemble the metal plate, then the drive bridge, and the drive cables.

* Also connect the new wire harness from the adaptor to motherboard.

![Alt text](photos/apricot_pc/reass.jpeg)

* Make sure the notch on the wire harness meshes with the indent on the connector **on both ends**!

![Alt text](photos/apricot_pc/mesh.jpeg)

* Bring out the back cover assembly.

* Cut off the zipties, and unplug all the blade terminal connectors.

* **Don't pull on the cable!** Use a pair of pliers, grab the neck and pull.

![Alt text](photos/apricot_pc/unplug.jpeg)

* Undo the nuts and bolts and remove the IEC socket

* Also remove the fan

![Alt text](photos/apricot_pc/iec.jpeg)

* Plug the new cable into the power switch as shown, polarity doesn't matter.

* Install a new **80mm PC Fan**, use the standoffs to help secure it.

* Double check airflow direction! The fan should push air **OUT OF** the case.

* Usually an arrow on the fan frame indicates the air direction.

![Alt text](photos/apricot_pc/fan.jpeg)

* Also install the blanking plate with the original nuts and bolts.

![Alt text](photos/apricot_pc/blank.jpeg)

* Plug in fan connector.

* Plug in PicoPSU.

* Plug in power switch wires.

![Alt text](photos/apricot_pc/final.jpeg)

* Undo the locking ring on the barrel jack

* Insert through the blanking plate.

* Secure the ring to fix it in place.

![Alt text](photos/apricot_pc/jack.jpeg)

* Put all the unneeded parts in a bag for safekeeping. **Don't throw anything away!**

![Alt text](photos/apricot_pc/bag.jpeg)

* That's pretty much it!

* Plug in the 12V jack, switch on, and see if it works!

![Alt text](photos/apricot_pc/money.jpeg)

## Questions or Comments?

Feel free to ask in official [Discord Chatroom](https://discord.gg/T9uuFudg7j), raise a [Github issue](https://github.com/dekuNukem/PicoRC/issues), or email `dekunukem` `gmail.com`!
