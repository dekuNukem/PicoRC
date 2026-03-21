# PicoRC PSU Kit for Sirius 1 / Victor 9000

[Purchase Link](https://www.tindie.com/) | [Official Discord](https://discord.gg/HAuuh3pAmB) | [Table of Contents](#table-of-contents)

----

A replacement PSU kit for **Sirius 1 / Victor 9000**

![Alt text](photos/sirius1/title.jpeg)

* **Non-destructive** and **Reversible**
	* Reuses Existing Hardware
	* Original Appearance
* **PC Fan** Header
	* Quieter & improved cooling with modern PC fan
* Mean Well PSU with Fused Rails

![Alt text](photos/sirius1/money.jpeg)

## Get One

* United Kingdom
	* [Kit]()
	* [Fully Assembled]()
* [USA / EU / Rest of World]()

Also available for [**many other computers.**](./README.md)

For more general-purpose diagnostics and retrofitting, [check out ATX4VC](https://github.com/dekuNukem/ATX4VC).

## Shopping List

Mean Well

80mm PC Fan

## Kit Assembly

**DON'T START YET!!!** Keep reading :)

You should have the following:

![Alt text](photos/sirius1/part.png)

### Soldering Notes

Nothing too tricky in this kit, all basic through-hole stuff.

If this is your first time, a few tips:

* Make sure your soldering iron has **proper temperature control**. Try your local makerspace or university lab.

* Use **leaded solder** and plenty of flux, temperature around 320C / 600F.

* [This video](https://www.youtube.com/watch?v=AqvHogekDI4) covers the basics pretty well.

### Assembly

Solder the components **as shown below**:

![Alt text](photos/sirius1/topside.png)

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

![Alt text](photos/sirius1/bottomside.jpeg)

### Bracket

Install the metal bracket.

The shorter side should be touching the PCB.

Secure with M3 screws from the bottom.

![Alt text](photos/sirius1/short.png)

Then install the ISA bracket, secure with two more M3 screws.

![Alt text](photos/sirius1/brackets.jpeg)

Installation

Install two 5A fuses.

![Alt text](photos/sirius1/fuses.jpeg)

Use a multimeter to **check for dead shorts** between each power rail and GND:

![Alt text](photos/sirius1/fingers.png)

If all good, plug in PicoPSU, and flip the switch.

![Alt text](photos/sirius1/test.png)

The LED should light up. The LED is wired to the `POWER_GOOD` signal, so there might be a slight delay.

Measure the voltage of each rail, make sure they are correct. 

---------

Undo the locking ring on the barrel jack.

Insert through the hole on the bracket.

Tighten the ring from the other side. Use 10mm socket.

![Alt text](photos/sirius1/jack.jpeg)

Insert the power cables into the terminal blades.

* Match the colours! (RED: 5V | ORANGE: PowerGood | BLACK: GND)

* Ensure the connectors are **all the way in**.

* Ensure the **insulating sleeves** are in place.

![Alt text](photos/sirius1/conn.png)

Now we're ready to install!

* 🚨🚨🚨🚨 This guide is for **IBM PC COMPATIBLES**, [CLICK ME FOR IBM 5155 PORTABLE PC](./ibm5155.md) 🚨🚨🚨🚨
* 🚨🚨🚨🚨 This guide is for **IBM PC COMPATIBLES**, [CLICK ME FOR IBM 5155 PORTABLE PC](./ibm5155.md) 🚨🚨🚨🚨
* 🚨🚨🚨🚨 This guide is for **IBM PC COMPATIBLES**, [CLICK ME FOR IBM 5155 PORTABLE PC](./ibm5155.md) 🚨🚨🚨🚨
* 🚨🚨🚨🚨 This guide is for **IBM PC COMPATIBLES**, [CLICK ME FOR IBM 5155 PORTABLE PC](./ibm5155.md) 🚨🚨🚨🚨

I'll be using an IBM PC XT as an example.

**⚠️⚠️ Insert the blanking plug into the power socket. ⚠️⚠️**

This prevents the old faulty/unknown PSU from being accidentally energized.

![Alt text](photos/sirius1/plug.jpeg)

Undo the screws in the back, and slide the cover forward to remove.

![Alt text](photos/sirius1/xtback.jpeg)

Insert the card into a free ISA slot, secure with screw.

![Alt text](photos/sirius1/slot.jpeg)

Insert a flat-blade screwdriver into the blade receptacle.

Expand the gap slightly so it goes in easier.

![Alt text](photos/sirius1/expand.png)

Now take a look at the AT-style connector.

We just need to insert the cables into the appropriate pins.

Other rails will be fed through the ISA bus.

![Alt text](photos/sirius1/rails.png)

Let's start with the **RED** 5V cable.

Any will do, but I suggest the rightmost pin, easier to remember.

Push **straight down**, make sure **lobe side faces outwards**.

Don't force if there is significant resistance, make the gap bigger and try again.

Of course, it shouldn't be too loose either.

![Alt text](photos/sirius1/lobe.png)

Repeat with the other two wires.

**BLACK** GND wire can be any of the four pins in the middle.

**ORANGE** PG wire is on the other end.

Make sure they are **all the way in**, and covered with **insulation sleeve**.

![Alt text](photos/sirius1/fff.png)

Double check the connection:

![Alt text](photos/sirius1/ttt.png)

---------

Some PCs use **non-standard connectors**, in which case you'll need to figure it out yourself.

* Check schematic if available.

* 5V is almost always **RED**.

* GND is almost always **BLACK**.

* PG can be different, but AT convention is **ORANGE**.

A few examples:

#### Dell 466/T

The connector is in two rows, but everything else is the same. So just match the colors.

![Alt text](photos/sirius1/466t.jpeg)

#### Hyundai/Novel PCTerminal (HPT-100)

![Alt text](photos/sirius1/pcterm.jpeg)

It uses a different connector, but the pinout is mostly the same (RED 5V on the edge, BLACK GND in the middle, PG is unused).

It also has square pins, in which case you can plug one lobe of the receptacle into it.

![Alt text](photos/sirius1/square.jpeg)

#### Compaq Deskpro 286

This one's a doozy, completely propitiatory connector and pinout.

Most rails are labelled, but not the PG signal, couldn't find a schematic.

In this case, you can open up the PSU and see if it is labelled there. 

[Fortunately it was](photos/sirius1/compaqpsu.jpeg), so here is the pinout for prosperity:

![Alt text](photos/sirius1/compaq.png)

## Moment of Truth

If testing an unknown PC, it is recommended to start minimal with just the motherboard and video card. Remove all extra cards and disconnect the drives.

Plug in and flip the switch!

![Alt text](photos/sirius1/flip.jpeg)

If it works, congrats! You can now add more parts back in.

For drives, use the harness that came with the PicoPSU.

![Alt text](photos/sirius1/molex.png)

Keep an eye on the temperature of the PicoPSU.

Active ventilation might be needed if it gets too hot.

Any standard 12V PC fan should work.

![Alt text](photos/sirius1/fan.jpeg)

## External Power Switch

The **PSW header** is for external power switch.

The PSU will turn on when the two pins are shorted together.

![Alt text](photos/sirius1/psw.jpeg)

Normally you can simply connect a switch or latching button to it.

However, if you want to use the Big Red Switch™, there are a few more steps.

![Alt text](photos/sirius1/red.jpg)

Normally, the Big Red Switch™ is part of the old PSU, so you would need to take it apart.

Inside, you'll most likely find a Double Pole Single Throw (DPST) switch, which switches two circuits at once.

![Alt text](photos/sirius1/oldpsu.jpeg)

Note the colour of the wires.

The **same colored** wire are **connected together** when the switch is on.

![Alt text](photos/sirius1/dpst.png)

⚠️⚠️ **MAINS VOLTAGE flows through this switch!!!** ⚠️⚠️ 

⚠️⚠️ Make sure to first **unplug/cut/desolder** ALL WIRES going into the switch! ⚠️⚠️ 

--------

To assemble the test clip, pull off the cap, insert the wire through the hole in the cap, solder the wire, and reinstall the cap.

![Alt text](photos/sirius1/clipass.jpeg)

You can then hook up one side of the switch to the clips.

⚠️⚠️ Again, make sure **all original wires to the Big Red Switch™ has been disconnected!** ⚠️⚠️

![Alt text](photos/sirius1/clip.jpeg)

![Alt text](photos/sirius1/clipped.jpeg)

Tuck all the original wiring inside the case. We won't be using them anymore.

Make sure they don't knock loose the test clips.

Now the Big Red Switch™ wires should be the only thing that exits the case.

![Alt text](photos/sirius1/tuck.jpeg)

It's also a good opportunity to replace the original cooling fan.

Any good quality **PC fan** should work, usually 80mm but do double check.

![Alt text](photos/sirius1/pcfan.jpeg)

Reinstall the deactivated old PSU, plug the fan header and power switch header into the adaptor.

![Alt text](photos/sirius1/newconn.jpeg)

That's it! Now the Big Red Switch™ will control the power!

![Alt text](photos/sirius1/xt.jpeg)

What's with the wireless keyboard and mouse? [Check out USB4VC!](https://github.com/dekuNukem/USB4VC/blob/master/README.md)

## Questions or Comments?

Feel free to ask in official [Discord Chatroom](https://discord.gg/T9uuFudg7j), raise a [Github issue](https://github.com/dekuNukem/PicoRC/issues), or email `dekunukem` `gmail.com`!
