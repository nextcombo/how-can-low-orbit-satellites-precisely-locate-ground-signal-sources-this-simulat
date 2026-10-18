# How can low-orbit satellites precisely locate ground signal sources? This simulation system reveals the answer! [Includes Python code]

How can low-orbit satellites precisely locate ground signal sources? This simulation system will tell you the answer! Phased Array Antenna + TDOA Positioning + Monte Carlo Analysis, Unveiling the Hardcore Technology Underpinning High Precision Positioning in Satellite Communications and Electronic Surveillance Low-Earth orbit (LEO) satellites, with their low orbital altitude, small signal delay, and scalable constellation advantages, are becoming the "satellite sentinels" for ground target positioning.
This article introduces a comprehensive LEO satellite TDOA positioning simulation system. It integrates phased array antenna pattern modeling, time difference of arrival (TDOA) positioning algorithms, link budget analysis, and Monte Carlo statistical evaluation, capable of simulating the entire process from signal transmission, satellite reception to position solution, and providing intuitive visual results. Whether you are a communication engineer, a radar enthusiast, or an interested reader in space-based positioning technology, this can inspire you.
🛰️ What can the system do? This set of simulation software provides an interactive graphical user interface (GUI), supporting custom configuration of various core parameters:
Signal parameters: Working frequency, bandwidth, Equivalent Isotropic Radiated Power (EIRP) of the transmitter source.
Antenna parameters: Ground-based phased array element size, simulation beam scanning and off-axis gain loss
Satellite parameters: Number of satellites, orbital height, inter-satellite distance, receiving antenna gain and noise figure.
Positioning indicators: Set the target positioning accuracy and verify the feasibility of the implementation plan.
Single Simulation Execution Process:
1  
Automatically arrange the satellite constellation architecture, adopting a reference main star combined with an orbital satellite layout.
2  
Calculate the power received by a single-star, signal-to-noise ratio, and antenna gain loss values.
3  
Adding TDOA measurement noise, solving the coordinates of ground signal sources relying on numerical optimization algorithms.
4  
Output positioning error, geometric precision factor GDOP and complete inter-satellite link data
Monte Carlo statistical analysis: Different star-to-star distances batch iteration simulation, generate median positioning error, quartile range, GDOP variation curve, automatically select the minimum satellite spacing that meets precision standards.
📡 One of the core theories: The phased array antenna and the directional ground radiation source rely on the phased array antenna to converge the beam towards the satellite. The antenna gain is highest at the beam center, while the satellite's deviation from the central azimuth results in off-axis losses.
The system is equipped with a two-dimensional uniform planar array directional pattern model, and the array elements are arranged in a specific configuration. The array factor can be decomposed into a two-dimensional product operation. By comparing the main beam gain with the difference of any azimuth gain, converting antenna loss, and synchronizing outputting single-star corresponding off-axis angle, gain loss and actual receiving power.
In actual scenarios, if a satellite falls into the sidelobe null zone of an antenna, the received signal-to-noise ratio will sharply decrease, directly increasing the measurement bias of TDOA. Statistical curves can intuitively display the variation rules of satellite signal-to-noise ratio and antenna loss with the change of satellite spacing, thereby pinpointing the root cause of the surge in positioning errors.
⏱️ Theoretical Core II: TDOA (Time Difference of Arrival) Positioning Principle
Taking the network of three satellites as an example, select a single satellite as the reference benchmark to obtain two independent time difference observation values:
Represents the distance from the signal source to the first satellite, which is the speed of light. Each set of time differences corresponds to a hyperbola trajectory, and the intersection points of the two curves represent the actual coordinates of the signal source.
There are multiple errors in the actual engineering process:
Thermal noise: Limited by bandwidth and signal-to-noise ratio.
Interstellar clock synchronization deviation
Atmospheric transmission delay brought by ionosphere and troposphere
Multipath delay caused by ground reflection
The system integrates various types of interference to generate time measurement random noise, which is in line with real working conditions. The differential evolution numerical optimization algorithm is used to search for the optimal coordinates within a two-dimensional plane, matching the measured and theoretical time difference data. Relying on fixed altitude simplification, it ensures efficient and stable solution.
📊 The third core theory: Link budget and signal-to-noise ratio directly determine the accuracy of positioning calculations. The system is equipped with a complete link budget calculation model:
FSPL Free Space Path Loss:
Emission antenna off-axis loss
Satellite receiving antenna gain
Receiver Noise Formula: Combined with the received power, a decibel form of signal-to-noise ratio (SNR) is derived. Changes in satellite spacing can affect the angle of signal incidence, leading to fluctuations in SNR. The system specifically adds a dimension for monitoring the worst satellite SNR.
📐 Core Theory Fourth Point: Geometric Accuracy Factor (GDOP) GDOP is used to assess the impact of satellite and target's spatial layout on positioning accuracy. Under equal measurement error conditions, an unreasonable topological structure can magnify positioning deviations.
Observation matrix is constructed based on TDOA observation equation, calculation formula: , numerically smaller represents a better spatial configuration.
The number and spacing of satellites can be flexibly adjusted, real-time updating GDOP values. Under normal operating conditions, GDOP is positively correlated with positioning errors, and the nonlinear impact of SNR and antenna loss also changes the trend of error variation.
🎛️ Features: Interactive Visualization and Results Interpretation
1️⃣ Single Simulation View XZ Side View: Show orbit height, true coordinates of the target and calculated coordinates along the vertical section
XY Plane View: Plane display of positioning results, the dashed line circle intuitively checks whether the threshold indicator meets the standard
Positioning Error Bar Chart: Comparative actual error with preset precision, color differentiation between qualified / non-qualified status
Satellite SNR Bar Chart: Marks the detection threshold for signals, distinguishes invalid observation satellites
2️⃣ Monte Carlo Analysis View Error - Star Spacing Curve: Median reflects overall error level, shadow interval reflects data dispersion
GDOP Change Curve: Tracks the evolution trend of spatial geometric accuracy with spacing
Error Distribution Histogram: Statistics a large number of samples to evaluate overall positioning performance
Link Extreme Value Curve: Synchronously observes the lowest SNR and maximum antenna loss, quickly troubleshoot abnormal error causes
🧪 Typical Application Scenarios
1  Satellite constellation design: Simulates the effect of satellite numbers, orbit height, and spacing on positioning effectiveness, optimizes network configuration
2  Link index verification: Incorporates equipment parameters to calculate received SNR, validates the feasibility of communication link
3  Blind zone avoidance analysis: Relying on antenna directional pattern to simulate beam loss, avoiding positioning failure areas
4  
Teaching Principle Demonstration: Physical explanation of TDOA positioning, GDOP factors, and Monte Carlo statistical knowledge.
💎 Summarizes this LEO satellite TDOA positioning simulation system's deep integration of antenna physical models with positioning algorithms, covering all dimensions of signal propagation, time difference observations, and spatial geometry simulation. Through single-simulation and batch statistical analysis, it achieves:
Master the impact of star spacing on positioning errors
Identify and resolve positioning anomalies caused by blind spots in antenna beams
Output network parameter suggestions meeting precision requirements
Clearly understand the intrinsic correlation between spatial configuration and positioning accuracy
Whether it is for satellite communication, electronic countermeasure research, or aerospace technology learning and research, this simulation platform can provide quantitative, intuitive, and interactive experimental analysis support.
This article is developed based on MATLAB and Python platforms, and the parameters mentioned in the text are only demonstration examples; actual projects need to be adapted and debugged according to hardware specifications.

## Images

![How can low-orbit satellites precisely locate ground signal sources? This simulation system reveals the answer! [Includes Python code]](01.jpg)
![How can low-orbit satellites precisely locate ground signal sources? This simulation system reveals the answer! [Includes Python code]](02.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
