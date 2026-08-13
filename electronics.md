# Beginner Electronics: A 25-Hour Competence Curriculum

> This curriculum was developed with AI assistance and has not been independently validated.

## Goal

After 25 focused hours, build, measure, explain, and debug simple low-voltage DC circuits from schematics—without copying a breadboard layout.

This is a deliberately edited route through [The Organic Chemistry Tutor](https://www.youtube.com/@TheOrganicChemistryTutor), not a watch-everything playlist. The channel is excellent for circuit concepts and calculations, but watching it linearly would produce more equation-solving than practical electronics.

## Final test

From a blank breadboard and a schematic, build an adjustable 555-based LED metronome powered by batteries.

Pass when you can:

- adjust it across roughly 40–200 flashes per minute;
- predict the effect of changing one resistor or capacitor;
- measure supply voltage and current correctly;
- find one deliberately introduced fault within ten minutes;
- explain the function of every component without notes.

Film a one-minute baseline attempt before hour one, even if it fails. Film the same test after hour 25.

## Safety boundary

- Use batteries only: 4×AA or another regulated supply of 5–9 V.
- Do not work on mains-powered equipment, wall voltage, transformers connected to mains, high-voltage circuits, or charged large capacitors.
- Disconnect power before moving components.
- Verify transistor pinouts and electrolytic-capacitor polarity from their datasheets.
- Never measure current by putting the meter directly across a battery or supply.

## Minimum kit

- full-size breadboard and solid-core jumper wires;
- 4×AA battery holder with switch and batteries;
- digital multimeter with a fused current input;
- resistor assortment including 220 Ω, 330 Ω, 1 kΩ, 4.7 kΩ, 10 kΩ, 100 kΩ, and 1 MΩ;
- LEDs, pushbuttons, one LDR, and 10 kΩ/100 kΩ potentiometers;
- 100 nF, 1 µF, 10 µF, and 100 µF capacitors, with electrolytics rated at least 16 V;
- 1N4148 or 1N4007 diodes, 2N2222A or BC547 transistors, and NE555 DIP-8 timers.

Expected cost: approximately 500–900 SEK if you need everything, including a basic multimeter.

## Working rule

For every 20 minutes of video, spend at least 40 minutes calculating, building, measuring, or debugging. Pause before worked examples and solve them yourself. Keep one page per circuit: schematic, prediction, measurements, fault, correction.

## 1. Orientation and baseline — 1 hour

**Watch**

- [Basic Electronics for Beginners](https://www.youtube.com/watch?v=uXr4lXYjXuU)

**Do**

1. Draw a battery–resistor–LED circuit.
2. For a 6 V supply, a 2 V LED, and a 10 mA target current, calculate the resistor: `R = (6 − 2) / 0.010 = 400 Ω`. Choose the next common value up: 470 Ω.
3. Try to build it without copying a breadboard picture.
4. Record what you did not understand. That is the baseline, not failure.

Complete when the LED lights safely and you can point to the closed current path.

## 2. Voltage, current, resistance, and power — 4 hours

**Watch**

- [Voltage, Current, and Resistance](https://www.youtube.com/watch?v=08YugQce9OA)
- [Ohm's Law](https://www.youtube.com/watch?v=_rSHqvjDksg)
- [Series and Parallel Circuits](https://www.youtube.com/watch?v=7mdc-lRrW1c)
- Optional consolidation: [Electrical Formulas — Basic Electricity for Beginners](https://www.youtube.com/watch?v=Pv_-OU4Dluo)

**Build and calculate**

1. One LED with a current-limiting resistor.
2. Two LEDs in series; decide whether 6 V is sufficient before powering it.
3. Two LEDs in parallel, each with its own resistor.
4. Two resistors in series and then in parallel.

For every circuit, predict total resistance, current, each voltage drop, and resistor power before measuring. Pass when measured values are within 10% of your prediction or you can explain the discrepancy.

## 3. Reading, measuring, and debugging — 5 hours

**Watch**

- [Resistor Color Code Chart Tutorial Review](https://www.youtube.com/watch?v=G1mZutobxDU)
- [Introduction to Multimeters](https://www.youtube.com/watch?v=n9Obx15AjdM)
- [Voltage Divider Circuit Explained](https://www.youtube.com/watch?v=JGXdi7XcQi8)

**Do**

1. Identify ten random resistors by colour, then measure them. Get at least 8/10 correct within tolerance.
2. Build a 10 kΩ/10 kΩ divider. Predict and measure its midpoint voltage.
3. Replace one resistor and calculate the new voltage before measuring.
4. Rebuild three earlier circuits using only your own schematics.
5. Create and diagnose these faults: open connection, reversed LED, wrong resistor decade, and disconnected breadboard rail.

Pass when you can measure voltage in parallel, current in series, resistance with power removed, and diagnose an unknown fault within ten minutes.

## 4. Components that sense, store, and vary — 4 hours

**Watch**

- [Capacitors — Basic Introduction](https://www.youtube.com/watch?v=BimpNou0orc)
- [Potentiometers — Basic Introduction](https://www.youtube.com/watch?v=XuBx9eQYscU)

**Build**

1. Use a potentiometer as a voltage divider; measure its output at five positions.
2. Replace one divider resistor with an LDR; record light and dark resistance and output voltage.
3. Make a slow RC charge/discharge circuit. Predict the time constant `τ = RC`, then observe and measure the voltage change.

Pass when you can explain why a potentiometer has three pins, why an LDR changes divider voltage, and why a capacitor affects change over time rather than simply “storing voltage.”

## 5. Diodes and transistor switching — 5 hours

**Watch**

- [What Is a Diode?](https://www.youtube.com/watch?v=g54vURe47gM)
- [LEDs — Light-Emitting Diodes](https://www.youtube.com/watch?v=Hl4v1aUFWrs)
- [Transistors — NPN and PNP: Basic Introduction](https://www.youtube.com/watch?v=AcxDiesy-nI)
- [BJT Transistors — Electronics Switches and Inverters](https://www.youtube.com/watch?v=VJJuxQk5fTY)
- [DIY Night-Activated LDR Sensor Circuit](https://www.youtube.com/watch?v=X5jm9_nikd8)

**Build**

1. Test a diode and LED in both directions.
2. Use an NPN transistor to switch an LED; calculate both LED and base resistors.
3. Build the night-light circuit from its schematic.
4. Measure the LDR divider voltage and transistor base voltage in light and dark conditions.

Pass when you can explain cutoff, saturation, and how a small base current controls a larger collector current. “The transistor creates current” is not an acceptable explanation.

## 6. Timing and final project — 6 hours

**Watch**

- [555 Timer IC — Low-Frequency Pulse Generator](https://www.youtube.com/watch?v=prszzP43P-c)
- [LED Blinking Circuit Using a 555 Timer](https://www.youtube.com/watch?v=P8o2o7AelGY)

**Do**

1. Build the fixed-rate LED flasher.
2. Change one resistor, then one capacitor; predict whether each change makes it faster or slower before powering it.
3. Replace the timing resistor with a potentiometer and tune the circuit to approximately 40, 80, 120, and 200 flashes per minute.
4. Draw a clean final schematic and rebuild it from a cleared breadboard.
5. Have someone introduce one fault, or introduce one yourself after a break, then diagnose it systematically.
6. Perform and film the final test.

## Ignore for now

Do not let the channel's breadth turn this into another endless syllabus. Skip these until the final test is passed:

- nodal and mesh analysis, Thevenin, Norton, superposition, and maximum-power-transfer problems;
- mains AC, rectifier power supplies, voltage multipliers, boost converters, and every high-voltage project;
- transistor biasing and multistage amplifiers;
- op-amps, RLC networks, impedance, power factor, and advanced oscillators;
- Arduino and microcontrollers. They will make projects easier, but they can hide the electronics you are trying to learn.

## Next competence card

The best next direction is **audio electronics**, not a generic intermediate electronics course:

1. build an LM386 mono amplifier;
2. understand RC high-pass and low-pass filters;
3. build a simple tone control or guitar buffer;
4. then attempt a guitar pedal or small radio receiver.

## Competence card summary

- **Capability:** Build and debug simple low-voltage analog circuits from schematics.
- **Practice budget:** 25 focused hours, probably 4–6 weeks.
- **Evidence:** Notebook calculations, circuit photos, baseline video, and final-test video.
- **Mastery test:** Adjustable 555 LED metronome, rebuilt from a schematic and debugged independently.
- **Maintenance:** Build or repair one small circuit every month.
- **Next card:** Build and characterize a small audio amplifier.

## Source note

The channel's broader indexed electronics collection contains roughly 65 videos and about 29 hours of material, spanning beginner through intermediate topics. This curriculum intentionally selects only the foundation needed for practical low-voltage work; the full sequence is catalogued by [Class Central](https://www.classcentral.com/course/youtube-electronic-circuits-90630).
