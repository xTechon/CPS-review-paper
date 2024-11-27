title:: Mobile device Side Channel Attacks

- ![Classification of Side Channel Attacks on Mobile Devices](../assets/Systematic_Classification_of_Side-Channel_Attacks_A_Case_Study_for_Mobile_Devices_1732505080640_0.pdf) #[[Published 2017]] #[[Review Paper]]
	- [Source](https://ieeexplore.ieee.org/abstract/document/8141883)
	- Lists out side channel attacks on mobile devices
	- Q: Summarize the classification system that is proposed in the PDF that I have attached here
	  collapsed:: true
		- The proposed classification system for side-channel attacks in the PDF 
		  categorizes attacks based on two main axes: the type of information 
		  exploited (WHAT) and the method of information acquisition (HOW).
		- **Type of Information (WHAT)**: 
		  This axis distinguishes between physical properties (e.g., power 
		  consumption, electromagnetic emissions) and logical properties (e.g., 
		  software features, memory usage) that can be exploited by attackers.
		- **Method of Information Acquisition (HOW)**:
		  This axis differentiates between active and passive attacks. Active 
		  attacks involve the attacker influencing the behavior of the target 
		  device, while passive attacks involve merely observing the information 
		  leakage without influencing the device.
		- The classification system accommodates various
		  attack scenarios, including those that can be executed remotely or 
		  require physical access to the device. It identifies the evolution of 
		  side-channel attacks from traditional methods requiring physical 
		  presence to modern attacks that can be launched through seemingly 
		  innocuous applications or websites.
		- Additionally, the system highlights the key 
		  enablers that facilitate these attacks on mobile devices, such as their 
		  always-on nature, the ease of software installation, and the multitude 
		  of sensors integrated into smartphones. The classification aims to 
		  provide a systematic framework for analyzing existing side-channel 
		  attacks and developing effective countermeasures.
	- Q: Can you list the attack scenarios from the paper that require physical access to the device
	  collapsed:: true
		- The paper outlines several attack scenarios that require physical access to
		   the device, categorized as local side-channel attacks. Here are the key
		   attack scenarios mentioned:
		- **Power Analysis Attacks**: These
		  attacks exploit the power consumption of a device to infer sensitive 
		  information, such as cryptographic keys. This typically requires 
		  physical access to the device to measure power traces.
		- **Electromagnetic Analysis Attacks**:
		  These attacks leverage electromagnetic emanations from the device to 
		  extract sensitive information. Access to the device is necessary to 
		  capture these emissions.
		- **Smudge Attacks**: These attacks
		  involve analyzing smudges or fingerprints left on a touchscreen to 
		  infer user input or unlock patterns. Physical access is needed to 
		  examine the screen directly.
		- **Shoulder Surfing and Reflections**:
		  This involves visually observing a user’s input on the touchscreen, 
		  either directly or through reflections. The attacker must be in 
		  proximity to the device to perform this attack.
		- **Hand/Device Movements**: 
		  Monitoring the physical movements of the device or the user’s hands 
		  while interacting with the device can infer input. This requires the 
		  attacker to be nearby to observe these movements.
		- **Active Fault Injection Attacks**:
		  These attacks manipulate the device's environment (e.g., by using 
		  voltage or clock glitches) to induce faults in the operation of the 
		  device. Physical access is necessary to implement such manipulations.
	- Q: May you list all the references from the paper that relates to the Electromagnetic Analysis Attacks
	  collapsed:: true
		- The paper references several works related to 
		  Electromagnetic Analysis Attacks. Here are the references mentioned in 
		  the context of these attacks:
		- **Schulz et al. [99]** - This work exploited electromagnetic emanation of Ethernet cables to observe parts of the transmitted Ethernet frames.
		- **He et al. [81]** - This study discusses network traffic analysis, which can include electromagnetic analysis in its broader context.
		- **Bojinov et al. [129]** - This work explores mobile device identification via sensor fingerprinting, which can relate to electromagnetic properties.
		- **Michalevsky et al. [137]** - This research involves recognizing speech from gyroscope signals, which may touch upon electromagnetic analysis indirectly.
		- **Gruss et al. [24]** - This paper discusses the implications of electromagnetic analysis in the context of microarchitectural attacks.
	- Conclusion: This source is not very helpful : (
- ![Side-channel_attacks_on_mobile_and_wearable_systems.pdf](../assets/Side-channel_attacks_on_mobile_and_wearable_systems_1732657718701_0.pdf) #[[Published 2016]] #[[Conference Paper]]
	- [Source](https://ieeexplore.ieee.org/abstract/document/7444764)
-
-