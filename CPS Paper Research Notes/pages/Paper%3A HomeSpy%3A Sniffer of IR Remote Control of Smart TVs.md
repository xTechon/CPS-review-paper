year-published:: #[[Published 2023]] 
paper-type:: 
source:: [ACM](https://dl.acm.org/doi/10.5555/3620237.3620492)

- ![HOMESPY:  the invisible sniffer of infrared remote control of smart TVs](../assets/usenixsecurity23-huang_1733346018950_0.pdf)
- Summary:
	- Paper Aims:
		- Is it possible for an IoT device to sniff smart TV IR remote control signals, even when it is not on the path between TV and controller?
		- If the IR signals can be sniffed, what can an attacker learn from the signal?
	- IR does not need line of sight anymore to gather information
	- "For example,(1) the attacker could know when the light or air-conditioner is turned on/off to __infer the victim’s daily routine__"
	- Threat Model:
		- **Availability of an IoT Device with IR Receiver**
			- In other words, the attacker can control an device with IR capabilities
		- **Attack Device Needs to be Powered On**
		- **Placement of the Attack Device**
			- Assumes attack device is close to victim device
	- What can the attack do?
		- Record IR signals not directly aimed at the attack device
		- Decode commands from captured IR signals
			- Achieved using a DB of IR codes from various devices
		- Infer credentials (as a keylogger essentially)
		- __Infer User Activities__
	- Evaluation
		- The current (in 2023) has no security measures (like encryption) due to the assumption of LOS comms (see References)
		- Encryption  difficult to implement
			- hard to share secrets without it being too short or needing extra hardware
		- Interference to IR comms
			- Light sources can interfere
		- Difficult to find alternatives to in-home TV control
- References:
	- [[Paper: Eavesdropping Vulnerability and Countermeasures in IR Comms for IoT Dev]]