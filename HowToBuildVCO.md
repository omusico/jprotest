# How to build a VCO circuit #

It's amazingly simple to build a VCO.  There is a VCO integrated circuit!  Its part number is  <a href='http://www.newark.com/texas-instruments/cd4046be/phase-lock-loop-pll-logic-ic/dp/06F2487'>CD4046BC<br>
</a> , available at Newark for only $0.54!  Here's the additional circuitry needed to "tune" or implement this IC, as described in the <a href='http://www.falkowski.net/images/CD4046BC.pdf'>datasheet</a>:
```
The linear voltage-controlled oscillator (VCO) produces an
output signal (VCO Out) whose frequency is determined by
the voltage at the VCOIN input, and the capacitor and resistors
connected to pin C1A, C1B, R1 and R2.
```

<img src='http://www.falkowski.net/images/circuit-vco-4046.jpg'>