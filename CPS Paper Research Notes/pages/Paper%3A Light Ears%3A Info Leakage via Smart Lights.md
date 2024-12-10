year-published:: #[[Published 2019]] 
paper-type:: 
source:: [ACM](https://dl.acm.org/doi/abs/10.1145/3351256)
doi:: [doi](https://doi.org/10.1145/3351256)

- ![Light Ears: Information Leakage via Smart Lights](../assets/3351256_1732641926328_0.pdf)
- Summary
	- 3 attacks listed in paper
		- 1st two infer users' audio/video playback using systematic observation and analysis of the multimedia-visualization functionality of smart light bulbs
		- 3rd attack uses the infrared capabilities of smart light bulbs to create a covert-channel to ex-filtrate user's private data out of secured home or office network.
	- Some Smart lights have Multimedia Visualization
		- Change the brightness of the light with the audio
	- Can use luminescence sensor to capture the changes in brightness
	- Threat Model
		- Passive Adversary
		- Goal is to infer the media consumption of target user
		- Requires light and color sensors
		- Malicious software used within network cannot communicate directly with an adversarial server over Internet, or that user's network is air gapped.