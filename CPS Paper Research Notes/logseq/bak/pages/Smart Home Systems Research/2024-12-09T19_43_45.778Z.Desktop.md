- [[Actuators]]
- [[Sensors]]
- [[Communication Protocols]]
- ![Smart Home Privacy Protection Methods against A passive Wireless Snooping Side-Cannel Attack](../assets/sensors-22-08564-v3_1732641062625_0.pdf) #[[Published 2022]] #[[Review Paper]]
	- [Source](https://www.mdpi.com/1424-8220/22/21/8564)
- ![Light Ears: Information Leakage via Smart Lights](../assets/3351256_1732641926328_0.pdf) #[[Published 2019]] #Actuators
  id:: 674750d7-20fb-464d-be43-2a16b9f43eb7
  collapsed:: true
	- [Source](https://dl.acm.org/doi/abs/10.1145/3351256)
	- 3 attacks listed in paper
		- 1st two infer users' audio/video playback using systematic observation and analysis of the multimedia-visualization functionality of smart light bulbs
		- 3rd attack uses the infrared capabilities of smart light bulbs to create a covert-channel to ex-filtrate user's private data out of secured home or office network.
- ![Security Concerns in IoT Light Bulbs: Investigating Covert Channels](../assets/2408.14613v1_1732656803976_0.pdf) #[[Unpublished]] #[[Review Paper]]
	- [Source](https://arxiv.org/abs/2408.14613)
- ![Wireless Traffic Analysis Based SCA and CM in Smart Home](../assets/3603165.3607446_1732657076087_0.pdf) #[[Published 2023]] #[[Communication Protocols]]
	- [Source](https://dl.acm.org/doi/abs/10.1145/3603165.3607446)
	- It's a one page poster, can't use it : (
- ![Signal Emulation Attack and Defense for Smart Home IoT](../assets/Signal_Emulation_Attack_and_Defense_for_Smart_Home_IoT_1732676954203_0.pdf) #[[Published 2022]]
	- [Source](https://ieeexplore.ieee.org/abstract/document/9763029)
	- This is an EM injection attack, out of scope for the research : (
- Many articles are referencing [[ZigBee]] signals and packets should research this
- ![WazaBee attacking Zigbee networks by diverting Bluetooth Low Energy chips](../assets/WazaBee_attacking_Zigbee_networks_by_diverting_Bluetooth_Low_Energy_chips_1732678115910_0.pdf) #[[Published 2021]] #[[Communication Protocols]]
	- [Source](https://ieeexplore.ieee.org/abstract/document/9505165)
	- This is another injection attack
- ![Smart Home Systems Overview and Comparative Analysis](../assets/Smart_Home_Systems_Overview_and_Comparative_Analysis_1732736637149_0.pdf) #[[Published 2018]] #[[Review Paper]]
	- [Source](https://ieeexplore.ieee.org/abstract/document/8718722)
- ![Don’t Kick Over the Beehive: Attacks and Security Analysis on Zigbee](../assets/3548606.3560703_1732737205683_0.pdf) #[[Published 2022]] #[[Communication Protocols]]
	- [Source](https://dl.acm.org/doi/abs/10.1145/3548606.3560703)
	- This is likely an injection attack and not a side channel attack
- ![Side channel attacks on smart home systems A short overview](../assets/Side_channel_attacks_on_smart_home_systems_A_short_overview_1732737614044_0.pdf) #[[Published 2017]] #[[Conference Paper]]
  collapsed:: true
	- [Source](https://ieeexplore.ieee.org/abstract/document/8217429)
	- Lists Side Channel Attack Categories
	- Data Privacy Protection in two Major categories:
		- Protecting Sensitive and private content of messages transmitted through the home network.
		- Concerns about the context of data, such as:
			- identities of communicators
			- temporal data
			- absolute/relative locations of targeted smart devices
	- This paper about SCAs that attack the contextual data (the second category)
	- C. Electromagnetic Analysis:
		- > Cryptographic devices performing encryption or decryption tasks emit power radiation of electromagnetic fields. In this type of attack, adversaries exploit leaked radiation for performing electromagnetic analysis to find correlations between leaked radiation and ciphertext. Since this radiation can be captured remotely, depending on the receiver equipment strength, this side-channel attack can be performed from a distance and hackers do not need to be close to the target [20].
			- The reference:
				- J. Longo, E. De Mulder, D. Page, and M. Tunstall, "SoC it to EM: electromagnetic side-channel attacks on a complex system-onchip," in International Workshop on Cryptographic Hardware and Embedded Systems, 2015, pp. 620-640.
	- ![image.png](../assets/image_1732845025260_0.png)
	-
	-
	-
- ![Everything has its Bad Side and Good Side: Turning Processors to Low Overhead Radios Using Side-Channels](../assets/3583120.3586959_1733193845587_0.pdf) #[[Published 2023]]
	- [Source](https://dl.acm.org/doi/abs/10.1145/3583120.3586959)
	- Not a security paper, it might have usable references though.
- ![Detecting the Presence of Electronic Devices in Smart Homes Using Harmonic Radar Technology](../assets/remotesensing-14-00327-v2_1733255571344_0.pdf) #[[Published 2022]]
	- [Source](https://www.mdpi.com/2072-4292/14/2/327)
- ![Enhanced Indoor Multi-Target Counting Based on Micro-Doppler Features with 24GHz Radar](../assets/Enhanced_Indoor_Multi-Target_Counting_Based_on_Micro-Doppler_Features_with_24GHz_Radar_1733260929097_0.pdf) #[[Published 2024]] #[[Conference Paper]]
	- [Source](https://ieeexplore.ieee.org/abstract/document/10642879)
	- This is not really a security paper, it doesn't talk about any vulnerabilities
- ![HOMESPY:  the invisible sniffer of infrared remote control of smart TVs](../assets/usenixsecurity23-huang_1733346018950_0.pdf) #[[Published 2023]]
  id:: 6750e67e-88e2-4331-85a8-83c93fe4e11c
  collapsed:: true
	- [Source](https://dl.acm.org/doi/10.5555/3620237.3620492)
- ![Precise Wireless Camera Localization Leveraging Traffic-Aided Spatial Analysis](../assets/Precise_Wireless_Camera_Localization_Leveraging_Traffic-Aided_Spatial_Analysis_1733348492205_0.pdf) #[[Published 2023]]
  id:: 6750e67e-5a64-4a74-bb43-c5f24612e24c
  collapsed:: true
	- [Source](https://ieeexplore.ieee.org/document/10319073)
- ![Eavesdropping Vulnerability and Countermeasure in Infrared Communication for IoT Devices](../assets/sensors-21-08207-v3_1733433304706_0.pdf) #[[Published 2021]]
	- [Source](https://www.mdpi.com/1424-8220/21/24/8207)
	- Simply states that IR channels for communication on devices should be encrypted, which they are not in a lot of cases
- [[SmartCfg]] seems to be another channel for which devices are connecting to smart home networks
- ![Passwords in the Air:  Harvesting Wi-Fi Credentials from SmartCfg Provisioning](../assets/3212480.3212496_1733434179136_0.pdf) #[[Published 2018]]
	- [Source](https://dl.acm.org/doi/10.1145/3212480.3212496)
	- Can't use this source because it's too old but it might have more recent papers that reference this paper.
	- Paper not really useful : (
- ![Et Tu Alexa? When Commodity WiFi Devices Turn into Adversarial Motion Sensors](../assets/et_tu_alexa_1733436109637_0.pdf) #[[Published 2020]]
  id:: 675222c5-5e85-447c-aa6f-493760c98559
	- [Source](https://arxiv.org/abs/1810.10109)
- ![IoTBeholder: A Privacy Snooping Attack on User Habitual Behaviors from Smart Home Wi-Fi Traffic](../assets/3580890_1733441097591_0.pdf) #[[Published 2023]]
  id:: 6752233a-d78f-4343-b732-56bf2d46faa1
  collapsed:: true
	- [Source](https://dl.acm.org/doi/abs/10.1145/3580890)
- ![WiFiLeaks: Exposing Stationary Human Presence Through a Wall With Commodity Mobile Devices](../assets/WiFiLeaks_Exposing_Stationary_Human_Presence_Through_a_Wall_With_Commodity_Mobile_Devices_1733441419056_0.pdf) #[[Published 2023]]
	- [Source](https://ieeexplore.ieee.org/abstract/document/10301514)
- ![Peek-a-Boo: I see your smart home activities, even encrypted](../assets/Peek-a-Boo_I_see_your_smart_home_activities_even_encrypted_1733442033064_0.pdf) #[[Published 2020]]
  id:: 675237cc-9803-4090-9ceb-375e1c1c6c49
  collapsed:: true
	- [Source](https://dl.acm.org/doi/10.1145/3395351.3399421)
- ![Intercepting Bluetooth Traffic from Wearable Health Devices](../assets/Intercepting_Bluetooth_Traffic_from_Wearable_Health_Devices_1733442577154_0.pdf) #[[Published 2024]]
	- [Source](https://ieeexplore.ieee.org/document/10579530)
- ![ZLeaks: Passive Inference Attacks on Zigbee based Smart Homes](../assets/ZLeaks_Passive_Inference_Attacks_on_Zigbee_based_Smart_Homes_1733443513652_0.pdf) #[[Published 2021]]
  id:: 67523c2f-21d2-4137-8346-290e872c6bb6
  collapsed:: true
	- [Source](https://arxiv.org/abs/2107.10830)
- ![BehavIoT: Measuring Smart Home IoT Behavior Using Network-Inferred Behavior Models](../assets/BehavIoT_Measuring_Smart_Home_IoT_Behavior_Using_Network-Inferred_Behavior_Models_1733443556835_0.pdf) #[[Published 2023]]
	- [Source](https://dl.acm.org/doi/10.1145/3618257.3624829)
	- References:
		- ((6752233a-d78f-4343-b732-56bf2d46faa1))
		- ((67523c2f-21d2-4137-8346-290e872c6bb6))
	- Not usable as a source but interesting how it builds off the previous studies
- ![FindSpy: A Wireless Camera Detection System Based on Pre-Trained Transformers](../assets/FindSpy_A_Wireless_Camera_Detection_System_Based_on_Pre-Trained_Transformers_1733447753848_0.pdf) #[[Published 2023]]
	- [Source](https://ieeexplore.ieee.org/document/10218088)
	- References:
		- ((675237cc-9803-4090-9ceb-375e1c1c6c49))
- ![DeepDeSpy: A Deep Learning-Based Wireless Spy Camera Detection System](../assets/DeepDeSpy_A_Deep_Learning-Based_Wireless_Spy_Camera_Detection_System_1733447797731_0.pdf) #[[Published 2021]]
	- [Source](https://ieeexplore.ieee.org/document/9582812)
	- References:
		- ((675237cc-9803-4090-9ceb-375e1c1c6c49))
- ![Extended Functionality Attacks on IoT Devices: The Case of Smart Lights](../assets/Extended_Functionality_Attacks_on_IoT_Devices_The_Case_of_Smart_Lights_1733448079900_0.pdf) #[[Published 2016]]
	- [Source](https://ieeexplore.ieee.org/document/7467343)
	- Use as a foundational to find more on smart lights
- ![IoTAthena Unveiling IoT Device Activities From Network Traffic](../assets/IoTAthena_Unveiling_IoT_Device_Activities_From_Network_Traffic_1733448411766_0.pdf) #[[Published 2021]]
  id:: 67525211-cdbf-42dc-b162-804cb0746022
	- [Source](https://ieeexplore.ieee.org/document/9504600)
- [Smart Tracer Source](https://ieeexplore.ieee.org/document/10229163) relates to the Case of Smart Lights
-