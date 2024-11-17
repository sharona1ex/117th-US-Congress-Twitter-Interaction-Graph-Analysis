<h1><center>117<sup>th</sup> US Congress Twitter Interaction Graph Analysis</center></h1>

**Objective:** The aim of this project is to derive a brief analysis of the 117th US Congress's twitter interactions using `PySpark` and `GraphFrames`. (source code: Social Network Analysis.ipynb)

**Dataset:** The dataset used is a network that represents the Twitter interaction network for the 117th United States Congress, both House of Representatives and Senate. [1] For the project, we are only using `congress_network_data.json` and `congress.edgelist` files to create the graph.

**Context:** The 117th United States Congress was a meeting of the legislative branch of the United States federal government, composed of the United States Senate and the United States House of Representatives. It convened in Washington, D.C., on January 3, 2021, during the final weeks of Donald Trump's first presidency and the first two years of Joe Biden's presidency and ended on January 3, 2023. [2]

**Analysis:**
1. `SpeakerPelosi` has the **highest outdegree (210)**, indicating that SpeakerPelosi is the most active in initiating interactions on Twitter. SpeakerPelosi **(aka Nancy Pelosi)** aligns with her role as Speaker of the House, a position that requires frequent communication.

2. `GOPLeader` (Kevin McCarthy) ranks high in both **outdegree (2nd, 157)** and **indegree (1st, 127)**. He's both active and frequently mentioned or interacted with by others. This reflects his position as the Republican leader in the House. (https://apnews.com/article/donald-trump-kevin-mccarthy-coronavirus-pandemic-9d801249ae7c642576a66a1ae2e3219a)

3. The `PageRank` results closely mirror the indegree rankings, with `GOPLeader, RepFranklin, and RepJeffDuncan` appearing in the **top 3** for both metrics. This suggests that these representatives are not only frequently mentioned but also occupy central positions in the network's information flow.

4. The `number of components` in this analysis is just one and it shows that each and every member is connected to one another directly or indirectly in the 117th US Congress.

5. Representatives like `RepFranklin, RepJeffDuncan, and RepJohnRose` appear prominently in indegree and PageRank metrics despite not being in top leadership positions. This could indicate that they are emerging influencers or particularly active in Twitter discussions.

6. The triangle count results provide insight into clustering within the network. `SpeakerPelosi` has the **highest triangle count (3281)**, followed by `GOPLeader` **(2777)**. This suggests that these leaders are part of many tightly connected groups, which could represent frequent collaborations or discussions among smaller groups of representatives.

<small> References:<br> [1] Stanford Network Analysis Project (SNAP). "Twitter Interaction Network for the 117th United States Congress." https://snap.stanford.edu<br> [2] Wikipedia contributors. (2023). "117th United States Congress." Wikipedia, The Free Encyclopedia. https://en.wikipedia.org/wiki/117th_United_States_Congress </small>
