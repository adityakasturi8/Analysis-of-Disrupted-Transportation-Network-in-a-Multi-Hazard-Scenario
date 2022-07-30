# Analysis of Disrupted Transportation Network in Multi-Hazard Scenario

## Author
__Aditya Kasturi__ 

## Acknowldgement
 
### 1.	INTRODUCTION

Community resilience is a measure of a community's long-term capacity to adapt to, withstand, and recover from adversity. In order to fully understand how physical, economic, and social infrastructure systems within a community interact to drive recovery efforts, specialists from multiple disciplines should collaborate to perform rigorous simulations. The Center for Risk-Based Community Resilience Planning is unique because it integrates engineering, social sciences, and economics to model community resilience holistically(Center for Risk-Based Community Resilience Planning, n.d.).

A nexus between social and technological infrastructure networks will bridge the gap between engineering and social science aspects of resilience planning. This will facilitate risk communication between stakeholders and community resilience. Technologies, financial, social, and political support, healthcare delivery, education, and public administration are being integrated into the model to promote recovery and vitality in a community. The Center's work will lead to quantitative and scientific measurement of community resilience. The result will increase community resilience to disasters by supporting a business case(Center for Risk-Based Community Resilience Planning, n.d.).

The Center's work at the University of Oklahoma for Community Resilience, known as OU Community Resilience CORE Lab, is managed by Dr. Charles D. Nicholson (Associate Professor in the School of Industrial and Systems Engineering) and Dr. Andres Gonzalez (Assistant Professor in the School of Industrial and System Engineering). The Community Resilience OU CORE Lab is active in working on Data Science and Analytics with the main focus of interest is to enhance the technical aspects of Risk-Based Community Resilience Planning during natural hazards and disruptive events through analysis of complex independent networks, predictive modeling, prescriptive research, Optimization, Machine Learning, and Network Analysis for both mitigation and recovery on various testbeds such as Memphis Metropolitan Statistical Area (MMSA), Joplin, Lamberton, Seaside, etc. 

Community resilience has arisen to reduce direct and indirect costs associated with natural, technological, and human-caused hazard occurrences. There is still a need for more guidance on how to prepare for and implement steps to promote community resilience, as well as science-based tools to quantify resilience and enable the evaluation of different resilience methods. The National Institute of Standards and Technology (NIST) program is developing science-based tools and metrics to support and measure resilience at the community scale, as well as economic evaluation of alternative solutions to improve resilience, engaging community resilience stakeholders for input and feedback on products such as guidance, tools, and metrics for planning and implementing resilience measures, and conducting disaster and failure studies (DFS)(Community Resilience Program | NIST, n.d.).

Networks are everywhere and are used to identify a collection of connected objects. We refer to the objects as nodes or vertices and usually draw them as points. Networks often referred to as graphs are extracted from the mathematical study of graph theory. 

![image](https://user-images.githubusercontent.com/95768375/181947051-b226fb71-7e55-485d-835a-f48b09144512.png)
Fig: Basic Network with nodes and edges

The ability of a system to tolerate or adapt to external shocks and recover from such shocks efficiently and effectively is referred to as its resilience. In resilience, Networks are beneficial on the broader spectrum, such as Societal Resilience, Community Resilience, Supply Chain Resilience, Organizational Resilience, etc.

As the project focuses on Community Resilience, There are four methodologies that are followed in community resilience, and they are as follows:
![image](https://user-images.githubusercontent.com/95768375/181947325-ca52c8f8-b6ab-4d45-adf6-340f9de56ca8.png)
![image](https://user-images.githubusercontent.com/95768375/181947375-049b2e49-9d75-4e5c-a249-f8451d550835.png)
Fig: Illustration of the concept of resilience and the effect of the risk mitigation plan


__Robustness:__ When the system is robust, it is able to withstand extreme events and continue to provide a certain level of service even after the incident.
__Rapidity:__ The ability to get back to the desired functionality as quickly as possible. 
__Redundancy:__ The ability to replace elements and components of a system. 
__Resourcefulness:__ When faced with the effects of extreme events, resourcefulness plays a vital role in the cap city's identifying, prioritizing, and mobilizing personnel and financial resources essentially.

__Transportation networks__ are networks or graphs in geographic space describing infrastructures that allow and restrict movement or Flow. Network Analysis is a type of proximity analysis that is extracted from graph theory that involves digital representations of networks, such as roads, power lines, pipelines, etc. Transportation networks can be of different types, such as Air networks, Maritime networks, Road networks, Rail networks, Power Grids, etc. 

Transportation networks in community resilience are critical to a community's economic and social well-being, and the status of such networks following the occurrence of an extreme hazard is vital. (For example, earthquakes, severe windstorms, flooding, terrorism, etc.) a substantial impact on the community's recovery Highway Bridges are weak points in the road transportation system. as well as the transportation network's resilience and recovery; their performance has a significant impact on the organization.

This project contributes toward Network Analysis on the Transportation (Road) Network of Seaside testbed to support identifying roads, buildings, and emergency locations to support the process of mitigation and restoration during a natural hazard or disaster.

### 2.	OBJECTIVE

As modern societies have become increasingly reliant on surface transportation networks, the need to protect these networks from disasters has become more important. Transportation infrastructure is one of sixteen critical infrastructure systems that the U.S. Department of Homeland Security has identified as being crucial to the health of contemporary societies. There are many risks that can affect transportation networks, including natural disasters, accidents, and deliberate attacks. Transport network disruptions can have serious repercussions, including societal upheaval, economic harm, and fatalities.

In the paper written by Weili Zhang, Naiyu Wang, and Charles Nicholson (Zhang et al., 2017) and Weili Zhang and Naiyu Wang(Zhang & Wang, 2016), a powerful metric known as Independent Pathway (IPW) is introduced where IPW is the two pathways between the exact Origin and Destination pair are considered as IPW if they do not share any standard road links(Zhang & Wang, 2016). The papers describe solving a multi-objective optimization model for mitigation and recovery of a community resilience based on a transportation network. In the paper, the authors used the shortest path as an approach and applied it to virtually/imaginative generated data with 30 nodes and 35 bridges. The fitness function took 30 minutes to iterate through the process. This methodology is inefficient for the metaheuristics framework as the execution time for the real-world data is very high and time-consuming. 

The Goal of this project is to create an efficient way of computing the independent pathways (IPW) to work as a fitness function for a metaheuristic to support a prescriptive analytics framework. The analysis will make use of recent developments in network theory based on NetworkX(A Network Analysis Python Package) to understand and measure the network connectivity of the Seaside testbed of the Road transportation network. This metric, referred to as the IPW (Independent PathWays(Zhang & Wang, 2016)), will take into account the network topology, redundancy level, emergency nodes, structural reliability of network components

Note: A detailed description of IPW is mentioned in the Methodology section of this document.

	
### 3.	DATA

A Center of Excellence for Risked-Based Community Resilience Planning (CoE) was established by the National Institute of Standards and Technology (NIST) to develop measurement science to support community resilience assessments. The Independent Networked Community Resilience Modeling Environment (IN-CORE) platform is used to implement measurement science. IN-CORE enables quantitative comparisons of alternative resilience strategies by incorporating risk-based decision-making technologies. IN-CORE allows community-based data to be seamlessly integrated, facilitating planning and intelligent post-disaster recovery strategies based on models that include interdependent physical and socio-economic systems based on physics that are developed for community disaster resilience(IN-CORE, n.d.).

![image](https://user-images.githubusercontent.com/95768375/181948900-e0eaac5e-2405-4490-881f-1d61aa795e62.png)
Fig: IN-CORE Platform Usage

The Dataset of the Seaside Testbed was acquired from the INCORE Platform. As a student for the Community Resilience CORE Lab, I was given exclusive access to the INCORE platform and to INCORE Cloud, where most of the data is stored and constantly updated daily.

Therefore, All the members working on the data can access it. The obstacle I faced was to get access to the INCORE platform essentially as there is clear documentation and demonstration on a certain way to get access to it.

The Seaside Transportation Network Testbed Data set contains 585 rows and 14 features. The Dataset is as follows:

![image](https://user-images.githubusercontent.com/95768375/181949185-eb319b70-6fe2-419a-8f45-ef8d7bb36dc2.png)
Fig: Dataset of the Seaside Testbed with 585 rows and 14 columns

![image](https://user-images.githubusercontent.com/95768375/181949850-c4bdbd73-3da0-4d1e-aba1-6f9d0ea9396a.png)
The above represents the information about the 14 features of the Dataset of the Seaside testbed.
The Dataset contains the nodes based on their geographical location and the distance between each of the nodes. For example, when you look at row 2, by looking at the start node and end node, we can determine that node 300 is connected to node 316, and the distance between these two nodes can be seen from the column 'length', which is 383.083680.

To illustrate, understand and visualize the data and perform network analysis on the data, Python Programming packages such as Geopandas, Momepy, and NetworkX have been used for this project. GeoPandas provides a high-level interface to shapely and pandas for working with geospatial data. It merges the functionality of the two libraries to make working with geospatial data simple and intuitive(GeoPandas 0.11.0 — GeoPandas). NetworkX is Python's graph-theory package and is mainly used to study the mathematical principles of complex networks(NetworkX — NetworkX Documentation, n.d.). Momepy is a Python library for quantitative analysis of urban forms such as urban morphometrics. Momepy is part of PySAL (Python Spatial Analysis Library) and is built on top of GeoPandas, and other PySAL(Momepy Documentation — Momepy 0.5.3 Documentation, n.d.). Momepy is a package that helps to convert data points from Geopandas to Networkx to perform network-based analysis. 


![image](https://user-images.githubusercontent.com/95768375/181950112-41cb1eb9-bc94-47d9-8212-7ffa7ecfd469.png)
Fig: Converted Dataset of the Seaside Testbed to work on Geopandas Dataframe

![image](https://user-images.githubusercontent.com/95768375/181950237-17a62c80-98c6-441e-a25c-49bafe464b68.png)
Fig: Original Map of the Seaside Testbed without any Implementation

![image](https://user-images.githubusercontent.com/95768375/181950350-88f766a6-5d7d-412d-b525-34b1b48fee50.png)
Fig: Implementation of Linestrings on Seaside Map using GeoPandas



The Geopandas implementation of the Seaside transportation network, which contains all the roads and bridges which are connected in the Dataset. .  This Visualization of the transportation network on the real map helped in understanding how the seaside data looks and how every street is connected in the map. It also shows the important places such as fire stations and hospitals which are vital to know as they are one of the evacuation points during a hazardous situation according to the transportation network problem, which is implemented in the methodology section of this report. An Example of a Fire station and Hospital from the Seaside Testbed is shown below.


![image](https://user-images.githubusercontent.com/95768375/181950649-77f729b9-85ca-4c69-be38-1e7ca3da1ea0.png)
![image](https://user-images.githubusercontent.com/95768375/181950715-aba49108-1fe5-486d-a6a6-159be15b2146.png)
Fig: Representation of Emergency Locations in the Seaside Testbed using GeoPandas


Using Momepy and Matplotlib Library, I have plotted the nodes to specifically understand how the Network is divided; is it either by the community or by street, etc. 

![image](https://user-images.githubusercontent.com/95768375/181950848-7b69673d-bfa9-47d7-bbde-0a56ae3c4b41.png)
Fig: Original Seaside Testbed vs. Nodes Plotted Testbed using Momepy and NetworkX

Based on the above node point representation, each node represents the starting and ending points of a street, with a few nodes representing the bridges. 

![image](https://user-images.githubusercontent.com/95768375/181951016-5755cbcd-659e-4c0b-a231-e936ed430913.png)
Fig: Represents the Original graph vs. Primal Graph vs. Overlay graph

The image above depicts the initial map of the Seaside Testbed retrieved from Open Street Map, followed by the Primal Graph drawn using the Momepy and NetworkX, and finally the final map. The final image shows a street overlay over a primordial graph to show how closely the original map and created network graph are connected. We can plainly detect a minor divergence of the geographical spots in the Overlay image. However, the majority of the points are correctly labeled and plotted.

### 4.	METHODOLOGY

__i.	Techniques__ 

__Background Information of the Problem:__

In the paper written by Weili Zhang, Naiyu Wang, and Charles Nicholson (Zhang et al., 2017) and Weili Zhang and  Naiyu Wang(Zhang & Wang, 2016), a powerful metric known as Independent Pathway (IPW) was introduced. The papers describe solving a Multi-objective optimization model for mitigation and recovery of a community resilience based on a transportation network. 

In the paper, the authors used the shortest path as an approach along with the Dijkstra algorithm and applied it to virtually/imaginative generated data with 30 nodes and 35 bridges. The fitness function (objective function) took 30 minutes to iterate through the process.

This methodology is inefficient for the metaheuristics framework as the execution time for the real-world data is very high and time-consuming. To mitigate this problem, In this project, I am re-initiating independent Pathways (IPW) but using the Maximum Flow algorithm. 

To better understand the Independent Pathways, we should first understand the All Pathways. 
__All Pathways (APW):__ 
The Number of All Pathways is likely to be very large between complex nodes; when a large number of pathways all share a common link, the number of APWs between an origin-destination pair can be overly sensitive to the damage to the commonly shared links. This is considered an NP-Hard problem.

To avoid calculating all the paths, we re-initiate the already created metric called Independent Pathways (Zhang & Wang, 2016) for this problem. 

__Independent Pathway(IPW):__ 
Two pathways between the same Origin and Destination pair are considered Independent Pathways (IPW) if they do not share any common link. 

![image](https://user-images.githubusercontent.com/95768375/181951993-3a44897e-f552-40f2-9cce-8af6d1ea1caf.png)
Fig: Example Node and Edge Representation to understand IPW

__For Example:__ In the above figure illustrates a basic example of a network. Assuming, Node 6 is the Source node and Node 4 is the Sink node. We calculate the independent pathways such that they do not share any common edges. From the above example, you can see that node 6 is connected to Nodes 3, 4, 7, and 9. And to Reach Node 4, there are 4 ways. {6 – 3 – 4 }, {6 – 4 },  {6 – 7 – 4} , {6 – 9 – 7 – 4} 
Case I : If we use the shortest path method to find the IPW we get the following:
			{6 – 3 – 4 }, {6 – 4 },  {6 – 7 – 4}
Case II : If we use the maximum flow method to find the IPW we get the following: 
			{6 – 3 – 4 }, {6 – 4 }, {6 – 9 – 7 – 4}

We are not considering the nodes which are not mentioned above for Case I: {6 – 9 – 7 – 4} and Case II: {6 – 7 – 4}, as they share a common link with the other with Node 7. 

Finding APW between two nodes is NP-Hard, and, therefore, impractical for decision-making practice. On the other hand, the technique of IPW for the same or different origin-destination pair may not have identical impacts on the network performance. 
				
				IPW = Max Pk (i,j) 
					Or
				IPW = Max Flow Pk(i,j) with capacity = 1

Each Pk (I,j) usually consists of several edges (links) connected in a series. This method is inversely proportional to the shortest distance from node i. 

We use Independent Pathways to efficiently find the independent networks, which helps improve the network efficiency and helps to measure the network performance capacity to identify the edges that are more likely to be destroyed in a disaster. 

__ii.	Procedures__

We achieve the technique to re-initiate the Independent Pathways in our problem using the Maximum Flow Algorithm. 
Maximum Flow Algorithm: According to graph theory, a flow network with a source(s), sink(t), and multiple edges have individual capacities that determine how much Flow they can accommodate. Identifying the maximum flow problem can be accomplished by multiple algorithms. The three most recommended algorithms for calculating the maximum Flow are Ford-Fulkerson, Dinic's, and Edmond Karp. 

![image](https://user-images.githubusercontent.com/95768375/181952916-0e92c2c0-c9c7-4ff9-9013-90b6ab5092f7.png)
Fig: Maximum Flow Optimization Model 

In this project, different types of maximum flow algorithms are used in NetworkX to find the best efficient algorithm to find the independent pathways, and they are as follows:

__Maximum Flow using Preflow_push:__ With this technique, Flow is pushed locally across nearby nodes and gradually becomes a maximum flow as a result of an acceptable network monitored by relabeling operations. This technique has a global augmentation to achieve maximum Flow. This algorithm has a running time of O(n2m) for n nodes and m edges.

__Edmond Karp maximum flow:__ The main difference between Ford- the Fulkerson algorithm and the Edmonds-Karp algorithm is that Ford-Fulkerson uses the DFS (Depth First Search) technique while Edmond-Karp uses the BFS technique. This algorithm has a running time of O(nm2) for n nodes and m edges.

__Dinic's algorithm:__ It is similar to Edmond Karp's maximum Flow; however, it includes concepts of the level graph and blocking Flow to achieve its performance. The algorithm has a running time of O(n2m) for n nodes and m edges

We can implement the independent pathways for all the pairs of nodes using all pair's maximum flow algorithm with the edge capacity = 1, i.e., the Flow of the two nodes is 1. This can also be defined as the average of all pair's maximum Flow is equal to the Independent Pathways. 

Implementing the IPW using maximum Flow would undoubtedly increase the time efficiency by reducing the algorithm's total computation time. 

__5.	RESULTS AND ANALYSIS__

The WIPW, a quantitative resilience-based performance indicator built on graph theory, was developed in this study to assess the ability of the road network to perform in the face of hazardous natural hazard events. A vital measure is necessary given the effect that a working road network has on providing accessibility for the relief items to be transported to the impacted communities. The WIPW includes network topology, redundancy level, traffic patterns, the location of local emergency response facilities, and the likelihood that any one bridge will fail. The WIPW efficiently measures a network's ability to execute in the face of a potential hazard. The WIPW formulation's weighting mechanism for nodes and links provides a transparent framework for systematically and logically incorporating other significant network qualities to particular communities into resilience-based decision-making. The main objective is to calculate independent pathways (IPW) efficiently so they can be used to support a prescriptive analytics framework using metaheuristics. This Seaside Transportation Network Testbed Data set contains 585 rows and 14 features from the INCORE Platform, which acquired the Seaside Testbed Dataset.
They are tabulated below

![image](https://user-images.githubusercontent.com/95768375/181954479-7fbddabb-1668-4b84-bc72-a96856ad396c.png)



From the above table, we can clearly say that the Edmond Karps maximum flow algorithm works better than the other algorithms with an average Independent Pathways = 2.073661 with a total time execution of 366.38 seconds. 

A contrast in results can be seen from the original paper to the new algorithm generated. 
Original Results =  Shortest Path Problem + Dijkstra algorithm (Zhang & Wang, 2016)
Reproduced New results = Maximum Flow algorithm using  Edmond Karp Algorithm

![image](https://user-images.githubusercontent.com/95768375/181955118-acc506e2-5296-4d4d-b4c2-5970331514ff.png)


The primary Goal of this work is to come up with an objective function for the calculation of the IPW in order to be utilized in metaheuristic algorithms for large-scale instances.

### 6.	DELIVERABLES 

As a result of the results presented, decision-makers can decide on the resilience strategies associated with various hazard scenarios. Insurers and policymakers can use the approach presented to manage bridges against multiple hazards throughout their lifetimes.
Interdependencies and interactions between hazardous events should be considered in future studies. By incorporating intervention actions (e.g., inspection, maintenance, and repair) into the proposed framework, decision-makers can deliver the best solution.

### 7.	REFERENCES

Center for Risk-Based Community Resilience Planning. (n.d.). Retrieved June 28, 2022, from http://resilience.colostate.edu/
Community Resilience Program | NIST. (n.d.). Retrieved July 12, 2022, from https://www.nist.gov/programs-projects/community-resilience-program
GeoPandas 0.11.0 — GeoPandas 0.11.0+0.g1977b50.dirty documentation. (n.d.). Retrieved July 14, 2022, from https://geopandas.org/en/stable/
IN-CORE. (n.d.). Retrieved July 12, 2022, from https://incore.ncsa.illinois.edu/
momepy documentation — momepy 0.5.3 documentation. (n.d.). Retrieved July 14, 2022, from http://docs.momepy.org/en/stable/
NetworkX — NetworkX documentation. (n.d.). Retrieved July 14, 2022, from https://networkx.org/
Zhang, W., & Wang, N. (2016). Resilience-based risk mitigation for road networks. Structural Safety, 62, 57–65. https://doi.org/10.1016/j.strusafe.2016.06.003
Zhang, W., Wang, N., & Nicholson, C. (2017). Resilience-based post-disaster recovery strategies for road-bridge networks. Structure and Infrastructure Engineering, 13(11), 1404–1413. https://doi.org/10.1080/15732479.2016.1271813

### Acknowledgement
__Advisor__ : Charles D. Nicholson 
__Team__: Himadri Sen Gupta & Ahmad Ghasemkhani
