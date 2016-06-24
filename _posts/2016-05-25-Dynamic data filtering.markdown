---
layout: post
title:  "Dynamic Data Filtering"
date:   2016-05-25
categories: Wireless-Sensor-Networks

---

The emerging field of wireless network consisting of spatially distributed autonomous devices to sense physical or environmental conditions, has gained much attention of the researchers. Being a hot topic of research, I decided to go into its depths and explore new areas related to data dissemination and power consumption. The studies showed that the presence of limited power sources acts as a critical problem here. So, a dynamic filtering scheme has been discussed here to resolve this problem for its efficient use. 

The data to be disseminated by a Sensor Node(SN) is first filtered and then sent to the Cluster Head Node(CHN). Sensing a slowly changing event with very high frequency leads to wastage of energy as it may generate redundant data. Whereas, sensing rapidly changing event with low frequency may cause loss of useful information. Therefore, spurious and redundant data filtering has to be done which itself requires a lot of efforts. The unpredictable change in the behavior of an event induces a need to have a dynamic and slidable data filtering window, which changes its position by self adjusting its lower and upper bounds as the sensor readings go up or down. As a result, once SN is deployed it remains self sustaining.

This way only the useful values lying inside the window are disseminated to CHN. Thus, significant amount of energy is saved by eliminating undesirable inter-node transmissions thereby reducing the cost of power of the sensor network operation.

#Simulation

To validate the proposal, a simulation was conducted on 10,000 random temperature readings between 13 deg C to 47 deg C. The scenario is depicted in two ways.

a) The temperature readings are kept constant for various Common node Dissemination intervals (CNDI) and the net power consumption is calculated for each CNDI.


b) The temperature readings are different for all Common node Dissemination intervals (CNDI) and the net power consumption is calculated for each CNDI.


Lately, I along with my mates have been writing a research paper on this. The complete algorithm and the simulation results are depicted there. I am looking forward to present it out at the earliest. :)



_________________________________________________________________________________________________________________________________________________________






