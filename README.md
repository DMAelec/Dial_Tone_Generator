# DIAL TONE GENERATOR

 This circuit provides a 1 volt peak-to-peak dial tone signal with equal proportions of 350Hz and 440Hz sine waves. The two frequencies are generated in multivibrator sections U1A and U1B. Triangle-like waveforms from the multivibrator sections are fed to summing amplifier U1D. A 470pF capacitor in the feedback path of U1D removes some of the unwanted harmonics from the composite waveform, which is then fed to section U1C, a Sallen-Key low-pass filter. U1C further reduces the harmonics, providing a high-quality summed-sine signal at its output. The two frequencies are close enough to permit a single-filter design, with the summing resistors at U1D's input selected to emphasize the 440Hz component, accordingly.

Calibration is performed by connecting a frequency counter to the "350 TP" and "440 TP" test points, and adjusting the respective trimmer potentiometers to obtain the correct frequencies. The frequencies are relatively independent of power supply voltage, and the single +7.5v power supply may be derived from a simple regulator circuit. The circuit consumes less than 3 milliamperes of current.

For convenience and economy, the circuit was designed with one CMOS quad op-amp integrated circuit.

BASED ON SCHEMATIC FROM:
https://www.theremin.us/Circuit_Library/dial_tone_generator.html