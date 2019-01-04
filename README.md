# CircuitPython2019
A 2019 Wish List for CircuitPython

When given the opportunity to think about how I’d like to see CircuitPython grow in 2019, I focused on my past projects that are anxiously waiting for conversion to CircuitPython and future projects planned for this year. Seven topical areas emerged from that thought process. What I’ve included here is a bulletized shopping list of ideas and features that would help my projects and improve my coding skills.

Please let me know if any of these need further clarification.

Caveat: I’m a CircuitPython beginner so it’s possible that some of these needs/wants/ideas have already been implemented or are in the works. If that’s the case, please be gentle and help me learn. Thanks.

### Terminal Emulation for Attached Displays

+ Adopt a text-only standard such as ANSI 3.64 (VT100 ANSI escape sequences) for cursor positioning and character attribute control to allow display formatting from text streams and files

### Glowy Things (LEDs)

+ Combine DotStar and Neopixel libraries into a single _StripKit_ library with unified API
+ To increase NeoPixel update speed, create an option to set NeoPixel brightness with a pseudo brightness factor value that scales the tuple's RGB value, contained in the tuple like the DotStar API
+ Provide optional HSV and/or color wheel color selection in addition to RGB within the library
+ Update library to predict and control maximum power draw for specialized boards such as the NeoTrellis M4
+ Create a similar color and brightness control library for traditional 3-pin RGB LEDs and single-color LEDs
  
### Audio

+ Automatically detect and convert incoming high-resolution wave files and streams to the optimum format of the target hardware device or provide a library of CircuitPython-based conversion helpers
+	Provide a port of the _PJRC Audio Library_ and _Audio System Design Tool_ to CircuitPython, starting with some essential functions such as FFT
  
### Radios

+	Extend existing libraries to include standard AT-like command control for RFMxx and future radio co-processor boards
+	Provide CircuitPython support for Software Defined Radio (SDR) primarily for control, tuning, and audio input/output processing
  
### ADC/DAC/Sensor Values

+	Provide capability to simultaneously support raw, normalized, and 16-bit values for ADC, DAC, and sensor values such as those currently provided in the MCP4725 DAC’s CircuitPython library
  
### I2C Extended Addressing

+	Extend I2C _busio_ to transparently support extended bus addressing provided by multiplexers such as the TCA9548A

### Actively Influence Hardware Redesign

+	First order: Code-initiated device reset/initialization during instantiation or optionally when an error is detected (such as for the SSD1306 display breakout and VL53L0X ToF sensor)
+	Second order (long term): Self-check/diagnostics, either when instantiated, in a diagnostic library, or in a collection of diagnostic examples
+	Third order (much, much longer term): Device/module/sensor autonomy via automatic self-checks

