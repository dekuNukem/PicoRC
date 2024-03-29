# PicoPSU Adaptor for IBM PC Compatibles

[Purchase Link](https://www.tindie.com/products/31437) | [Official Discord](https://discord.gg/HAuuh3pAmB) | [Table of Contents](#table-of-contents)

----

This adaptor lets you use **Pico ATX PSU** on IBM PC and clones. 

From IBM 5150 all the way to Pentium III era!

![Alt text](photos/ibmpc/title.jpeg)

The PSU-in-a-Card replaces the original PSU, and uses very common **12V power brick** instead.

![Alt text](photos/ibmpc/backplug.jpeg)

## Features

* **Non-destructive**

* Onboard **-5V regulator**

* **PC fan** header

* Built-in power switch. Also supports external switch.

## Compatibility

It works on **any** machine with an **ISA slot** and **AT-style** (or similar) power connector.

Also works with **IBM 5155 Portable Personal Computer**, [click me to learn more!](./ibm5155.md)

## Get One / Other Stuff

[Click me to get one!](https://www.tindie.com/products/31437)

Also available for [**Compact Macintosh, Apple II/IIGS, Osborne 1, Apricot PC, BBC Micro, and more!**](./README.md)

For more general-purpose diagnostics and retrofitting, check out the [full-fat ATX4VC](https://github.com/dekuNukem/ATX4VC)!

## Table of Contents

- [Getting a Pico PSU](#getting-a-pico-psu)

- [Kit Assembly](#kit-assembly)

- [Installation](#installation)

- [External Power Switch](#external-power-switch)

- [Questions or Comments?](#questions-or-comments)

## Getting a Pico PSU

PicoPSUs are tiny ATX power supplies for small PCs, but are perfect for retro computers as well.

![Alt text](photos/mac_plus/pico.jpg)

* [Official website](https://www.mini-box.com/DC-DC) and [distributors](https://www.mini-box.com/site/resellers.html).

* The **160W** one is recommended.

* The cheaper 80 or 120W should also work on PCs **without** spinning hard drives.

* Avoid generic clones. They over-rate and are of low quality.

* A power brick with **12V DC** and **center positive** 5.5x2.5mm barrel jack is needed.

* They are very popular and you might already have one. Make sure it has enough wattage.

Remember that this solution is **only as good as your PicoPSU and 12V Brick**, so don't skimp on them!

## Kit Assembly

* 🚨🚨🚨🚨 This guide is for **IBM PC COMPATIBLES**, [CLICK ME FOR IBM 5155 PORTABLE PC](./ibm5155.md) 🚨🚨🚨🚨
* 🚨🚨🚨🚨 This guide is for **IBM PC COMPATIBLES**, [CLICK ME FOR IBM 5155 PORTABLE PC](./ibm5155.md) 🚨🚨🚨🚨
* 🚨🚨🚨🚨 This guide is for **IBM PC COMPATIBLES**, [CLICK ME FOR IBM 5155 PORTABLE PC](./ibm5155.md) 🚨🚨🚨🚨
* 🚨🚨🚨🚨 This guide is for **IBM PC COMPATIBLES**, [CLICK ME FOR IBM 5155 PORTABLE PC](./ibm5155.md) 🚨🚨🚨🚨

**DON'T START YET!!!** Keep reading :)

Observe the parts:

![Alt text](photos/ibmpc/part.png)

Optional External Power Switch Kit:

![Alt text](photos/ibmpc/buttonkit.png)

### Soldering Notes

Nothing too tricky in this kit, all basic through-hole stuff.

If this is your first time, a few tips:

* Make sure your soldering iron has **proper temperature control**. Try your local makerspace or university lab.

* Use **leaded solder** and plenty of flux, temperature around 320C / 600F.

* [This video](https://www.youtube.com/watch?v=AqvHogekDI4) covers the basics pretty well.

### Assembly

Solder the components **as shown below**:

![Alt text](photos/ibmpc/topside.png)

* Double check capacitor polarity!

* Black electrolytic caps: White stripe is **NEGATIVE**.

* Blue Tantalum caps: White stripe is **POSITIVE**.

* Yellow ceramic caps: No polarity.

### Cleaning

This is optional, but I like to clean off the flux with 90%+ isopropyl alcohol.

Submerge and scrub with a toothbrush.

Make sure it is **completely dry** before proceeding.

### Inspection

* Compare with the photo and notes above. Make sure everything is in correct orientation.

* Solder joints should be **shiny and smooth**. If you see spikes, put on more flux and melt it again.

* There must be **no solder bridges**. If any, put on flux and melt it to remove.

![Alt text](photos/ibmpc/bottomside.jpeg)

### Bracket

Install the metal bracket.

The shorter side should be touching the PCB.

Secure with M3 screws from the bottom.

![Alt text](photos/ibmpc/short.png)

Then install the ISA bracket, secure with two more M3 screws.

![Alt text](photos/ibmpc/brackets.jpeg)

Installation

Install two 5A fuses.

![Alt text](photos/ibmpc/fuses.jpeg)

Use a multimeter to **check for dead shorts** between each power rail and GND:

![Alt text](photos/ibmpc/fingers.png)

If all good, plug in PicoPSU, and flip the switch.

![Alt text](photos/ibmpc/test.png)

The LED should light up. The LED is wired to the `POWER_GOOD` signal, so there might be a slight delay.

Measure the voltage of each rail, make sure they are correct. 

---------

Undo the locking ring on the barrel jack.

Insert through the hole on the bracket.

Tighten the ring from the other side. Use 10mm socket.

![Alt text](photos/ibmpc/jack.jpeg)

Insert the power cables into the terminal blades.

* Match the colours! (RED: 5V | ORANGE: PowerGood | BLACK: GND)

* Ensure the connectors are **all the way in**.

* Ensure the **insulating sleeves** are in place.

![Alt text](photos/ibmpc/conn.png)

Now we're ready to install!

* 🚨🚨🚨🚨 This guide is for **IBM PC COMPATIBLES**, [CLICK ME FOR IBM 5155 PORTABLE PC](./ibm5155.md) 🚨🚨🚨🚨
* 🚨🚨🚨🚨 This guide is for **IBM PC COMPATIBLES**, [CLICK ME FOR IBM 5155 PORTABLE PC](./ibm5155.md) 🚨🚨🚨🚨
* 🚨🚨🚨🚨 This guide is for **IBM PC COMPATIBLES**, [CLICK ME FOR IBM 5155 PORTABLE PC](./ibm5155.md) 🚨🚨🚨🚨
* 🚨🚨🚨🚨 This guide is for **IBM PC COMPATIBLES**, [CLICK ME FOR IBM 5155 PORTABLE PC](./ibm5155.md) 🚨🚨🚨🚨

I'll be using an IBM PC XT as an example.

**⚠️⚠️ Insert the blanking plug into the power socket. ⚠️⚠️**

This prevents the old faulty/unknown PSU from being accidentally energized.

![Alt text](photos/ibmpc/plug.jpeg)

Undo the screws in the back, and slide the cover forward to remove.

![Alt text](photos/ibmpc/xtback.jpeg)

Insert the card into a free ISA slot, secure with screw.

![Alt text](photos/ibmpc/slot.jpeg)

Insert a flat-blade screwdriver into the blade receptacle.

Expand the gap slightly so it goes in easier.

![Alt text](photos/ibmpc/expand.png)

Now take a look at the AT-style connector.

We just need to insert the cables into the appropriate pins.

Other rails will be fed through the ISA bus.

![Alt text](photos/ibmpc/rails.png)

Let's start with the **RED** 5V cable.

Any will do, but I suggest the rightmost pin, easier to remember.

Push **straight down**, make sure **lobe side faces outwards**.

Don't force if there is significant resistance, make the gap bigger and try again.

Of course, it shouldn't be too loose either.

![Alt text](photos/ibmpc/lobe.png)

Repeat with the other two wires.

**BLACK** GND wire can be any of the four pins in the middle.

**ORANGE** PG wire is on the other end.

Make sure they are **all the way in**, and covered with **insulation sleeve**.

![Alt text](photos/ibmpc/fff.png)

Double check the connection:

![Alt text](photos/ibmpc/ttt.png)

---------

Some PCs use **non-standard connectors**, in which case you'll need to figure it out yourself.

* Check schematic if available.

* 5V is almost always **RED**.

* GND is almost always **BLACK**.

* PG can be different, but AT convention is **ORANGE**.

A few examples:

#### Dell 466/T

The connector is in two rows, but everything else is the same. So just match the colors.

![Alt text](photos/ibmpc/466t.jpeg)

#### Hyundai/Novel PCTerminal (HPT-100)

![Alt text](photos/ibmpc/pcterm.jpeg)

It uses a different connector, but the pinout is mostly the same (RED 5V on the edge, BLACK GND in the middle, PG is unused).

It also has square pins, in which case you can plug one lobe of the receptacle into it.

![Alt text](photos/ibmpc/square.jpeg)

#### Compaq Deskpro 286

This one's a doozy, completely propitiatory connector and pinout.

Most rails are labelled, but not the PG signal, couldn't find a schematic.

In this case, you can open up the PSU and see if it is labelled there. 

[Fortunately it was](photos/ibmpc/compaqpsu.jpeg), so here is the pinout for prosperity:

![Alt text](photos/ibmpc/compaq.png)

## Moment of Truth

If testing an unknown PC, it is recommended to start minimal with just the motherboard and video card. Remove all extra cards and disconnect the drives.

Plug in and flip the switch!

![Alt text](photos/ibmpc/flip.jpeg)

If it works, congrats! You can now add more parts back in.

For drives, use the harness that came with the PicoPSU.

![Alt text](photos/ibmpc/molex.png)

Keep an eye on the temperature of the PicoPSU.

Active ventilation might be needed if it gets too hot.

Any standard 12V PC fan should work.

![Alt text](photos/ibmpc/fan.jpeg)

## External Power Switch

The **PSW header** is for external power switch.

The PSU will turn on when the two pins are shorted together.

![Alt text](photos/ibmpc/psw.jpeg)

Normally you can simply connect a switch or latching button to it.

However, if you want to use the Big Red Switch™, there are a few more steps.

![Alt text](photos/ibmpc/red.jpg)

Normally, the Big Red Switch™ is part of the old PSU, so you would need to take it apart.

Inside, you'll most likely find a Double Pole Single Throw (DPST) switch, which switches two circuits at once.

![Alt text](photos/ibmpc/oldpsu.jpeg)

Note the colour of the wires.

The **same colored** wire are **connected together** when the switch is on.

![Alt text](photos/ibmpc/dpst.png)

⚠️⚠️ **MAINS VOLTAGE flows through this switch!!!** ⚠️⚠️ 

⚠️⚠️ Make sure to first **unplug/cut/desolder** ALL WIRES going into the switch! ⚠️⚠️ 

--------

To assemble the test clip, pull off the cap, insert the wire through the hole in the cap, solder the wire, and reinstall the cap.

![Alt text](photos/ibmpc/clipass.jpeg)

You can then hook up one side of the switch to the clips.

⚠️⚠️ Again, make sure **all original wires to the Big Red Switch™ has been disconnected!** ⚠️⚠️

![Alt text](photos/ibmpc/clip.jpeg)

![Alt text](photos/ibmpc/clipped.jpeg)

Tuck all the original wiring inside the case. We won't be using them anymore.

Make sure they don't knock loose the test clips.

Now the Big Red Switch™ wires should be the only thing that exits the case.

![Alt text](photos/ibmpc/tuck.jpeg)

It's also a good opportunity to replace the original cooling fan.

Any good quality **PC fan** should work, usually 80mm but do double check.

![Alt text](photos/ibmpc/pcfan.jpeg)

Reinstall the deactivated old PSU, plug the fan header and power switch header into the adaptor.

![Alt text](photos/ibmpc/newconn.jpeg)

That's it! Now the Big Red Switch™ will control the power!

![Alt text](photos/ibmpc/xt.jpeg)

What's with the wireless keyboard and mouse? [Check out USB4VC!](https://github.com/dekuNukem/USB4VC/blob/master/README.md)

## Questions or Comments?

Feel free to ask in official [Discord Chatroom](https://discord.gg/T9uuFudg7j), raise a [Github issue](https://github.com/dekuNukem/PicoRC/issues), or email `dekunukem` `gmail.com`!
