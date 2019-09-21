# IoT Pulse Oximeter
This is project has a two-fold purpose:
1) Create a Sigfox enabled finger-tip pulse oximeter for use in public hospitals in South Africa to allow doctors and other medical staff to more easily track patient oxygen saturation in near real-time.
2) Provide a guide for anyone wanting to build one themselves and/or learn about some basic reverse engineering of serial communications.

## Project Overview
The project is based on the Yonker YK-80 finger-tip pulse oximeter which is readily available online. The oximeter works by measuring the absorption of different wavelengths of light when passing through the finger-tip; oxygenated haemoglobin exhibits higher absorption than normal haemoglobin and thus the measurements give an insight into the levels of oxygenated haemoglobin and ultimately the sp02 of the patient (partial pressure of oxygen). For the majority of individuals measuremed sp02 should be greater than 90%; anything lower can indicate the person is not receiving adequate oxygen. In the hospital setting this is important when monitoring patients that are on ventilation and/or other critically ill patients that could require ventilation.

Typically all public hospitals will have equipment that can measure the sp02 of such patients; however, it is currently up to nursing staff to notice significant changes and contact the doctor on duty. Due to the nature of public healthcare this cannot or is not always done in a timely manner and endanger the patient. While equipment with automated reporting techniques over various wireless network back ends does exist, it is generally expensive and requires a level of technological sophistication and infrastructure that is not viable in the majority of public hospitals in South Africa. 

There is a clear need for technology that is cost-effective to operate and can operate without relying on access to the internet. This project was born to meet this need.

The viable options for such a IoT service are clearly fairly restricted; in fact apart from LoRa, GSM/GPRS and Sigfox there is no other cost-effective backend solution. GSM/GPRS and Sigfox are available throughout the majority of South Africa, however, LoRa does not appear to have had a similar uptake in the country and most areas do not have access to a LoRa gateway. Comparing GSM/GPRS and Sigfox it is clear that Sigfox is at an advantage. Firstly, accessing sim cards for multiple devices is a tedious process due to government regulations. Secondly, using GSM/GPRS to connect to a backend server is signifcantly more effort than required with Sigfox and reducing the technological barrier to entry is important as it enables the development process to be accelerated. It was thus decided a Sigfox solution would be the best route forward.

In order to investigate the validity of the concept an existing commercial pulse oximeter was reverse engineered and interfaced to the Sigfox network. It is hoped that once the concept is tested and validated in a clinical setting that it will be expanded to other monitoring equipment and ultimately lead to building a low cost device reporting network that device manufacturers can use to design lower-cost equipment with automated reporting capabilities.

## Reverse Engineering the YK-80 Pulse Oximeter Serial Protocol

## Getting Setup with Sigfox

## Interfacing the Oximeter with Sigfox
