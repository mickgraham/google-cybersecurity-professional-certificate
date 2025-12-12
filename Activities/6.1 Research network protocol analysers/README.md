# Activity: Research network protocol analysers

*This activity is based on a fictional scenario.*

**References**

* **diagram-template.pptx:** Wireshark and tcpdump venn diagram template
* **diagram-exemplar.pptx:** Sample solution

## Scenario

In your role as a cybersecurity analyst, you have been asked to research the differences and similarities between Wireshark and tcpdump and create a chart that outlines your findings.

## Research network protocol analysers

| Category | Wireshark (GUI Tool) | Both | tcpdump (CLI Tool) |
|----------|------------------------|-------|-----------------------|
| **Required Software / Equipment** | Windows support | libpcap library dependency,<br>Open-source | Natively installed on many Linux distros |
| **User Interface / Layout** | Graphical user interface (GUI) | Show packet breakdowns,<br>Can save/load .pcap files| Command-line interface (CLI) |
| **Typical Use Cases** | Detailed interactive analysis | Incident response | Quick packet captures ,<br>Automated or scripted captures |
| **Capturing / Analysing / Filtering Traffic** | Captures and analyses packets visually | Read/write .pcap files | Captures raw packets |
| **Limitations / Considerations** | Heavy resource usage,<br> Requires a graphical environment | Require elevated permissions | No visualisation or deep protocol analysis |

* Wireshark is best for interactive, detailed analysis using a GUI, protocol decoding, and visualisation.
* tcpdump is best for quick, scriptable, terminal-based captures, especially on headless or remote systems.
* Both are open-source, rely on libpcap, and are standard tools in incident response and network analysis.
