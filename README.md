<div align="left">
  <img src="https://github.com/Dalageo/TwinCAT-VirtualAGV/assets/153513781/498163f4-35a1-45b9-a442-9889c5e9966e" alt="Bechoff TwinCat" width="700"/>
</div>

<div align="left">
  <a href="https://www.beckhoff.com/en-en/products/automation/twincat/" target="_blank">
    <img src="https://img.shields.io/badge/TwinCAT-3.1.4024.55-blue" alt="TwinCAT 3.1.4024.55"></a>
  <a href="https://github.com/Dalageo/TwinCAT-VirtualTram/blob/main/LICENSE" target="_blank">
    <img src="https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey" alt="License: CC BY-NC-SA 4.0"></a>
  <img src="https://img.shields.io/github/stars/Dalageo/TwinCat-VirtualTram?style=social" alt="GitHub stars">
</div>

# Designing and Simulating an Automated Tram Control System Using TwinCAT PLC Programming

This repository contains a simulation project for an Automated Tram System, developed within the <a href="https://www.beckhoff.com/en-en/products/automation/twincat/"> TwinCAT </a> environment as part of a master's course assignment <a href="https://www.hv.se/en/">University West</a>. The assignment involves developing a Human-Machine Interface (HMI) and a virtual process with visualization to control a tram navigating between two stations along a predefined track.
The designed system allows for both manual and automatic operation of the tram, ensuring it can handle passenger boarding and alighting with safety and efficiency. It includes the following functionalities:

- **Manual Mode Activation**: The tram can be driven manually in any direction without restrictions by the driver using the HMI.
- **Automatic Mode Activation**: Automatic driving is enabled when the tram is stationary at the home station, allowing it to shuttle continuously between the two stations.
- **Immediate Stop**: The tram can be immediately stopped by the driver regardless of the current mode. Once stopped, it will remain stationary until manually operated back to the home station.
- **Mode Transition Control**: To switch from automatic to manual mode, the tram must first be stopped at the home station before changing modes.
- **Tram Position and Status Monitoring**: Sensors confirm the tram's presence at stations by turning green, while the HMI provides real-time updates on tram status, including location, movement, and emergency stop.

| Tram | HMI |
|------|-----|
| <img src="https://github.com/Dalageo/TwinCAT-VirtualTram/assets/153513781/fc165a58-38da-4509-9efa-9b0c05afccc7" alt="Tram" width="520"/> | <img src="https://github.com/Dalageo/TwinCAT-VirtualTram/assets/153513781/79a958f4-410f-430c-aef5-23a8f577fa44" alt="HMI" width="250"/> |

## Setup Instructions

1. **Download and Install:**
   [TwinCAT 3 download | eXtended Automation Engineering (XAE)](https://www.beckhoff.com/en-en/support/download-finder/search-result/?download_group=97028248&download_item=650023470)
   
2. **Clone the repository:**
   ```sh
   git clone https://github.com/Dalageo/TwinCAT-VirtualTram.git
   
3. **Navigate to the cloned directory and execute the `TwinCAT Virtual Tram.sln` solution file.**

4. **Navigate to TwinCAT directory and execute Start.bat**:
   ```sh
   C:/TwinCAT/3.1/Runtimes/UmRT_Default/Start.bat

5. **Change the Target System in TwinCAT to UmRT_Default.**
   
6. **Visualization Image Pool Setup**:
    - In the Solution Explorer of `TwinCAT Virtual Tram.sln`, navigate to PLCSim's VISUs and click on the `ImagePool.TcIPO`.
    - Set the correct file path for each image by navigating to the cloned directory TwinCAT-VirtualTram/Image Pool, where you'll find `Background.png`, `Sensor.png`, `Station.png`, and `Tram.png`.
  
7. **Activate Configuration.**
   
8. **Login and Start both 'PLCSim' and 'PLCStudent'.**
  
## Contributions

This project was part of a master course assignment at [University West](https://www.hv.se/en/), with special thanks to the professors for assigning it.

## License

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/). It was chosen to prevent commercial use and to promote free access and open collaboration, ensuring any adaptations remain freely available to everyone.

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

## Citation

```bibtex
@software{Dalageorgos_TwinCAT-VirtualTram_2024,
author = {Dalageorgos, Konstantinos},
license = {CC-BY-NC-SA-4.0},
month = jul,
title = {{TwinCAT-VirtualTram}},
url = {https://github.com/Dalageo/TwinCAT-VirtualTram},
version = {1.0.0},
year = {2024}
}
