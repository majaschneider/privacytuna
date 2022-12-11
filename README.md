# Privacy Tuna: Tuning the Utility-Privacy Trade-Off in Trajectory Data

<img src="resources/tuna_logo_db_l.png" alt="" width="128"/>

*Privacy Tuna* is an open source visualization system that enables users to assess the privacy risk in 
trajectory data, to apply privacy-preserving mechanisms and intuitively tune the trade-off 
between utility and privacy by adjusting the parameters of the algorithm.


### The Privacy of Trajectory Data
Trajectory data, often collected on a large scale with mobile sensors in smartphones and vehicles, 
is a valuable source for realizing smart city applications, or improving the user experience in apps. 
But such data can also leak private information about those who produced it. It can reveal not only a person's 
whereabouts, but also very personal information about them, such as their points of interest (POI), which in turn can 
reveal a person's age, gender, religion or home and work address. Location privacy preserving mechanisms (LPPM) can 
mitigate this issue by transforming the data so that private details are protected. But privacy-preservation 
typically comes at the cost of a loss of utility. It can be challenging to find a suitable mechanism and the right 
settings to satisfy privacy as well as utility. 
an interactive framework to visualize trajectory data, and intuitively estimate data utility and privacy while applying LPPMs.
Our tool makes it easy for data owners to investigate the value of their data, choose the right mechanism and tune its
parameters to achieve a good utility-privacy trade-off.


### Features of *Privacy Tuna*

- Visualize trajectory data and visually compare raw and protected data
- Understand and estimate the risks from potential privacy leakage in the data
- Find a suitable privacy-preserving mechanism that prevents information leakage
- Measure the utility of the data to understand its value
- Tune the parameters of privacy-preserving mechanisms to achieve a good balance between utility and privacy

More information can be found [here](resources/Schneider_Privacy_Tuna_20221209.pdf).


### Demonstrator & Video
<img src="resources/fig6.png" alt="" width="900"/>

You can try out our demonstrator [here](https://livinglab.scadsai.uni-leipzig.de/privacy-tuna/).
It includes a few routes from Porto Taxi dataset [[1](resources/D_TOUR_Schneider.pdf)], 
consisting of cab rides in Porto, Portugal. The dataset can be found [here](resources/porto_taxi_dataset_small.csv).
To get a quick overview over the features and how to use *Privacy Tuna*, take a look at the 
<a href="https://cloud.scadsai.uni-leipzig.de/index.php/s/snTpZd7o4NCS5rB" target="_blank">demonstration video</a>.


### Usage
- Flask backend is available at https://github.com/majaschneider/privacytuna-services
- SpringBoot backend and database are available at https://github.com/majaschneider/privacytuna-backend
- Angular Frontend is available at https://github.com/majaschneider/privacytuna-frontend


### License
*Privacy Tuna* is licensed under [Apache License, Version 2.0](LICENSE)


### Acknowledgement
*Privacy Tuna* is developed by University of Leipzig & ScaDS.AI Dresden/Leipzig, Germany partially funded by the 
German Federal Ministry of Education and Research under grant DE4L 01MD19008D and ScaDS.AI Dresden/Leipzig 01IS18026B.


### Software Stack
*Privacy Tuna* uses the following software stack:
- Flask (https://flask.palletsprojects.com/en/2.2.x/)
- SpringBoot (https://spring.io)
- Angular (https://angular.io)
- Leaflet (https://leafletjs.com)
- PostgreSQL (https://www.postgresql.org)
- PostGIS (https://postgis.net)
- KeyCloak (https://www.keycloak.org)


### References
[[1]](resources/D_TOUR_Schneider.pdf) Schneider et al. (2022), D-TOUR : Detour-based point of interest detection in privacy-sensitive trajectories