# whoview
The WhoView class is used respond to the MQTT topic **diy/system/who**. This class is one of six general classes in my *do it yourself home automation system* (**DIYHA**). Each python DIYHA application is hosted on a Raspberry Pi server and will respond to a **diy/system/who** subscribed topic and report on their status, hostname and IP address. Some applications have a true user interface, e.g., 8x8 matrix or seven segment LED, to display their IP address. 

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![PyPI - Python Version](https://img.shields.io/pypi/pyversions/Django)
[![linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)

> Live demo [_here_](https://www.example.com). <!-- If you have the project hosted somewhere, include the link here. -->

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Features](#features)
* [Screenshots](#screenshots)
* [Setup](#setup)
* [Usage](#usage)
* [Project Status](#project-status)
* [Room for Improvement](#room-for-improvement)
* [Acknowledgements](#acknowledgements)
* [Contact](#contact)
<!-- * [License](#license) -->


## General Information
- Provide general information about your project here.
  - This is one of six classes used in my home automation system (**DIYHA**). I've used OOP and MVC concepts in my DIYHA system. 
- What problem does it (intend to) solve?
  - I wanted to isolate the who server identification status into a single class. The main python application subscribes to a **diy/system/who** topic and responds by turning on or off who messages.
- What is the purpose of your project?
  - My home automation system contains environment sensors, motion sensors, LED clocks, light switches, emergency sirens, a django web server, interfaces to Adafruit.io and a mosquitto MQTT broker.
- Why did you undertake it?
  - This was a fun project to learn about python, Raspberry Pi, Arduino processors, hardware and more.
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- python - version 3.7.3
- paho.mqtt.client - version TBD

## Features
List the ready features here:
- Handles the basic **diy/system/who** functions
- Reports on status, hostname and IP address by way of a MQTT publish and LOGGING info message.
- Code passes pylint with a score of 10.0


## Screenshots
Not applicable.
<!-- ![Example screenshot](./diyhadiagram.png)-->
<!-- If you have screenshots you'd like to share, include them here. -->

## Architecture
![Example screenshot](./diyhadiagram.png)
<!-- If you have screenshots you'd like to share, include them here. -->

## Setup
What are the project requirements/dependencies? Where are they listed? A requirements.txt or a Pipfile.lock file perhaps? Where is it located?

Proceed to describe how to install / setup one's local environment / get started with the project.


## Usage
How does one go about using it?
Provide various use cases and code examples here.

```
├── asset.py
├── asset.service
├── LICENSE
├── logging.ini
├── pkg_classes
│   ├── configmodel.py
│   ├── djangoview.py
│   ├── statuscontroller.py
│   ├── testview.py
│   ├── topicmodel.py
│   └── whoview.py
├── README.md
├── requirements.txt
├── systemd_script.sh
```
`write-your-code-here`


## Implementation Status
![Status](https://progress-bar.dev/80/?title=progress)


## Room for Improvement
Include areas you believe need improvement / could be improved. Also add TODOs for future development.

Room for improvement:
- Improvement to be done 1
- Improvement to be done 2

To do:
- Feature to be added 1
- Feature to be added 2


## Acknowledgements
Give credit here.
- This project was inspired by...
- This project was based on [this tutorial](https://www.example.com).
- Many thanks to...


## Contact
Created by [@parttimehacker](http://parttimehacker.io/) - feel free to contact me!
### Repository Stats
![Your Repository’s Stats](https://github-readme-stats.vercel.app/api?username=parttimehacker&show_icons=true)
### Repository Languages
![Your Repository's Stats](https://github-readme-stats.vercel.app/api/top-langs/?username=parttimehacker&theme=blue-green)
### HITS
![Hits](https://hitcounter.pythonanywhere.com/count/tag.svg?url=https://github.com/parttimehacker)


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
