# Step 1 - Arduino Basics "Power, Ground & Ohm's Law" (no code yet)

## What I learned
- **Arduino 5V & GND**: 5V is the alimentaion; **GND (0V, mass)** is the return path. A circuit have to go **from 5V → through the load → back to GND**
- **Breadboard rails**: Systematically red = + (5V) and blue/black = - (GND). Power pass all along this board.
- **Resistor basics**: A resistor is an electronic component that **limits current**.
  - Symbol : zig-zag line or rectangle.
  - Unit: Ohm (Ω).
- **Measuring resistance and voltage**:
  - Resistance (R) is measured in **Ohms (Ω)** with an ohmmeter/multimeter.
  - Voltage (U) is measured in **Volts (V)** between two points with a voltmeter/multimeter.
  - Intensity (I) is measured in **Amperes (A)** (often **miliamps (mA)**).
- **Ohm's Law**: \( U = R * I \)
- **LED basics**: LEDs are polarized (power only passes on one side).
  - **Anode (+)** = long leg (represent with an A on the diagram) → goes toward 5V (usually through a resistor).
  - **Cathode (-)** = short leg (represent with a K on the diagram) → goes to GND.
  - The **serie resistor** can be placed on either side of the LED (must be in series) it **limits current** so the LED doesn't burn out.
- **LED forward voltage (Vf)** depends on color (we just saw the red one):

---

## Exercices (Tinkercad simulations)
1. **Lamp test**: Connect one lamp between 5V and GND → it lights up (lamp filament = resistor).
   - Measurement: ~5V across the lamp, current measured in series.
2. **Two lamps in parallel**: Connect +5V to both lamps anodes, GND to both cathodes.
   - Measurement: Each lamp gets ~5V.
   - Current divides between the two branches.
   - Both lamps light with full brightness.
3. **Two lamps in series**: Connect +5V → lamp1 → lamp2 → GND.
   - Measurement: Voltage splits (~2.5V each if lamps are identical).
   - Current is the same through both lamps.
   - Both lamps light, but dimmer (they share the voltage).
4. **LED + resisor**: +5V → resistor (220Ω) → LED → GND.
   - Measurement: LED drop ~2V, resistor drop ~3V, current ~10-15 mA.

---

## Sources
- [Arduino – Premiers pas en informatique embarquée (PDF)](../arduino-premiers-pas-en-informatique-embarquee.pdf)  
- [Arduino YouTube Playlist](https://youtu.be/coASg9W8ufc?si=UJOpBKLUhe1zS9gJ)  
