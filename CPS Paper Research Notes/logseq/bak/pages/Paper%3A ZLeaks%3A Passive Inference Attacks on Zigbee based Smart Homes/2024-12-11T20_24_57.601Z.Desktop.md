year-published:: #[[Published 2021]] 
paper-type:: 
source:: [ARXIV](https://arxiv.org/abs/2107.10830)

- ![ZLeaks: Passive Inference Attacks on Zigbee based Smart Homes](../assets/ZLeaks_Passive_Inference_Attacks_on_Zigbee_based_Smart_Homes_1733443513652_0.pdf)
- Summary
	- can passively identify devices and events in a Zigbee network by analyzing encrypted traffic
	- Overview
	  collapsed:: true
		- **Device and Event Identification**:
			- ZLeaks can infer functionality-specific application layer (APL) 
			  commands from Zigbee traffic, allowing it to identify unknown events and
			  devices with an accuracy of 83.6% without needing prior device 
			  signatures.
		- **Periodic Reporting Patterns**:
			- The tool also exploits the periodic reporting patterns of devices to 
			  create unique fingerprints, achieving a 99.8% accuracy in identifying 
			  known devices even when no user activity occurs.
		- **Experimental Validation**:
			- The authors evaluated ZLeaks on a diverse set of 19 unique Zigbee devices 
			  across five popular smart hubs in various environments, including a 
			  controlled RF shield and a living smart-home lab. They also validated 
			  their findings using third-party capture files.
	- Adversarial Model
		- **Passive Eavesdropping**:
			- The attacker does not need to be physically present in the network or have 
			  access to the devices. They can simply listen to the wireless 
			  communications to gather information.
		- **Exploitation of Unencrypted Metadata**:
			- The model highlights that even though the payloads of the Zigbee 
			  communications are encrypted, certain unencrypted metadata (such as MAC 
			  OUI, frame lengths, and command types) can be leveraged to infer device 
			  identities and events.
		- **No Prior Knowledge Required**:
			- The adversary does not need prior knowledge of the specific devices or 
			  their event signatures. The inference attacks can be conducted based on 
			  the observed traffic patterns and metadata.
		- **Potential for Information Leakage**:
			- The model suggests that the design of the Zigbee protocol, which 
			  prioritizes low power consumption and efficiency, inadvertently leads to
			  significant information leakage that can be exploited by attackers.
	- Attack information gains
	  collapsed:: true
		- **Device Identification**:
			- The attacker can identify various Zigbee devices in the network, including 
			  their types (e.g., bulbs, outlets, sensors, door locks) and 
			  manufacturers, based on the inferred application layer (APL) commands 
			  and periodic reporting patterns.
		- **Event Detection**:
			- The attack enables the identification of specific events triggered by the devices, 
			  such as turning a light on or off, locking or unlocking a door, or 
			  detecting motion. This is achieved by inferring functionality-specific 
			  APL commands from the traffic.
		- **User  Habits and Routines**:
			- By analyzing the patterns of device usage and the timing of events, the 
			  attacker can infer the daily routines and habits of the occupants. For 
			  example, they could determine when the occupants are home or away based 
			  on the activity of smart devices.
		- **Vulnerability Assessment**:
			- The attacker can assess the security posture of the smart home by 
			  identifying devices that may have unpatched vulnerabilities. This 
			  information could be used to plan further attacks or exploit weaknesses 
			  in the network.
		- **Presence Detection**:
			- The ability to monitor device states (e.g., whether a door is locked or a 
			  light is on) allows the attacker to infer the presence or absence of 
			  individuals in the home, which could be useful for planning a burglary 
			  or other malicious activities.
		- **Device Reporting Patterns**:
			- The attacker can extract periodic reporting signatures from devices, 
			  which can serve as unique fingerprints for identifying devices even when
			  no events are triggered.
	- Countermeasures
	  collapsed:: true
		- **Use of SOC MAC OUI**:
			- The authors suggest using System on Chip (SOC) manufacturer identifiers as the MAC Organizationally Unique Identifier (OUI) instead of the real manufacturer's identity. This 
			  change would help obscure the actual manufacturer of the devices, making it more difficult for attackers to identify specific devices.
		- **Random Payload Padding**:
			- To complicate command inference, the authors recommend implementing random padding in the payloads of Zigbee messages. By adding a small number of random bytes to each payload, even identical APL commands would result in different payload sizes, thereby increasing the entropy and making it harder for attackers to infer information based on packet lengths.
		- **Attribute Pipelining**:
			- The authors propose using attribute pipelining, where multiple attributes are sent in a single packet instead of a series of packets. This approach would help disguise the timing and frequency of events, making it more challenging for attackers to deduce user activities based on traffic patterns.
		- **Decoy Packet Injection**:
			- Another suggested countermeasure involves using mains-powered Zigbee routers or 
			  coordinators to inject decoy packets into the network. This technique would help obfuscate the actual traffic patterns and make it harder for attackers to identify real events.
		- **Periodic Reporting Patterns**:
			- The authors emphasize the need for devices to have unique and less predictable reporting patterns. By varying the reporting intervals and patterns, it would be more difficult for attackers to establish consistent signatures for device behavior.
		- **Design Changes in Zigbee Protocol**:
			- The authors argue that significant design changes in the Zigbee protocol are necessary to 
			  effectively prevent the proposed inference attacks. They highlight the importance of incorporating security as a fundamental design tenet in future smart home technologies, such as the emerging Matter protocol.
- References
	- [[Paper: Peek-a-Boo: Seeing Encrypted Home Activities]]