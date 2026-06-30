---
permalink: /
title: "Huijie Zhang – Satellite Network & Network Telemetry Research"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

This is the personal academic website of  Huijie Zhang.
I am a graduate researcher in the field of **communication engineering and satellite communications**, currently focusing on **LEO satellite network measurement, telemetry systems, and intelligent network management**.
I am affiliated with Nanjing University, where I work under the supervision of Kanglian Zhao.

My research interests lie in designing efficient and intelligent mechanisms for large-scale, highly dynamic satellite networks. In particular, I focus on how to improve the observability, freshness, and interpretability of network state information under highly dynamic conditions.

My work combines network measurement, optimization, and data-driven intelligence to support next-generation LEO satellite network systems.

Research Interests
- LEO satellite network architecture and system design  
- In-band network telemetry (INT/IOAM) and network measurement  
- Path-aware probing and active measurement in dynamic networks  
- Semantic-driven network state modeling and intelligent O&M  

Selected Achievements
- Two invention patents (authorized)
- Challenge Cup Gold Award
- Research work in satellite network measurement and optimization (ongoing submissions)
- Multiple project participations in network telemetry and intelligent systems

A flow-aware in-situ detection method for space networks.
======
The present invention discloses an in-situ space flow telemetry method (in-Situ Space Flow Telemetry, iSFT), which performs real-time data collection and monitoring in space networks. The method mainly includes the following steps:
First, a compression method for in-situ telemetry data is proposed, in which both in-band Operations, Administration, and Maintenance (OAM) option headers and metadata are compressed to obtain a compact in-situ telemetry option header and metadata. Compared with RFC-standard approaches, this method saves memory resources more efficiently.
Second, the Flow Label field in the IPv6 header is used to determine node types and identify sampled packets, achieving accurate, efficient, and resource-saving detection.
In addition, a sampling-template-based mechanism is adopted to instruct each node to collect in-situ telemetry metadata. The collected telemetry metadata is classified into three categories—packet loss, latency, and congestion—with a total of eight sampling templates.
Finally, a method is introduced for inserting the in-situ telemetry option header between the UDP/TCP header and the payload of the original packet for transmission.

A packet path tracing method for satellite networks.
======
The present invention discloses a packet path tracing method for satellite networks. The method realizes packet path tracing in a dynamic satellite network by utilizing the flow label in the IPv6 packet header. A unique flow identifier is assigned to each traffic flow by mapping the flow label of the packet, and this identifier is mapped into the IPv6 header flow label and written into the in-band telemetry header. At each satellite node, the flow is identified through the flow label, and metadata is collected. The telemetry data is then transmitted to an in-band telemetry collection module.

The in-band telemetry collection module analyzes the received telemetry data based on timestamps, packet sequence numbers, and node identifiers, and reconstructs the forwarding path of all packets within the service flow. Based on this, a time-varying graph of the service flow path is constructed using time-varying graph theory.

Finally, a constellation topology table based on ephemeris is introduced as the spatiotemporal reference for satellite network link establishment. A traffic scheduling strategy table and a solar eclipse period table are further introduced as references. By combining these with the time-varying graph of the service flow path, the method infers the causes of packet path switching.
