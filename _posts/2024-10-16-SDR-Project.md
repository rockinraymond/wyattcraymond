---
layout: post
title: Exploring Satellite Decoding with Software Defined Radios (SDR)
---
The world of satellite communication is continually evolving, driven by the need for adaptable and cost-effective solutions. As we look to decode signals from weather and educational satellites, Software Defined Radios (SDRs) have emerged as a powerful and versatile tool. In my latest project at Old Dominion University, I explored the potential of SDRs to receive and decode satellite signals, offering a deep dive into the technology's real-world applications. This blog post summarizes key findings and insights from my Master Project report, titled "Decoding Satellite Signals Using Software Defined Radios."

Software Defined Radios (SDRs) are communication systems where the signal processing is largely handled by software instead of hardware. Unlike traditional radios that require physical components for signal modulation and demodulation, SDRs leverage software flexibility to process various signal types and frequencies. This enables quick adaptation to new satellite protocols, making SDRs especially valuable in the dynamic landscape of satellite communication.

SDRs are widely adopted for satellite communication because they allow for decoding signals from a wide variety of satellite systems without needing to replace hardware components. My project focused on receiving signals from both NOAA weather satellites and the BEESAT pico-satellites. Using a low-cost SDR device like the RTL-SDR dongle, I was able to process complex satellite signals, decode telemetry, and generate real-time weather imagery.

![Gpredict and SDRSharp Software](/images/noaa18may24th.JPG)

The hardware setup for receiving satellite signals was minimal but effective. I used an RTL-SDR Blog V3 dongle connected to a simple dipole antenna. Paired with powerful software like Gpredict for satellite tracking and WxToIMG for decoding, I was able to achieve accurate results in real-time. My experiments took place in a location where I ensured minimal obstructions for optimal signal reception. This simple yet powerful setup demonstrates how SDR technology can be accessible to both hobbyists and professionals.

![SDR Hardware Setup using RTL-SDR Dongle, Dipole antenna and my laptop](/images/SDR_SETUP.jpg)

The NOAA satellites, which are critical for weather forecasting, employ the Automatic Picture Transmission (APT) system to transmit low-resolution images of the Earth. During the project, I captured APT signals from NOAA 15, 18, and 19 satellites. Using the captured signals, I was able to decode and produce weather images with color overlays and thermal enhancements. SDR technology, coupled with software like SDRSharp and WxToIMG, allowed for seamless decoding of these signals.

![NOAA 19 Decoded Image](/images/NOAA19_24MAY_1000.jpg)

![NOAA 19 Decoded Image - Color Filter](/images/NOAA19_24MAY_1000_color.jpg)

![NOAA 19 Decoded Image - Thermal Filter](/images/NOAA19_24MAY_1000_thermal.jpg)

The versatility of SDRs makes them an ideal tool for decoding satellite signals, and the potential applications extend beyond weather forecasting to include space research, environmental monitoring, and educational outreach. My project has shown that, with minimal hardware investment and open-source software, anyone can explore the exciting world of satellite communication.

As SDR technology continues to advance, I look forward to future innovations that will further streamline the process of satellite signal decoding and open up new possibilities for communication systems around the world.

For anyone interested in learning more, the full project report provides in-depth details on the setup, methodologies, and results obtained during my experiments. SDRs have proven to be a game-changing technology, and I hope this post inspires others to explore the field further! [Report can be downloaded here](/ECE_698_Report_WyattRaymond.pdf)
