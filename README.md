Abstract
In this study, we analyzed the actors network that we constructed from the data of the cinema websites by using complex network analysis techniques. After the construction bipartite actor-film relationship network, we constructed an actor-actor network via one-mode projection. We performed an exploratory complex network analysis on these networks. We have created two different networks which are past date and present date, reflecting the role mate relationships between the actors. When we examined these networks, we observed that actors relationships in the past were more intense, while actors relationships today were less intense. We also performed community analysis and other graph metrics.

1.	Introduction
Turkish cinema is an important part of Turkish culture and has been improved over the years. "Yeşilçam" is the unforgettable period of Cinema of Turkey. "Yeşilçam" is the unforgettable period of Cinema of Turkey. Yeşilçam is named after Yeşilçam Street in the Beyoğlu district of Istanbul where many actors, directors, crew members and studios were based. Yeşilçam period covers the years when Turkish cinema was most active. Yeşilçam experienced its heyday from the 1970s to the 1990s, when it produced 250 to 350 films annually. That period, there was no internet in our lives, the number of channels on TV was limited, the entertainment industry was not as developed as it is now. This situation enabled the development of the cinema industry. There are movies of all kinds in this period. A great number of theater comedies, village films about blood feuds, and love and honor films were shot. There are most famous actors cinema of Turkey in this period. Kemal Sunal and Cuneyt Arkin have been important names in the history of cinema. Today, their movies are still watched on TVs. 
Nowadays, the technical level of the Turkish films has reached world standards, and educated young people from cinema schools have started to dominate the cinema. The budgets of Turkish films have begun to reach million dollars, and the audience numbers to million. In recent years, the number of audiences and films, international awards, film export and diversity in production have been increased.
Comedy films have an important place in Yeşilçam period and today's Turkish cinema. It is one of the most popular genres for audiences of all ages.
When we examined the films of comedy type in Yeşilçam period and today, we noticed that there is a relationship between actors which are role mates. Similarly, an actor is linked to one or more films but not any actors. A group of actors is determined for films, first. Each actor is linked to the film or films he plays. A network between actors has been created using this connection.  When we look at the network in detail, we can get the role mates between the actors, and when we look in general, we can get many statistics on the network, such as popularity, centrality, density etc. 
Complex networks have been an active subject studied for more than two decades by network researchers from diverse fields including mathematics, physics, statistics, biology, computer science, and sociology.
In this study, we used complex network analysis tools and techniques to discover and analyze groups of actors by history. These are:
•	between 1970 and 1989 films
•	2018 and 2019 films
We obtained two networks and made inferences by evaluating these networks comparatively. 

2.	Data Collection
The data used in this study were obtained collecting manually from the "http://www.beyazperde.com/" website. The films and actors collected to a list of python variable. 
Sample list :
milyarder = ['Şener Şen', 'Uğur Yücel', 'Tulug Çizgen', 'Adile Naşit', 'Bilge Zobu', 'İhsan Yüce']

Later, the lists of movies were merged and converted to matrix format. Small pieces of code were written to create node and edge lists from the combined film lists. Node lists are consist of actors, and edge lists are consist of role mates. Node and Edge lists need to be converted to csv format for network visualization and statistic in Gephi. Thus, The Gephi program allows us to import nodes and edges easily. After consisting of nodes and edges in code, the data saved in CSV file format to desktop with using "csv" library. Then the saved file can be imported to Gephi.


3.	Visual Analysis
	Numerical metrics contain useful information in the network structure. However, visual analysis of the network structure is very important to see the overall structure of the network to explore the network and make inferences. We wanted to explore the relations between the actors from the past to the present by forming two networks. Then, we created "Actors playing in 1970-1989 Turkish Films Network" and "Actors playing in 2018 and 2019 Turkish Films Network". When we first look at the "Actors playing in 1970-1989 Turkish Films" graph, we see a highly centralized network. It means that at that time the same actors played together in many movies. Centralization is less in the "Actors playing in 2018 and 2019 Turkish Films" graph. Because today there are many actors in the film industry and they take part in different movies.

Centrality defines how important a node is in the network.
Table 1: Topological measures of the "Actors playing in 1970-1989 Turkish Films Network" and "Actors playing in 2018 and 2019 Turkish Films Network"
	Actors playing in 1970-1989 Turkish Films Network	Actors playing in 2018 and 2019 Turkish Films Network
Nodes	424	894
Edges	5464	6086
Clustering Coefficient	0,743	0,887
Avg. Path Length	2,273	3,645
Density	0,061	0,015
Avg. Weighted Degree	25,774	13,613
Diameter	5	7


4.	Centrality Analysis

Centrality defines how important a node is in the network.


Rank	Actor	Degree
1	Kemal Sunal	230
2	Ali Şen	159
3	İhsan Yüce	157
4	Kenan Fosforoğlu	128
5	Cevat Kurtuluş	118
6	Adile Naşit	116
7	Hulusi Kentmen	113
8	Ayşen Gruda	106
9	Ahmet Turgutlu	102
10	Reha Yurdakul	102
Rank	Actor	Degree
1	Sinan Bengier	64
2	Erkan Can	52
3	Ali Rıza Tanyeli	51
4	Uraz Kaygılaroğlu	50
5	Toygan Avanoğlu	48
6	Şafak Sezer	48
7	Esra Sönmezer	47
8	Çetin Altay	45
9	Ayhan Taş	44
10	Doğa Konakoğlu	43









The most important top 10 actors are listed tables.




Rank	Actor	Closeness
1	Kemal Sunal	0.68336
2	Hakkı Kıvanç	0.604286
3	Ali Şen	0.59915
4	İhsan Yüce	0.584254
5	Kenan Fosforoğlu	0.582645
6	Adile Naşit	0.573171
7	Hulisi Kentment	0.568548
8	Ayşen Gruda	0.563249
9	Reha Yurdakul	0.556579
10	Cevat Kurtuluş	0.547927
Rank	Actor	Closeness
1	Haydar Zeytünlü	1.0
2	Furkan Tezcan	1.0
3	Turgut Güneş	1.0
4	Kenan Balık	1.0
5	Belit Şentürk	1.0
6	Soner Karakuş	1.0
7	İlker Su Osmanoğlu	1.0
8	İsmail Suat Tuzlu	1.0
9	Onur Dilber	1.0
10	Ümit İbrahim Kantarcılar	1.0









It shows how close a node is to other nodes in the network.

Rank	Actor	Betweeness
1	Kemal Sunal	18.019.928.063
2	Hakkı Kıvanç	5.166.679.114
3	Ali Şen	489.537.055
4	İhsan Yüce	4.313.887.417
5	Adile Naşit	3.485.292.869
6	Adile Naşit	3.485.292.869
7	Kenan Fosforoğlu	3.404.810.626
8	Şener Şen	3.316.437.708
9	Ayşen Gruda	2.998.061.157
10	Cevat Kurtuluş	2.908.009.971

Rank	Actor	Betweenness
1	Sinan Bengier	3.095.360.923.760.080
2	Ayhan Taş	282.807.558.012.078
3	Ali Rıza Tanyeli	2.442.127.560.650.060
4	Toygan Avanoğlu	23.761.263.320.020.700
5	Şafak Sezer	1.923.785.688.019.550
6	Bengi İdil Uras	18.994.663.355.012.100
7	HÜseyin Elmalıpınar	18.394.811.316.535.100
8	Erkan Can	16.377.079.478.664.600
9	Esin Civangil	16.319.807.683.428.500
10	Uraz Kaygılaroğlu	16.195.834.826.549.500


It is about a node being located on the shortest paths between other nodes.

5.	Structural Analysis
	In this section, the networks are evaluated as a whole, various criteria are applied and analyzed. 

Reciprocity: Reciprocity is a measure of whether the connections between nodes are bi-directional. It can analysis only in directional networks. In this study, the networks are undirectional. Thus, the reciprocity cannot apply here.

Average Degree: It is one of the criteria that defines the general structure of a network in degrees.
Average Degree of Actors playing in 1970-1989 Turkish Films Network:
(2*5464) / 424 = 25.77
Average Degree of Actors playing in 2018 and 2019 Turkish Films Network:
(2*6086) / 894 = 13.61
Degree Distribution: It describes how many nodes with what degree there are in the network. It is used to understand the characteristic structure of the network.


Density: It is a measure of how connected a network is.

(424*421) / 2 = 89.252 number of maximum edges
5464 / 89.252 = 0.061

(894*893) / 2 = 399.171 number of maximum edges
6086 / 399.171 = 0.015


