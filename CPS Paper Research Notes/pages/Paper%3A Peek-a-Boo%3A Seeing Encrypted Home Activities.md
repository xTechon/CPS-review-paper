year-published:: #[[Published 2020]] 
paper-type:: 
source:: [ACM](https://dl.acm.org/doi/10.1145/3395351.3399421)

- ![Peek-a-Boo: I see your smart home activities, even encrypted](../assets/Peek-a-Boo_I_see_your_smart_home_activities_even_encrypted_1733442033064_0.pdf) #[[Published 2020]]
- Summary
  collapsed:: true
	- 4 stages to attack:
		- Device Identification
		- Device State Detection
		- Device State Classification
		- User Activity Inference
	- Main Defense
		- Spoof traffic in the network to obscure the real states of devices and activities
	- Adversarial Model
		- attacker can install sniffers within vicinity of smart network
		- attacker does not need to interfere with network traffic
		- the attacker can capture/analyze wireless traffic from various protocols
		- The attacker has access to the same types of smart home devices as the targeted user, which allows the attacker to analyze traffic from the devices and train algorithms for device identification and activity inference.
		- Attacker can access protocol headers which are not protected by encryption
		- No need for exact device models
			- Must have knowledge of brand and device type
- References
	- [[Paper: Et Tu Alexa? Commodity WiFi Devices as Adversarial Motion Sensors]]