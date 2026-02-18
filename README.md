<h1 align="center">
MV16
</h1>

<h2 align="center">
Atari ST MV16 cartridge by UBISOFT. Remake from original.<br>
It was included with the game B.A.T. (Bureau of Astral Troubleshooters)
</h2>

---
 
<img title="Original MV16 Cartridge" style="width:44%" align=top src="Pics/Original_cart.jpg">  <img title="Original B.A.T Box" style="width:55.5%" align=top src="Pics/Box_3.jpg">  

---

<img title="Orignal Cartridge opened cardboard box" style="width:43.1%" align=top src="Pics/original_cart_opened.jpg">  <img title="Nine versions of MV16 Cartridge" style="width:56%" align=top src="Pics/9_PCB_tilted.png">

---

## Smaller then original  

I bought the original box with cartridge a while ago with the intention to reverse engineer it. The new SMT version was done around summer 2020 (covid time) and is more then half as long as the original.

---

## BOM

Bill of material (BOM is included in each gerber zip as well as text files in the 'Gerbers' directory)

| Quantity | Value                    | Package             | Device/Description                                            |
| :---     | :---                     | :---                | :---                                                          |
| 9        | 4.7 kΩ<br>(1% or better) | EXBV8V              | Capacitor, ceramic (THT: 5mm leg spacing, SMT: 0805)          |
| 1        | 10 kΩ                    | R0805               | Capacitor, ceramic (THT: 2,5mm leg spacing, SMT: 0805)        |
| 1        | 100 kΩ                   | R0805               | Electrolytic Capacitor,<br>(THT: 2,5mm leg spacing, ø5x11mm)<br>(SMT: B6 ø5x5,4mm)   |
| 2        | 10 µF                    | UD-5X5,8_NICHICON   | Electrolytic Capacitor,<br>(THT: 2,5mm leg spacing, ø5x11mm)<br>(SMT: B6 ø6,3x5,8mm) |
| 1        | 100 µF                   | UD-6,3X7,7_NICHICON | Resistor, Carbon film<br>(THT: 0,25W 5% tolerance, SMT: 0805) |
| 1        | 100 nF                   | E/7260-38_NP        | Resistor, Carbon film<br>(THT: 0,25W 5% tolerance, SMT: 0805) |
| 1        | 150 nF                   | E/7260-38_NP        | Resistor, Carbon film<br>(THT: 0,25W 5% tolerance, SMT: 0805) |
| 1        | 1N4148                   | SOD323              | Resistor, Carbon film<br>(THT: 0,25W 5% tolerance, SMT: 0805) |
| 1        | 35RASMT2BHNTRX           | 35RASMT2BHNTRX      | Resistor, Metal film<br>(THT: 0,6W 1% tolerance, SMT:0805)<br>(All 0805 is 1% so it doesn't apply here) |
| 2        | 74XX374DW                | SOIC-20W            |  AD7528, TLC7528 or MX7528. 2 Channel Digital to Analog Converters - CMOS 8-Bit Buffered Multiplying DAC. AD7528 (Analog Devices), TLC7528 (Texas Instrument) or MX7528 (Maxim) will also work. Original have AD7528. I have tried with AD and TLC. |
| 1        | LM386M                   | SOIC-08             | Bipolar Transistor. BJT, 30V, 100mA, NPN. (SMT: I have tried with BC848B as well and it works but sounds a bit different. 849 is low noice. Use 849 if you can) |

---

## Enclosure

There is no enclosure at the moment. If anyone makes one, please contact me so I can add it to this repository. There is two hole on the THT pcb as the original. ~~I don't think it~~ It will not fit in the original case. ~~I haven't tested that though~~. The two SMT versions have one hole and two notches on the side of the pcb. So it should be easy to make an enclosure for it. But what do I know, I'm not a 3D designer.

---

## Tips and help

| [Through hole]<br>[THT BOM]      | <img title="Through hole pcb, bottom" style="width:29%" src="Pics/THT_bottom.jpg">  <img title="Through hole pcb, top" style="width:28.4%" src="Pics/THT_top.jpg"> |
| :--- | :---:  |
| [Surface Mount v1]<br>[SMT v1 BOM]  | <img title="SMT v1 pcb, bottom" style="width:26.4%" src="Pics/smt_v1_bottom.jpg">  <img title="SMT v1 pcb, top" style="width:28%" src="Pics/smt_v1_top.jpg"> |
| [Surface Mount v2]<br>[SMT v2 BOM]<br>The RCA jack has a very tight fit. v1 is easier to build. | <img title="SMT v2 pcb, bottom" style="width:26%" src="Pics/smt_v2_bottom.jpg">  <img title="SMT v2 pcb, top" style="width:28.6%" src="Pics/smt_v2_top.jpg"> |
|                   |   |
| SMT: I would suggest to use a file to chamfer the edge of the connector to easier put it in the cartridge port. | <img title="SMT v2 pcb, bottom" style="width:29%" src="Pics/45d_chamfer.jpg"> |
| SMT: Choose one of the diode on the pcb. ${\color{red}Don't \space use \space both!}$ | <img title="SMT v2 pcb, bottom" style="width:29%" src="Pics/diode.jpg"> |
| SMT: The components are crammed together in a grid which corresponds to the silkscreen grid. Otherwise just look at the picture of the board you choose to build. | <img title="SMT v2 pcb, bottom" style="width:29%" src="Pics/placement.jpg"> |
---

The disk that was included in the box can be found at [Atari Mania](https://www.atarimania.com/utility-atari-st-playback_25563.html)<br>
Label for cartridge (size ca: 39,6 mm x 57 mm) is included in the [label](Labels/Sticker%2039,6mmx57mm.jpg) folder. [PDF with multiple labels](Labels/Microdeal%20Stereo%20Playback%20label.pdf) <br>
More photos can be found in the [Pics](Pics/) folder. <br>
Datasheet for some of the components used in the original or the new design can be found in the [Datasheet](Datasheet/) folder. <br>
All three PCB unpopulated: [TOP](Pics/3v_pcb_top.jpg), [BOTTOM](Pics/3v_pcb_bottom.jpg). <br>
[Schematics](Schematics/Microdeal%20Stereo%20Playback_schematics.pdf) and [Manual](Manual/Microdeal%20Stereo%20Playback%20manual.pdf) scanned by me. Also the box and other material included in the box can be found in the [Scanned](Scanned/) folder.

---

## Testing

I used HexTracker v0.849B to test the cartridge. [ScummVM lite](https://www.happydaze.se/scummvm-lite-atari/) (Atari) should also work. There is other trackers that also works. 

---

PCB made by Daniel Guldkrans aka DoG in Eagle November 2025.


[Through hole]: Gerbers/Microdeal_Stereo_Playback_v1.21_THT.zip
[THT BOM]: Gerbers/Microdeal_Stereo_Playback_v1.21_THT_BOM.txt
[Surface Mount v1]: Gerbers/Microdeal_Stereo_Playback_SMT_v1.21_v1.zip
[SMT v1 BOM]: Gerbers/Microdeal_Stereo_Playback_SMT_v1.21_v1_BOM.txt
[Surface Mount v2]: Gerbers/Microdeal_Stereo_Playback_SMT_v1.21_v2.zip
[SMT v2 BOM]: Gerbers/Microdeal_Stereo_Playback_SMT_v1.21_v2_BOM.txt
