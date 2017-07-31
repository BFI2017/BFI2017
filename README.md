# SourceCodeOfBFI
  Networking (SDN), which separates the control plane and data plane, is a promising new network architecture for the Future Internet. OpenFlow is the de facto standard which defines the communication protocol between the controller and switches. The most challenging issue in OpenFlow switches is the lookup of multiple OpenFlow tables. The lookup of OpenFlow tables is so complicated that the state-of-the-art research are still focusing on the design of lookup pipeline architecture, and there is no specific algorithm for the lookup of OpenFlow tables.
  In this paper, we revise the long-pipeline architecture of OpenFlow 1.4 to a 5-stage pipeline architecture to make a tradeoff between flexibility and implementability, and decompose the lookup of OpenFlow tables into three kinds of lookup: longest prefix matching (IP lookup), multi-field matching (packet classification), and exact matching. Then we design new algorithms for packet classification, because the state-of-the-art solutions for them seldom support fast update which is highly demanding for OpenFlow. The other two kinds of lookups can be well handled by state-of-the-art. Experimental results show that our proposed algorithms work excellently, and outperform state-of-the-art solutions. We have released the source code of our algorithms and the data set used in our experiments at Github, and carefully removed the identity information.
