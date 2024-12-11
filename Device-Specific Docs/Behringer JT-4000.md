# Behringer JT-4000

The Behringer JT-4000 is a $50 Impulse buy Roland JP-8000-like based on the STM32 microcontroller and a pair of LM13700s

You know and love the JP-8k from Sandstorm and other earworm hooks from 90's trance.

It do saws, it do saws super, it do super saws super cheap.

## Mod Shortlist

Quick rundown of what may be possible to tinker with of reasonable value

### External Keybed

Key press/release data is communicated to microcontroller via I2C

Must run LA on bus (having a functonal LA like https://www.sparkfun.com/products/18627 will help) to determine how best to hijack the bus

_may_ be possible to exceed limitations of physical bed depending on software

- Improved or unnatural response [high chance, low value]
- Extended range/voice [mixed chance, mixed value - why not use midi?]

### VC Filter Controls

Filter Cutoff and Res can be replaced with vactrols

### Menu macroing

Hijacking the encoder and buttons would allow for triggering preset changes or even setting parameters through triggers

This would rely on a steady state

## Disassembly Notes

Disassembly is reasonably straightforward and non-destructive

- Four screws at the bottom hold the faceplate in
- Two screws hold the PCB to the case
- PCB is also glued down to the case under the keybed, heat is not required for removal, a guitar pick or spludger can be used to pry the edges from from the case
- Grey plastic above PCB is mostly decorative and any bending on the edges caused by prying are cosmetic

## Controls

1x Rotary Encoder w/ Switch (menuing)
3x Pots [VALUES TBD]
6x Tac switches (total of 7 control buttons)

### Keybed

Controlled by Vintek IC (see below)

Capacitive keybed is 16 pins on the bottom triggering low, keys send I2C data to STM32

## Internal Markings

Rear: musictribe - 0722ABR

## Notable ICs

STM32 Based
Holtek HT16K33 - LED Controller
U9/U10 - V13700M (x2) - Specific implementation TBD

- Likely one for OSC and one for Filter

U5 - Vintek VK36N16I - Touchpad Controller
- Vintek IC converts touch to I2C.
- Exact datasheet not found, 9 channel datasheet: https://www.szvinka.com/uploadfile/Datasheet/Touch/VK36N/VK36N9I/VK36N9I_V1.1-EN.pdf
- Each pad should be behind a ~1k Resistor
- SCL / SCA should be pins 16/17 respectively
- VDD should be 18
- INT should be 19
- SCL, SCA, and INT should be tied VDD (19?) through 10K
- Addr 0xA1?

## Internal Connectors

X4 - Appears to sit between Encoder/Buttons and STM

Back of Keybed - point per key running back to Vintek IC

## Test Points

TP1
TP2
TP3 - Top right of STM
TP4 - Top left of Holtek
TP5 - Top left of STM
TP6 - Right of Holtek
TP7 - Below LCD FFC
TP8
TP9
TP10 - Below Second Button
