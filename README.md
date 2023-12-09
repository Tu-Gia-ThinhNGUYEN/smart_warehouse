# 1. Overview

This is parts of project "Smart Warehouse" with SPK-Salt team. This project was developed for the Mitsubishi Electric Cup Automation 2021 (MECA 2021) competition.

In this project, I'm responsible for Webserver and Supervisory Control And Data Acquisition (SCADA) system development.

# 2. Results
## 2.1 SCADA

The SCADA system is developed in Windows Form App with C#. This system is used for supervise and control warehouse model (using Programmable Logic Controller (PLC) iQ-R series of Mitsubishi Electric). In addition, this system also aquisition data from under layer, store data to the local storage and cloud (Firebase), this system also plays role of back-end for webserver read data from realtime database then handle requirement of user from webserver to PLC and update respond of PLC to realtime database.

The Graphic User Interface (GUI) is as bellow:

![SCADA](/images/SCADA.PNG)

## 2.2 Webserver

The webserver is using hosting of Firebase. All requirement of user will be updated to realtime databse, which will be handled by SCADA system, then responds and updates all status of Smart Warehouse system to webserver. So webserver is able to be online over internet through this method.

Link of webserver is here: https://meca-spksalt.web.app/

Preview of website:

![SCADA](/images/Web capture_7-5-2022_20513_127.0.0.1.jpeg)

## 2.3 Overview of all systems

![SCADA](/images/Model.png)
