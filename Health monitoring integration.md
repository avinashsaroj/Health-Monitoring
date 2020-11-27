# Interfacing the Health Monitoring Sensors

Selecting the health monitoring sensors is an important part of the project that requires a lot of research , but interfacing those sensors to a suitable and powerful controller is completely a different set of actions that increase the productivity and fruitfulness of those sensors. 

Special attention has been paid to the interfacing part because , as far as the aim of the project suggest the health monitoring of the Air Force pilots , this can be a really important and life saving task. Special attention will be paid to timing deadlines of the output of the controller , it has to be repeatable and simple .

## Selection of the controller and the options available

As far as selection of the controller is concerned relating just to the interfacing of sensors , there are many controllers present that will serve the purpose well. Some of them are mentioned below:

| Controller     | Cost     |
| -------------- | -------- |
| Atmega 16      | INR 225  |
| Arduino Mini   | INR 245  |
| STM 32         | INR 268  |
| Raspberry Pi 4 | INR 3590 |

### Why?

It is not the interfacing that matters or the cost of the controller, it is the functionality and the ease of use that the system provides to it's user. Our aim is to use a controller or I will say a system that is easy to use for the pilot and that provides multiple options for the data management.

I have listed some of the advantages focusing on which I have selected the given system:

- The availability of the Operating System
- Availability of the high speed USB ports
- High primary and the secondary storage
- Easy to access
- Built in networking system
- Easy Graphical User Interface
- Easy Casting options

### Technical Specs

| Specs        | Brief                                                        |
| ------------ | ------------------------------------------------------------ |
| RAM          | 2 GB                                                         |
| ROM          | as required but we will use 128GB                            |
| USB          | USB 3, USB 2                                                 |
| Network      | Gigabit ethernet and inbuilt WiFi and BLE                    |
| Supply ports | Ethernet,USB,USB-C                                           |
| Power        | 15W (5V input)                                               |
| Processor    | Broadcom BCM2711, Quad core Cortex-A72 (ARM v8) 64-bit SoC @ 1.5GHz |
| GPIO         | 40 Pins                                                      |
| Compliance   | The Raspberry Pi 4 has undergone extensive compliance testing and meets a number of regional and international standards. |



## Interfacing

As most of the sensors are giving analog output, so all the sensors are connected to the ADC pins. All the data is stored into the secondary memory and simultaneously the live graph will be processed onto the LED display. Power to all the sensors is  to be delivered by the Raspberry Pi itself. Inputs from the sensors is to be processed by the system once at a time , since the graph also needs to be plotted at the same time.

### Data Processing

Data processing is the core of the functionality of the project, because the data is to be stored as well as displayed. As far as storing is concerned , the readings are stored in a CSV file and each sensor will have it's different file for the data. And for display , the live graph of the data will be displayed on the screen and the screen will also have the maximum and minimum readings recorded by the controller in a particular set of event. And the screen will also have the normal health standards of the parameter being measured.

### Alarms

Just storing the data and displaying is not sufficient because of the importance of the environment that the pilot is in. When the data is being displayed on the the it will also be compared to the standards of the parameter and a alarm will be set. The alarm will possibly be a speech text produced by the computer.

### Data Backup

Data can be stored onto the secondary memory and it can also be simultaneously stored onto a external device as per the convenience of the pilot. Data will automatically be uploaded to a server provided there is a internet connection or a local server connectivity for the system.

## Innovation

Beyond just fulfilling the need of the project and satisfying it's requirement our team is also putting in some ideas for the improvement of the accessibility of the system and making is more accurate and user friendly. Some of the innovation ideas are listed below:

- Accessing the system is not a challenge , as the system is itself being integrated into the helmet of the pilot (keeping in mind the freedom of the pilot)
- The system is planned to possess the Talk-back feature that is the system will be able to respond to the pilot to some extent
- I case the readings of the parameter exceed the standards of the parameter , the alarm will be set and the data will immediately be sent to the server

## References

[2]*Raspberrypi.org*, 2020. [Online]. Available: https://www.raspberrypi.org/products/raspberry-pi-4-model-b/specifications/?resellerType=home. [Accessed: 26- Nov- 2020].

[3]A. Saroj, "avinashsaroj - Overview", *GitHub*, 2020. [Online]. Available: https://github.com/avinashsaroj?tab=repositories. [Accessed: 26- Nov- 2020].

