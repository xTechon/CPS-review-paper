year-published:: #[[Published 2020]] 
paper-type:: 
source:: [ARXIV](https://arxiv.org/abs/1907.11797)

- ![Ping Pong: Packet-Level Signatures for Smart Home Device Events](../assets/pingpong_1733785172254_0.pdf)
- Summary
	- **Discovery of New Signatures**:
		- The authors identified simple packet-level signatures that consist of sequences of packet lengths and directions, which can effectively detect specific device events (e.g., turning a light bulb ON or OFF).
	- **Automated Extraction**:
		- PING PONG automates the process of collecting training data by triggering device events and capturing the resulting network traffic. It then extracts request-reply packet pairs, clusters them, and creates longer sequences to form the final signatures.
	- Adversarial Model
	  collapsed:: true
		- two types of adversaries: a WAN sniffer and a Wi-Fi sniffer.
		- **WAN Sniffer**:
			- This adversary monitors network traffic between the home router and the ISP network (or beyond). They can inspect the IP headers of all packets but do not have access to the device MAC addresses, which means they cannot identify which specific device has sent the traffic. This type of adversary could include intelligence agencies or ISPs. The WAN sniffer can analyze the overall traffic patterns and infer device activity based on the packet lengths and directions.
		- **Wi-Fi Sniffer**:
			- This adversary monitors encrypted IEEE 802.11 traffic within the local network. They do not know the WPA2 key, so they only have access to information sent in clear text, such as MAC addresses, packet lengths, and timing information. The Wi-Fi sniffer cannot reconstruct TCP connections but can separate traffic into flows of packets exchanged between pairs of MAC addresses. This adversary has a more limited view compared to the WAN sniffer but can still gather significant information about device activity based on the 
			  characteristics of the network traffic.
		- Both adversaries are assumed to know the type of smart home device they 
		  wish to target and can passively monitor the network traffic to extract 
		  signatures and infer user behavior.
		- even with encryption, the metadata from the network traffic can leak private information about the devices and their activities
	- Countermeasures
	  collapsed:: true
		- **Packet Padding**:
			- This technique involves adding dummy bytes to packets to obscure the actual packet lengths. By padding packets to a fixed length (e.g., the Maximum Transmission Unit, MTU) or adding a random number of bytes, the attacker’s ability to infer device activity based on packet length is reduced. The paper discusses how packet padding can effectively guard against packet-level signature attacks.
		- **Traffic Shaping**:
			- This approach intentionally delays packets to confuse inference techniques that rely on the timing of packet arrivals and the overall volume of traffic. By shaping the traffic, the patterns that attackers might use to infer device activity can be obscured.
		- **Traffic Injection**:
			- This method involves adding dummy packets into the network traffic that mimic
			  the characteristics of real events (e.g., similar packet lengths, inter-arrival times, or volume signatures). By injecting fake events into the traffic, the real event traffic can be hidden among the noise created by the dummy packets.
	- VS other techniques
	  collapsed:: true
		- **Traffic Volume/Shape-Based Signatures**:
			- This category includes techniques that analyze the volume and shape of traffic to infer device activity. These methods can identify whether a device is active but often struggle to determine the exact type of event or command being executed. Examples include the work by Apthorpe et al., which focuses on traffic volume analysis.
		- **Statistical Analysis Techniques**:
			- Some existing methods rely on statistical analysis of traffic patterns over time to infer device behavior. These techniques may use features such as the total number of packets, inter-arrival times, and other statistical metrics to make inferences about device activity.
		- **Machine Learning Approaches**:
			- Several studies have employed machine learning classifiers to analyze network traffic and infer device activity. These approaches often require extensive training on labeled datasets and may not generalize well to new devices or event types.
		- **HomeSnitch**:
			- This is a specific tool mentioned in the paper that identifies IoT activity based 
			  on the observation that devices and servers communicate in a request-reply manner. While HomeSnitch shares some similarities with PING PONG, it relies on broader statistics derived from the entire client-server dialog rather than focusing on the specific lengths and directions of individual packets.
		- **Zigbee/Z-Wave Specific Techniques**:
			- Some techniques focus on specific protocols like Zigbee or Z-Wave, which may require specialized sniffers to capture traffic. These methods are often limited to a narrow set of devices and may not be applicable to a wider range of smart home devices that use different communication protocols.
		- **Volume-Based Inference Attacks**:
			- These attacks analyze the overall volume of traffic to infer device activity. They can be mitigated by traffic shaping techniques, which aim to obscure the volume patterns that attackers rely on.
		- paper highlights the limitations of these existing techniques, such as their inability to differentiate between specific event types, their reliance on clear-text communication, and their higher false positive rates.