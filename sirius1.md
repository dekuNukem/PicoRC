# PicoRC PSU Kit for Sirius 1 / Victor 9000

[Purchase Link](https://www.tindie.com/) | [Official Discord](https://discord.gg/HAuuh3pAmB) | [Table of Contents](#table-of-contents)

----

A replacement PSU kit for **Sirius 1 / Victor 9000** Computers

![Alt text](photos/sirius1/title.jpeg)

* **Non-destructive** and **Reversible**
	* Reuses Existing Hardware
	* Original Appearance
* Modern **PC Fan** Support
	* Quieter & improved cooling
* Mean Well PSU with Fused Rails
	* Low-cost and reliable

![Alt text](photos/sirius1/back.jpeg)

![Alt text](photos/sirius1/money.jpeg)

## Get One

* United Kingdom
	* [Kit]()
	* [Fully Assembled]()
* [USA / EU / Rest of World]()

Also available for [**many other computers.**](./README.md)

For more general-purpose diagnostics and retrofitting, [check out ATX4VC](https://github.com/dekuNukem/ATX4VC).

## Shopping List

Apart from the kit itself, you also need to buy a **Mean Well PSU** and a **80mm PC Fan**.

### Mean Well PSU

This kit uses **Mean Well RT-65B** Chassis Mount PSU.

It provides +5V, +12V, and -12V needed by the computer.

Inexpensive and good quality at around 20USD/GBP.

Buy from a reputable distributer such as DigiKey, Mouser, or RS components. (**NOT ebay or aliexpress**)

**MAKE SURE IT IS THE "B" VARIANT!**

### 80mm PC Fan

Used to replace the fan

Any 4-pin 80mm PC fan should work. 

## Kit Assembly

**DON'T START YET!!!** Keep reading :)

You should have the following:

![Alt text](photos/sirius1/parts.png)

### Soldering Notes

Nothing too tricky in this kit, all basic through-hole stuff.

If this is your first time:

* Make sure your soldering iron has **proper temperature control**
	* Try your local makerspace or university lab
* Use **leaded solder** and plenty of flux
	* Temperature around 350C / 660F.
* [This video](https://www.youtube.com/watch?v=AqvHogekDI4) covers the basics pretty well

### Assembly

* Solder the components **as shown below**:

![Alt text](photos/sirius1/topside.png)

* Double check polarity!
	* Black electrolytic capacitor: White stripe is **NEGATIVE**.
	* Blue Tantalum capacitor: White stripe is **POSITIVE**.
	* Yellow ceramic capacitor: No polarity.
	* Inductor / Choke: No polarity.

-----

* On the MeanWell PSU, install the ring terminal cable on the rails shown.
	* Undo Screw
	* Insert through ring (flat side down)
	* Redo Screw

![Alt text](photos/sirius1/meanwell1.jpeg)

* Fasten the MeanWell PSU to the PCB with M3 screws

![Alt text](photos/sirius1/fast.png)

* Bend the wires
* Insert strands through corresponding holes
	* Make sure **all strands goes through**
	* And **no loose strands being caught on top side**

![Alt text](photos/sirius1/bent.png)

### Inspection

* Compare with photos and notes above.
	* Ensure everything has correct polarity.
* Solder joints should be **shiny and smooth**.
	* If you see spikes, put on more flux and melt it again.
* There must be **no solder bridges**.

![Alt text](photos/sirius1/clean.jpeg)

### Installation

* Remove 4 screws on the back

![Alt text](photos/sirius1/backcase.png)

* Unhinge the back cover **from top side**
	* Might need a gentle tug due to velcro pads
* Reach in and unplug the **reset button**

![Alt text](photos/sirius1/velcro.png)

* Remove top cover
* Unplug the power connector
* Remove 5 screws

![Alt text](photos/sirius1/remove.png)

* Rotate PSU away
* Unplug both power connectors

![Alt text](photos/sirius1/unplug.png)

* Remove the PSU Completely
* Insert the screws back in their holes for safekeeping
	* Finger tight is fine
* Put the computer away for now

![Alt text](photos/sirius1/screwback.png)

* Remove 7 screws on the PSU

![Alt text](photos/sirius1/psuscrew1.jpeg)

![Alt text](photos/sirius1/psuscrew2.jpeg)

* Split the PSU in half
* Unplug the connectors shown
* Reinstall screws for safekeeping

![Alt text](photos/sirius1/split.png)

* On the fan connector:
	* Press down on the metal tab with a **thin flathead screwdriver**
	* AND **gently pull on the cable**
	* It should release

![Alt text](photos/sirius1/press.png)

* Separate the two halves
* Leave the main harness inside for now

[Photo: PSU two halves separated]

* Undo screws
* Remove the circuit board

[Photo: Looking into PSU with original PCU, no mains power wires, no fan wires, output harness unplugged]

* Observe the **four highlighted screw holes** inside the metal case
* Some are **bare holes**, some have **threaded inserts**.
	* Numbers can be different
	* You may have 2 each, or 3 & 1.

![Alt text](photos/sirius1/holes.png)

* Install **M3 Screws and Standoffs** on the PCB
	* **ONLY** on corners with **bare holes**

![Alt text](photos/sirius1/standoff.png)

![Alt text](photos/sirius1/bare.png)

* Lower the PCB assembly into the case.
* Ensure holes line up
	* You can loosen screws slightly to adjust
* Use original screws for threaded inserts

![Alt text](photos/sirius1/incase.png)

* Flip over
* Install **M3 Nuts** on bare holes
* We're done with this half of the case!
	* Put it away for now

![Alt text](photos/sirius1/bareback.png)

* Take out the other half
* Undo the four screws to remove the fan

![Alt text](photos/sirius1/fanback.png)

* Install the new PC Fan
	* Fan should **blow air OUT of case**
		* See arrow on the fan shroud for air direction
	* Ensure the cable is on the corner shown
	* You can use the original nuts & bolts
	* But if the fan comes with self-tapping screws, you can use those too.

![Alt text](photos/sirius1/fan.png)

* Next up: Power Connection
	* ⚠️ **Involves mains voltage!**
	* Ensure everything is unplugged
	* Pay attention to the instructions!

* Look at the connector that plugs into the old PSU
	* It should have **two wires**.
	* Brown is **LIVE**
		* Comes out of **fuse holder**
	* White is **Neutral**
		* Comes out of the **power switch**
	* **Remember where they go!**
		* Take photos!

![Alt text](photos/sirius1/conn.png)

* Unplug the **LIVE** wire from the **Fuse Holder**
	* Use a **pair of pliers**
	* Grab the **NECK**
	* Wiggle side-to-side and pull
	* **DO NOT** pull on the wire itself!
* Plug the new **BROWN** wire into the same terminal.
	* All the way in
	* Ensure the **protective cover is in place**

![Alt text](photos/sirius1/post.png)

* Unplug the old **white Neutral** wire
* Plug in the new **blue Neutral** wire
	* Same precautions

![Alt text](photos/sirius1/blue.png)

* On the home stretch now!
* Plug the output harness into the PCB
	* Match the **missing pin**
	* **Check BOTH ends** to ensure it's not off-by-one.
* Insert fan cable through the grommet
	* Plug into fan header
* Install mains wires to MeanWell PSU
	* Neutral: Blue
	* Live: Brown
* Double check all terminal connections
	* Should be tight
	* No rattles

![Alt text](photos/sirius1/final.png)

* Put the two halves back together
	* Remove hand-tight temp screws
	* Tuck wires, ensure nothing is pinched.
	* Redo the screws

Take a breath and turn it on **by itself**!

Good signs include:

* Not blowing up
* Fan spins
* Power light is on

If so, congrats!

![Alt text](photos/sirius1/run.jpeg)

* Before reinstalling, double check voltage
	* Use a multimeter
	* Black probe on metal case (Use a screw to hold in place)
	* Touch red probe on each metal contact 
	* Make sure voltage rail matches
		* ±5% is fine
		* NC = Not connected, no wires.
	* If values are completely wrong, make sure you didn't plug in the harness **backwards** or **off-by-one**.

![Alt text](photos/sirius1/volt.png)

## 💥 Exploding Caps Alert

There are a few **Tantalum Capacitors** on the **floppy controller PCB**.

As they age, they often **fail short** and **explode** or **trip the protection** circuit.

![Alt text](photos/sirius1/caps.png)

How they look like:

![Alt text](photos/sirius1/look.png)

### Check for Shorted Caps

* Multimeter, continuity mode, touch **both ends of the cap**.
* If the meter shows a dead short (less than 10 ohm), then most likely the cap has shorted.
	* You can just cut it off, no need to replace.
* If no short, you can leave it or cut it.

How they look after the big woopsie:

![Alt text](photos/sirius1/explode.png)

Anyway, now you're aware, we can continue putting it back together.

* Reconnect the power connectors
	* Match missing pins

![Alt text](photos/sirius1/backin.png)

* Remove finger-tight temp screws
* Reinstall PSU

![Alt text](photos/sirius1/reass.png)

### First Power-On

* Use eye-protection
* If a cap explodes, cut it off.
* If fuses blows or PSU goes into protection, check for shorted caps on 12V rail again.

Hopefully it works!

While you're in there, might worth giving the floppy drive a service and clean out the dust.

### Keep the Original Parts!

* **DO NOT** throw anything away!
* Put all the removed parts in a bag or box
* Clearly **label and date** for future reference

![Alt text](photos/sirius1/bag.jpeg)

Reassemble fully and enjoy!

![Alt text](photos/sirius1/money.jpeg)

## Questions or Comments?

Feel free to ask in official [Discord Chatroom](https://discord.gg/T9uuFudg7j), raise a [Github issue](https://github.com/dekuNukem/PicoRC/issues), or email `dekunukem` `gmail.com`!
