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

| Quantity | Parts    | Value                    | Package             | Device/Description                                |
| :---     | :---     | :---                     | :---                | :---                                              |
| 9        | RN1-RN9  | 4.7 kΩ<br>(1% or better) | EXBV8V              | Array Chip Resistor. Use 1% or better if you can  |
| 1        | R1       | 10 kΩ                    | R0805               | Resistor, Carbon film                             |
| 1        | R2       | 100 kΩ                   | R0805               | Resistor, Carbon film                             |
| 2        | C1, C2   | 10 µF                    | UD-5X5,8_NICHICON   | Electrolytic Capacitor                            |
| 1        | C3       | 100 µF                   | UD-6,3X7,7_NICHICON | Electrolytic Capacitor                            |
| 1        | C4       | 33 nF                    | E/7260-38_NP        | Film Capacitor, Polyphenylene Sulfide (PPS), Metallized - Stacked               |
| 1        | C5       | 150 nF                   | E/7260-38_NP        | Film Capacitor, Polyester, Polyethylene Naphthalate (PEN), Metallized - Stacked |
| 1        | D1       | 1N4148                   | SOD323              | Schottky barrier diode                            |
| 1        | J1       | 35RASMT2BHNTRX           | 35RASMT2BHNTRX      | 3.5mm phone jack, surface mount                   |
| 2        | IC1, IC2 | 74XX374DW                | SOIC-20W            | Octal D type transparent LATCH, edge triggered. HCT, LS |
| 1        | IC3      | LM386M                   | SOIC-08             | Low Voltage Audio Power Amplifier. I used LM386MX |

---

## Enclosure

There is no enclosure for this. If anyone makes one, please contact me so I can add it. 

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
