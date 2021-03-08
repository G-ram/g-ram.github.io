---
permalink: /
title: ""
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

# [Research](#research)
I am primarily interested in improving the energy-efficiency of low-power computers and the applications that such compute devices enable. Low and ultra-low-power sensor devices enable many new applications. These include in- and on- body medical implants, wildlife monitoring, tiny satellites, and civil infrastructure monitoring. Energy-efficiency is the key determinant for how deployed devices in these applications will perform: for devices powered by batteries, energy efficiency determines the lifetime of the device and for devices sourcing energy harvested from the environment, energy efficiency determines which applications are feasible and the duty cycle (how long it takes to recharge) of the device. 

Commercially-available off-the-shelf systems in this domain are not energy-efficient and are severely resource constrained, often possessing mere kilobytes of main memory. Unfortunately, offloading computation from a sensor device to a more powerful edge device or to the cloud is infeasible or impractical because communication is vastly more expensive than computation. These problems lead to two directions of research: first, designing intelligent applications that can make decisions on the devices, but do not require significant resources, and second, designing new, more energy-efficient computer architectures to better support these new classes of applications.

Please refer to my publications as well as [intermittent.systems](http://www.intermittent.systems/) and [cmu-corgi](https://cmu-corgi.github.io/) for more information.

### Ultra-low-power CGRA generation framework and architecture (SNAFU)
- Paper: To appear at ISCA'48

### Ultra-low-power vector-datflow architecture (MANIC)
<figure style="float:left;max-width:250px;margin:0px;">
	<img align="left" src="/files/manic.png" style="padding:0.4em;margin:0px;">
	<figcaption style="padding-left:0.4em;font-weight: bold;">MANIC Silicon - fabbed 2021</figcaption>
</figure>
Commercially-available off-the-shelf microcontrollers are energy-inefficient. Instruction supply energy and data supply energy (RF accesses) are two primary sources of energy-inefficiency. Vector execution is one way to improve energy-efficiency by amortizing instruction fetch and decode. However, traditional vector architectures require a vector register file with expensive access energy. We introduce MANIC, a loosely-coupled vector co-processor that implements a new execution model called vector-dataflow execution. Vector-dataflow execution eliminates the majority of vector register file accesses by identifying opportunities for dataflow and forwarding values from producers to consumers. In typical vector execution, control completes an entire instruction’s worth of computation before moving onto the subsequent instruction. MANIC flips this around. MANIC considers a collection of instructions at once, exposing opportunities for dataflow. In vector-dataflow execution, control transfers executes the first elements of the instructions*, then the second elements, then the third and so on. 

In 2021, we fabricated MANIC in a sub-28nm, ultra-low-power commercial process. Verification of the chip is ongoing, but initial results are promising.  
- Paper: [https://dl.acm.org/doi/10.1145/3352460.3358277](https://dl.acm.org/doi/10.1145/3352460.3358277)

### Inference on Intermittent Embedded Systems (GENESYS, SONIC, TAILS)
Continuous streaming of raw sensor data from a node to a central hub is inpractical for an intermittent device because communication is expensive and oftentimes infeasible. Thus, it is important to make the most out of any opportunity to communicate. Machine learning allows us to effectively determine whether sensor data is relevant and should or should not be transmitted. SONIC and TAILS are two runtime systems that make inference on intermittent devices correct and efficient. SONIC is entirely software-based, while TAILS relies upon hardware acceleration available on a variety of new MCUs. A paper summarizing these systems appearred at ASPLOS'19.
- Paper: [https://dl.acm.org/citation.cfm?id=3304011](https://dl.acm.org/citation.cfm?id=3304011)
- Github: [https://github.com/CMUAbstract/SONIC](https://github.com/CMUAbstract/SONIC)

# Fellowships/Awards
### Apple Scholar in AI/ML
Prestigious 2-year fellowship awarded by Apple to twelve PhD students globally. Fellowship was awarded in recognition of work on on-device machine-learning. Please see [ml@apple](https://machinelearning.apple.com/updates/introducing-apple-scholars-aiml) for more information.


# [Publications](#publications)
1. *SNAFU: An Ultra-Low-Power, Energy-Minimal CGRA-Generation Framework and Architecture*
Graham Gobieski, Oguz Atli, Ken Mai, Brandon Lucia, Nathan Beckmann  
*To appear at ISCA'48*
2. *MANIC: A Vector-Dataflow Architecture for Ultra-Low-Power Embedded Systems*
Graham Gobieski, Amolak Nagi, Nathan Serafin, Mehmet Meric Isgenc, Nathan Beckmann, Brandon Lucia  
[[paper]](https://dl.acm.org/doi/10.1145/3352460.3358277)
3. *Intelligence Beyond the Edge: Inference on Intermittent Embedded Systems*  
Graham Gobieski, Brandon Lucia, and Nathan Beckmann. ASPLOS'19.  
[[paper]](https://dl.acm.org/citation.cfm?id=3304011) [[ArXiv]](https://arxiv.org/abs/1810.07751)
4. *Intermittent Deep Neural Network Inference*  
Graham Gobieski, Nathan Beckmann, and Brandon Lucia. SysML'18.  
[[paper]](http://www.cs.cmu.edu/~beckmann/publications/papers/2018.sysml.sonic.pdf)
5. *Shuffler: Fast and Deployable Continuous Code Re-Randomization*  
David Williams-King, Graham Gobieski, Kent Williams-King, James P Blake, Xinhao Yuan, Patrick Colp, Michelle Zheng, Vasileios P Kemerlis, Junfeng Yang, William Aiello  
[[paper]](https://www.usenix.org/system/files/conference/osdi16/osdi16-williams-king.pdf)
6. *Clickable poly (ionic liquids): A materials platform for transfection*  
Jessica Freyer, Spencer Brucks, Graham Gobieski, Sebastian Russell, Carrie Yozwiak, Mengzhen Sun, Zhixing Chen, Yivan Jiang, Jeffrey Bandar, Brent Stockwell, Tristan Lambert, Luis Campos  
[[paper]](https://pdfs.semanticscholar.org/9c16/8b43d6ebe66e1c3e4c4a993dddd56594309b.pdf)

