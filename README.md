# ffellowship
Frequency Fellowship: Examining Radio Wave Propagation from a High Altitude Balloon
---

This is a project for Hack Club's [Apex](https://apex.hackclub.com),
made by:
- [Marcus Kauffman](https://kauffman.tools) KN6UYL (@mineinjava)
- Hudson Hilal (@hhilal123)
- Joshua Truman (@jstruman4929)

We initially had two project ideas for Apex: this and dropping what was
effectively a lawn dart from 100,000 feet. After the lawn dart project
was rejected, we submitted this project.

Many high altitude balloons (HABs) have been launched, almost all of
which have some sort of tracker that transmits the balloon's location.
These transmissions are received by stations on the ground and then
uploaded to the internet, from which we can view the locations of
receiving stations for analysis. Our goal for this project is to study
the differences between different tracker design techniques,
specifically:

- Does radio band selection influence likelihood of reception?
    - Receiving stations on the 2m band are much more common than those
      on the 20m band, but 20m transmissions theoretically travel
      farther.
- There are three common methods of modulating signals:
    - Connecting to a dedicated radio for transmission
    - Using a MS5351M or similar clock generator IC
    - Using [fancy PLL](https://github.com/kaduhi/pico-fractional-pll)
      to "bit-bang" the radio waveform

    **Question: do these three modulation methods have a significant
    difference in quality and therefore propagation?**
- How do different antenna designs affect propagation.

As suggested above, this project can easily be divided into three
"sub-projects":

## 1. Use of the MS5351M Clock Generator IC.

This subproject revolves around the MS5351M clock generator. It features
a custom PCB. Note that this tracker will transmit on both the 20m and
2m bands because the MS5351M has multiple clock generators.

This tracker has quite a few features, many of which are to support
ultra-low power operation, as is common with this style of tracker:

- GPS
- Temperature/pressure sensor
- Shunt
- 3v3 buck-boost converter
- power supervisor to restart the pico
- Sensors can be powered off to conserve power.

This PCB is designed around the Raspberry Pi Pico due to its rigorous
testing and ease of integration. It also features mainly 1206 components
to aid in manual reflow soldering of the PCB.

See the dPicoTracker/ directory for more info.

<img width="1220" alt="image" src="https://github.com/user-attachments/assets/7f470492-ae92-42a6-9955-464c4acf6c3a" />
<img width="442" alt="image" src="https://github.com/user-attachments/assets/3d54dc78-25ee-414b-87be-a32b8e5429ea" />
<img width="450" alt="image" src="https://github.com/user-attachments/assets/0fcfec73-e802-4580-a60f-e8776f611511" />

## 2. Use of PLL:

This subproject uses the Raspberry Pi Pico to generate RF signals,
*without the use of a dedicated radio/chip*. It is by far the simplest
design and also features a GPS which is essential for correcting for the
oscillator drift.

## 3. Use of a Dedicated HT Radio.

This subproject uses a Raspberry Pi Zero W and a custom PCB to connect
to a HT, which will be stripped down to save weight. 

The PCB consists of a voltage regulator to power the Pi and a 555 timer
circuit to ensure that transmissions are limited in time (in case
of a software crash).

<img width="1302" alt="image" src="https://github.com/user-attachments/assets/36d1860b-98f9-4235-a175-2ab4391e6281" />
<img width="619" alt="image" src="https://github.com/user-attachments/assets/dac293cd-b379-4ed7-8f10-603090a213a1" />
<img width="617" alt="image" src="https://github.com/user-attachments/assets/eae42010-35e1-4933-8691-403493354298" />


## Integration:

*coming soon*

## Project Status:

*coming soon*
