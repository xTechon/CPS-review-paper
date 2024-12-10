year-published:: #[[Published 2019]] 
paper-type:: 
source:: [ACM](https://dl.acm.org/doi/abs/10.1145/3351256)
doi:: [doi](https://doi.org/10.1145/3351256)

- ![Light Ears: Information Leakage via Smart Lights](../assets/3351256_1732641926328_0.pdf)
- Summary
  collapsed:: true
	- 3 attacks listed in paper
		- 1st two infer users' audio/video playback using systematic observation and analysis of the multimedia-visualization functionality of smart light bulbs
		- 3rd attack uses the infrared capabilities of smart light bulbs to create a covert-channel to ex-filtrate user's private data out of secured home or office network.
	- Some Smart lights have Multimedia Visualization
		- Change the brightness of the light with the audio
	- Threat Model
		- Passive Adversary
		- Goal is to infer the media consumption of target user
		- Requires light and color sensors
		- Malicious software used within network cannot communicate directly with an adversarial server over Internet, or that user's network is air gapped.
		- Adversary requires IR sensing hardware
		- Adversary needs sufficient computational resources
	- Audio attack:
		- Can use luminescence sensor to capture the changes in brightness
		- Changes in brightness used to recreate audio stream after normalizing the changes caused by color hues
		- difficult to infer due to random order of hue affecting the observed luminance
	- Video Inference Attack
		- Video Visualization causes the smart bulb to react to colors present in the video stream.
		- Video Inference attack focuses on color changes more than the audio inference attack
		- Video inference not as effective as the source video needs to be in a pre-existing database.
			- Still effective at inferring the video genre
	- > practicality of the presented attacks rely heavily on the adversary’s ability to
		- (i) procure sensing and computational instruments,
		- (ii) setup a secure observation point in the neighborhood of the target user, and
		- (iii) have a stable and undisrupted view of the target user’s bulb/window
	- Defenses and countermeasures:
		- The side channels are non-trivial and difficult to implement
		- For the exfiltration attack, adding authentication or access control to the lights would help remedy the problem. Manufactures should add these features to prevent further side/covert channels
		- For users, windows with low visible transmittance hinder the attacks.
		- Using curtains also reduces the attack viability
		- Max brightness of the bulbs can be reduced by the user to hinder inference attacks
		- Using network rules to prevent unauthorized smartphones/computers from accessing the smart light bulbs also helps