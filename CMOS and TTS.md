Created: `17-Sep-2024`, `10:26`
Tags: [[SC1005]]

# CMOS (complementary metal oxide semiconductor)
- unipolar field-effect transistors
- Gate, drain source
- with correct voltage at G, current can flow between S and D
- HC series pin compatible with TTL, same pin layout
- HCT series electrically compatible with TTL
- e.g.
	- old: 40/140
	- metal gate: 74C
	- high speed: 74HC
	- elec comp with TTL: 74HCT

# TTL (transistor transistor logic)
- bipolar junction transistors
- has a base, emitter and collector
- with correct voltage at B, current can flow between c and e
- B is the switch to control
- dont differ in pin layout or logic with different prefixes
- e.g.
	- hex inverters
		- standard: 74
		- high speed: 74H
		- low power: 74L

# Voltage ranges
TTL
- 5v
CMOS
- V_DD ranges from
- 3v-18v
	- 5v is used when in the same circuit as TTL ICs
Some CMOS devices arent compatible with TTL, because the indeterminate range for CMOS device is 1.5-3.5v, while TTL's indeterminate range is 0.8-2v. Therefore, if the voltage for TTL cna be 1 or 0 but indeterminate in the CMOS IC

# Unconnected (floating) input
TTL
- floating input is logic 1
- between 1.4-1.8v
- not recommended due to noise pickup
CMOS
- disastrous result
- IC may become overheated
- all unused input must be connected to $V_{DD}$, GND or another input