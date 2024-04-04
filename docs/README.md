# Wokwi Inverter Chip Example

This is a basic custom chip for [Wokwi](https://wokwi.com/). It implements a simple inverter: the output is always opposite to the input.

## Pin names

| Name | Description              |
| ---- | ------------------------ |
| IN   | Input signal             |
| OUT  | Output (inverted) signal |
| GND  | Ground                   |
| VCC  | Supply voltage           |

## Usage

To use this chip in your project, include it as a dependency in your `diagram.json` file:

```json
  "dependencies": {
    "chip-inverter": "github:devilxnux/at24cxx-chip@1.0.0"
  }
```

Then, add the chip to your circuit by adding a `at24cxx-inverter` item to the `parts` section of diagram.json:

```json
  "parts": {
    ...,
    { "type": "at24cxx-inverter", "id": "chip1" }
  },
```

For a complete example, see [the inverter chip test project](https://wokwi.com/projects/350946636543820370).
