---
layout: project
type: project
image: images/SmartAlawai.jpg
title: Alawai River 2014 Data Analysis
permalink: projects/Smart Alawai
date: 2020-01-23
labels:
  - Data Analysis
  - Data Visualization
  - Python3 
summary: As a technical research assistant, I contributed to analyze the data obtained from Alawai River in 2014 Spring.
---

<div class="ui small rounded images">
  <img class="ui image" src="../images/Sensonrs location.png">
  <img class="ui image" src="../images/Mean velocities plot Westpng.png">
  <img class="ui image" src="../images/Plot of Pressures with no tides.png">
  <img class="ui image" src="../images/Salinity plot.png">
</div>

  SMART ALAWAI PROJECT is a local project that faculties from schools/universities in Oahu and (under)graduates in University of Hawaii at Manoa work for the improvement of water quality of Alawai River in Honolulu. As a project member, I and my supervsior Associate Professor Brian Powell in University of Hawaii at manoa analyzed the data obtained by the sensors deployed in each different location of Alawai River in 2014 Spring. The data consist of several environmental sections stored as dictionaries: Temperature, Salinity, Pressure, and etc. Each sensor recored the data in every five minutes for 4 months. 
  
  The main purpose of the analysis was to find the behavior of Alawai after discharging by comparing the data with the discharge data. The analysis was made of three sections: Observational data, Model Data, and Comparison. In the first section, I broke down each dictionaries of the data from each sensor and analyzed them with visualiziation with colormeshes and xy plot graphs. In the second section, I analyzed the model data, looking at how close the model is to the actual observed data. In the last section, I made the comparison between the observation data and model data, to explain how successfully the machine predicted

  Through this year and 9 months project, I sucessfully led the fundmental analysis to be the base for the conclusion. Moreover, I learned how to visualize and analyze the big data with Python3. As well, I could improve my understanding of the dictionary system and effective coding in Python3. 
  
```js
for d in range(18):
    xin_east = u_east[:,d] + 1j*v_east[:,d]
    
    fit_east = seapy.tide.fit(time_east, xin_east, tides = ['M2', 'S2', 'K1'], tide_start=datetime.datetime(2017,3,28))
    
    vel_notides_east = xin_east - fit_east['fit']
    u_notides_east = np.real(vel_notides_east)
    v_notides_east = np.imag(vel_notides_east)
    
    mean_u_notides_east[d] = np.mean(u_notides_east)
    mean_v_notides_east[d] = np.mean(v_notides_east)
    std_u_notides_east[d] = np.std(u_notides_east)
    std_v_notides_east[d] = np.std(v_notides_east)
    depths_east = np.mean(bin_depths_east, axis = 0)
    
```

You can learn more at the [Smart-Alawai Website](http://www.smart-alawai.manoa.hawaii.edu/).



