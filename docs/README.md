# Wokwi sn5454 Chip

This is a custom chip for [Wokwi](https://wokwi.com/). It implements the sn5454 IC.

## Description

The sn5454 contains 4-wide AND-OR-INVERT. They perform the Boolean function
of Y = NOT( (A . B) + (C . D) + (E . F) + (G . H) ) .

## Pin names

| Name | Description       |
| ---- | ----------------- |
|  A   | Input signal  A   |
|  B   | Input signal  B   |
|  C   | Input signal  C   |
|  D   | Input signal  D   |
|  E   | Input signal  E   |
|  F   | Input signal  F   |
|  G   | Input signal  G   |
|  H   | Input signal  H   |
|  Y   | Output signal     |
| GND  | Ground            |
| VCC  | Supply voltage    |


## Usage

To use this chip in your project, include it as a dependency in your `diagram.json` file:

```json
  "dependencies": {
    "chip-sn5454": "github:wokwi-custom-chips/sn5454@0.1.0"
  }
```

Then, add the chip to your circuit by adding a `chip-sn5454` item to the `parts` section of diagram.json:

```json
  "parts": {
    ...,
    { "type": "chip-sn5454", "id": "chip1" }
  },
```

For a complete example, see [The sn5454 chip test project](https://wokwi.com/projects/399264986831740929).
