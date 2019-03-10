---
layout: post
title:  "AstroJays - Avionics & Payload"
date:   2017-08-14
categories: blog
---

##### Overview:

In August of 2017 I joined the [AstroJays](https://www.linkedin.com/company/11467715/). The AstroJays are a team of Johns Hopkins University undergraduates dedicated to learning how to design, assemble, and launch rockets. Each year, the team participates in the SpaceSport America Cup where over 1,100 students and faculty from more than 70 institutions, gather to collaborate and compete at a world class space-sport facility. The competition typically involves the designing building and flying of high powered rockets containing a significant payload in a professional setting.

I became the team's payload leader by proposing the use of a current NASA project I had undergone at the university (You can check that project out here). Soon after I became the leader of the Avionics Ground Station team.

##### *Avionics:*
As leader of the Ground-Station avionics team I was in charge of a team of 6 software and computer engineers in the development and implementation of a web application that  provides live-data from the rocket to the user. The web app was developed for users that have no coding experience. The app completely ingests and process the data providing live graphs to the user on acceleration, altitude, angular position and GPS live coordinates of the rocket overlaid on a google map.

<img src="https://raw.githubusercontent.com/lrodri29/LuisWeb/gh-p/Screen%20Shot%202018-03-11%20at%208.20.08%20PM.png" width="50%" height="100%" align="right"/>The application uses both FlaskApp and React in unison to work in both the processing and display of the rocket's data respectively. In the back-end a FlaskApp uses Python to collect data from a connected Arduino to the operations computer which communicates to the Arduino on-board the rocket through an ROF and antenna. The python code pulls in the data, processes it and then sends it to the front-end React App which creates data plots to visualize the data. You can see an image of the web-app on the right.

##### *Payload:*
As leader of the payload team I proposed the use of the project I describe [here](http://luisrodriguezeng.com/blog/2017/05/15/NASA-Funded-Microfluidic-ITP-Device.html). The payload's delivery method is as follows: An Arduino UNO on the on-board avionics section of the rocket collects data on altitude and communicates it to a second Arduino on board which controls the payload bay. Once the rocket is within a given range of the target apogee the payload's Arduino communicates with a pump that pushes the liquid through the microfluidic device at a constant velocity. The payload's Arduino also flips the switch on a relay by providing current to the magnetic coil in it allowing for four 9V batteries to power each side of the microfluidic device shown in figure 2 <img src="https://raw.githubusercontent.com/lrodri29/LuisWeb/gh-p/Screen%20Shot%202018-02-28%20at%209.35.38%20PM.png" width="50%" height="100%" align="right"/>. The electromagnetic field displaced across the device's channel achieves a separation of the sample consisting of positively and negatively charged particles to simulate blood serum.

The AstroJays rocket also carries methane and CO2 sensors to measure and assess contamination levels at apogee in the launch site area. The purpose of these sensors is mainly to investigate the long term effect of rocket launches on the atmosphere near the launch site where the SpaceSport America Cup takes place. These tests are not considered the rocket's main payload but will be the first of a series of a three year data collection period which the team will present at the 2020 competition as the main payload of that year's rocket.
