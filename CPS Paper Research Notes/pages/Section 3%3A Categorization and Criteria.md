- Selecting reasonable papers and categorizing them into a meaningful taxonomy (20 points
  total)
	- Selection of at least 10 papers from reliable sources, reasonably recent (last 5 years),
	  and not SoK or review (survey) papers (5 points)
	- Creates multiple distinct, meaningful categories for these papers with reasonable
	  distributions of papers in each category (i.e., do NOT make one category of papers with
	  9 papers and another with 1, 10 categories based on the author of each paper, “fuzzy”
	  categories with heavy overlap, etc.) (5 points)
	- The papers placed in each category clearly belong in the category based on its criteria (5
	  points)
	- The chosen criteria for category placement reveals some information about the state of
	  research on the topic and ties into the analysis (5 points)
- Paper Categories
	- Many of the Papers attempt to infer user behavior based on the side channel information gathered
		- [[Paper: HomeSpy: Sniffer of IR Remote Control of Smart TVs]]
		- [[Paper: Peek-a-Boo: Seeing Encrypted Home Activities]]
		- [[Paper: IoTBeholder: A Privacy Snooping Attack on User Habitual Behaviors from Smart Home Wi-Fi Traffic]]
		- [[Paper: Light Ears: Info Leakage via Smart Lights]]
	- Others trying to locate a device(s) or people using part(s) of the smart home network
		- [[Paper: Wireless Camera Localization Leveraging Traffic-Aided Spatial Analysis]]
		- [[Paper: IoTBeholder: A Privacy Snooping Attack on User Habitual Behaviors from Smart Home Wi-Fi Traffic]]
		- [[Paper: Et Tu Alexa? Commodity WiFi Devices as Adversarial Motion Sensors]]
	- Papers trying to view device activity based on information from Side Channel
		- [[Paper: ZLeaks: Passive Inference Attacks on Zigbee based Smart Homes]]
		- [[Paper: Fingerprinting encrypted voice traffic on smart speakers with Deep Learning]]
			- uses machine learning
		- [[Paper: PingPong: Packet-Level Signatures for Smart Home Dev Events]]
			- uses machine learning
		- [[Paper: Your Smart Home Can't Keep a Secret: Automated Fingerprinting]]
			- uses machine learning
- Submitted Text
	- Research papers from the last five years were selected based on the paper's relation to smart Home EM side channel attacks. The papers were then broken into 3 categories based on the intent of the attacker: finding the location and behavior of a device(s) and person(s). Many, of the attacks uses inferences based on or supplemented by machine learning algorithms. All of the inference attacks are effective against encryption and they all have similar countermeasures.
	- Title: Attacker attempting to view device activity
		- Papers involving adversarial models where the goal is to infer device identity, state, and activity (cite papers) based on analyzing wireless traffic of the smart home. This research focuses on analyzing the traffic of the smart home network, regardless of encryption status. Of the four paper analyzed in this category, all but one use machine learning to supplement a portion of the attack (cite the 3).
	- Title: Attacker attempting to locate devices or people
		- This research focuses more on locating devices or people. The threat models of these paper assumes the attacker does not have does not have physical access to interior of the target property but has limit access around the property to place sniffers (cite all three). Unlike the previous category attack rely less on the size or timings of the packet sent over the network, but more on the presences of packets at all. In (cite alexa), information found by the packet header is not required, but (cite other two papers) require the packet headers to identify the devices for localization which can be interfered with as proposed in (cite zleaks). (cite iotBeholder) localizes the device as part of a multistage attack, but fits more inline with the next category.
	- Title Attacker attempting to infer information about users inside the home
		- Beyond finding a device's activity or location based on EM side channel information, attack goals in this category seek to infer and even predict user behavior inside of a smart home (cite all 4). These attacks will typically use information about the device state and use a trained model to infer user behavior. While (cite peek) is referenced by many other papers analyzed here, (cite beholder) goes a step farther and attempts to predict user behavior based on information from the traffic.
-
-