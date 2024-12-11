year-published:: #[[Published 2023]] 
paper-type:: 
source:: [ACM](https://dl.acm.org/doi/abs/10.1145/3580890)

- ![IoTBeholder: A Privacy Snooping Attack on User Habitual Behaviors from Smart Home Wi-Fi Traffic](../assets/3580890_1733441097591_0.pdf)
id:: 6752233a-d78f-4343-b732-56bf2d46faa1
- Summary
	- Estimates location of device inside a user's home (device localization)
	- **Wi-Fi Based Device Localization**:
		- This module estimates the coarse location of devices within a user's 
		  home by analyzing Wi-Fi signals and extracting MAC addresses.
	- **Device Classification Module**:
		- A machine learning model processes raw Wi-Fi packets to classify devices accurately, even in unreliable network conditions.
	- **Device Activity Identification Module**:
		- This module identifies the activities of devices using a combination of
		  machine learning and logical corrections to improve accuracy.
	- **Habitual Behavior and Automation Rules Mining Module**:
		- It mines user habitual behaviors and automation rules from the 
		  identified device activities using sequential pattern mining and 
		  hierarchical clustering techniques.
	- **User  Action Prediction Module**:
		- This module predicts future user actions based on the mined habitual behaviors, utilizing deep learning methods.
	- Adversarial model
		- User and Attacker model
		- User
			- Users live in a smart home environment with various IoT devices that
			  they can operate physically or through mobile apps and automation 
			  platforms.
			- Users can secure their Wi-Fi networks in various ways, such as 
			  setting access keys and encrypting traffic (e.g., using WPA2/WPA3).
			- Users cannot alter the fundamental functions of their devices, such 
			  as modifying firmware or changing wireless transmission methods.
		- Attacker
			- The attacker has limited access to the physical environment, meaning
			  they can walk around the user's residence or deploy commercial 
			  off-the-shelf (COTS) equipment for packet sniffing without being 
			  discovered.
			- The attacker does not have prior knowledge of the devices in the 
			  user's home, including their types, locations, or how many devices are 
			  deployed.
			- The attacker cannot gain access to the local area network (LAN) of 
			  the user's home, meaning they cannot join the network without the access
			  key.
			- The attacker can use a device in promiscuous mode to sniff encrypted
			  Wi-Fi packets over the air, but they cannot access information at the 
			  IP layer and above.
	- Countermeasures
		- Spoof packets over the network to obfuscate behavior
		- Have access points inject traffic using spoofed MAC addresses to create noise over the network
		- The countermeasures may impact device performance
- References:
  collapsed:: true
	- [[Paper: Peek-a-Boo: Seeing Encrypted Home Activities]]
	- [[Paper: Et Tu Alexa? Commodity WiFi Devices as Adversarial Motion Sensors]]
- Citations: