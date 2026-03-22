# PicoRC PSU Kit for Sirius 1 / Victor 9000

[Purchase Link](https://www.tindie.com/) | [Official Discord](https://discord.gg/HAuuh3pAmB) | [Table of Contents](#table-of-contents)

----

A replacement PSU kit for **Sirius 1 / Victor 9000**

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

Mean Well

80mm PC Fan

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

[Photo: PSU two halves separated]

* Undo screws
* Remove the circuit board

[Photo: Looking into PSU with original PCU, no mains power wires, no fan wires, output harness unplugged]


## Questions or Comments?

Feel free to ask in official [Discord Chatroom](https://discord.gg/T9uuFudg7j), raise a [Github issue](https://github.com/dekuNukem/PicoRC/issues), or email `dekunukem` `gmail.com`!
