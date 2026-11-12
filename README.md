<div align="center">

  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,60:161b22,100:1f6feb&height=200&section=header&text=Maciej%20Stadler&fontSize=42&fontAlignY=38&desc=5th-semester%20Automatic%20Control%20and%20Robotics%20Student%20%7C%20AGH&descFontSize=16&descAlignY=58&fontColor=ffffff&descColor=79c0ff" width="100%" alt="Header" />

  <p align="center">
    <b>Embedded Systems • Real-Time Control • Robotics & Computer Vision</b>
  </p>

  <p align="center">
    <a href="https://www.linkedin.com/in/maciejstadler/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
    <a href="https://github.com/corki1337"><img src="https://img.shields.io/badge/GitHub-corki1337-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub" /></a>
    <img src="https://img.shields.io/badge/Location-Kraków%2C%20Poland-238636?style=flat-square" alt="Location" />
  </p>

</div>

---

### 👨‍💻 About Me

- 🎓 **5th-semester Automatic Control & Robotics (AiR)** student at **AGH University of Krakow**, combining control theory with hands-on hardware.
- ⚡ **Embedded & Firmware:** Writing peripheral drivers, communication protocols and real-time control loops in C/C++ on **STM32**, **ESP32-S3** and **Raspberry Pi**, both on FreeRTOS and with direct HAL/register access.
- 🎛️ **Control:** Designing and tuning closed-loop controllers on real hardware: cascaded PID, sensor fusion and actuator handling.
- 🐧 **Linux-native:** Daily driver on Ubuntu with Git workflows, CMake build pipelines and low-level debugging.
- 🌱 **Current Focus:** Robotics with ROS 2, real-time embedded architectures and computer vision.

---

### 🚀 Featured Projects

#### ⚖️ [STM32 Self-Balancing Robot](https://github.com/corki1337/stm32-self-balancing-robot)
> *A two-wheeled inverted-pendulum robot on STM32L476 with FreeRTOS, remote-controlled over ExpressLRS.*
- **Cascaded control:** PD tilt-angle loop at **1 kHz** with the derivative taken directly from the gyroscope, driven by a PI wheel-speed loop at 100 Hz, with anti-windup and fixed-period scheduling.
- **Sensor fusion:** MPU6050 over I²C, complementary filter for tilt estimation and gyro bias calibration at startup.
- **CRSF protocol from scratch:** 420 kbaud UART with **DMA Receive-to-Idle**, frame synchronization, CRC-8 validation and 16×11-bit channel unpacking. ISR-to-task notifications, a latest-value queue between tasks and a 200 ms link-loss failsafe.
- **Motor control:** Dual DRV8874 H-bridges at 20 kHz PWM, quadrature encoders on hardware timers, fall detection with motor cut-off.
- `C` • `STM32 HAL` • `FreeRTOS` • `DMA` • `UART` • `I²C` • `PWM` • `PID Control`

---

#### 🎮 [ESP32-S3 Retro Handheld Console](https://github.com/corki1337/esp32-console)
> *A complete handheld game console built from the ground up on ESP32-S3 without external GUI libraries.*
- **Custom 2D Graphics Engine:** 160×128 ST7735S display driven via asynchronous **SPI DMA double-buffering** with color-key transparency.
- **Multithreaded Audio:** Independent **FreeRTOS task** streaming 16-bit 16 kHz PCM audio over **I2S** with thread-safe mutex dispatch.
- **Hardware Integration:** Curve-calibrated **ADC** battery monitoring, **LEDC PWM** gamma-corrected backlight and **NVS** flash persistence.
- **Built-in Games:** 3 games written in modern C++ (including *Pickle Snake* with dynamic body corners).
- `ESP-IDF` • `C++17` • `FreeRTOS` • `SPI DMA` • `I2S Audio`

---

#### 🎯 [bala_tracker — Vision-Guided Laser Pan-Tilt](https://github.com/corki1337/bala_tracker)
> *A distributed ROS 2 system: a Raspberry Pi 5 detects a colored object and an ESP32-S3 aims a laser at it with a pan-tilt servo mount.*
- **Perception node:** Pi Camera v3 through a GStreamer/libcamera pipeline at 720p60, HSV color segmentation, morphological filtering and largest-contour centroid extraction.
- **ROS 2 ↔ micro-ROS:** Target coordinates published as `geometry_msgs/Point` from ROS 2 Jazzy to a micro-ROS node on the ESP32-S3 over a serial transport.
- **Actuation:** ESP32-S3 maps image coordinates to servo angles and drives both axes with 50 Hz PWM.
- `ROS 2` • `micro-ROS` • `Python` • `OpenCV` • `ESP32-S3` • `Raspberry Pi 5`

---

#### 🏭 [NetSim — Production Network Simulator](https://github.com/corki1337/NetSim)
> *An object-oriented discrete-time simulator of a production network: loading ramps, workers and storehouses.*
- Nodes connected through weighted **probabilistic routing** with an injectable random generator.
- Network **consistency check** via graph traversal, structure loading and saving from text files, and periodic simulation reports.
- `C++` • `Object-Oriented Design` • `STL` • `CMake`

---

### 🛠️ Tech Stack & Tooling

<div align="center">
  <img src="https://skillicons.dev/icons?i=c,cpp,python,cmake,linux,git,ros,opencv,arduino,raspberrypi,vscode&theme=dark" alt="Tech Stack" />
</div>

<br/>

| Domain | Technologies |
| :--- | :--- |
| **Microcontrollers** | STM32 (HAL, CubeMX), ESP32-S3 (ESP-IDF), Arduino, Raspberry Pi |
| **Embedded** | FreeRTOS, DMA, UART, SPI, I²C, I2S, ADC, PWM, timers & encoders |
| **Control & Robotics** | PID / cascaded control, sensor fusion, ROS 2, micro-ROS |
| **Languages** | C, C++17, Python |
| **Vision** | OpenCV, GStreamer |
| **Environment** | Linux (Ubuntu), Git, CMake, STM32CubeIDE, VS Code |

---

<div align="center">
  <sub>Maciej Stadler • Kraków, Poland</sub>
</div>
