---
permalink: /
title: "About"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

# [Research](#research)
My primary focus of research is new architectures for energy-harvesting, intermittent devices. Intermittent computing has increasingly become a popular domain because many environments contain no stable power source or the conditions do not accommodate a battery. These might include sensor nodes embedded in the body, deep in the ocean, or in space. Traditional programming models and architectures, however, are not necessarily applicable to the domain of intermittent computing. Moreover, since communcation is so expensive, sensor nodes require additional intelligence so as to maximize efficiency. In the past, there has been much work on using software solutions that reduce programming complexity and ensure correct execution. However, microarchitectural solutions have mostly been overlooked. As the Internet of Things becomes more important and machine learning on embedded devices becomes more feasible, new emerging architectures for intermittent devices will become increasingly relevant. Please refer to [intermittent.systems](http://www.intermittent.systems/) for more information.

### Intermittent Parallel Architecture
We seek to design from the ground-up an MCU that takes into account all of the challenges of intermittent computing as well as the computational requirements of emerging applications. Specifically, the memory system can be designed to make checkpointing more efficient, the core pipeline can be designed to leverage SIMD, and the software runtime system can be co-designed with the hardware to maximize performance per joule.

### Inference on Intermittent Embedded Systems
Continuous streaming of raw sensor data from a node to a central hub is inpractical for an intermittent device because communication is expensive and oftentimes infeasible. Thus, it is important to make the most out of any opportunity to communicate. Machine learning allows us to effectively determine whether sensor data is relevant and should or should not be transmitted. SONIC and TAILS are two runtime systems that make inference on intermittent devices correct and efficient. SONIC is entirely software-based, while TAILS relies upon hardware acceleration available on a variety of new MCUs. A paper summarizing these systems will appear at ASPLOS'19.
- ArXiv: [https://arxiv.org/abs/1810.07751](https://arxiv.org/abs/1810.07751)
- Github: [https://github.com/CMUAbstract/SONIC](https://github.com/CMUAbstract/SONIC)


# [Publications](#publications)
1. *Intelligence Beyond the Edge: Inference on Intermittent Embedded Systems*  
Graham Gobieski, Brandon Lucia, and Nathan Beckmann. ASPLOS'19.  
[[paper]](https://arxiv.org/abs/1810.07751)
2. *Intermittent Deep Neural Network Inference*  
Graham Gobieski, Nathan Beckmann, and Brandon Lucia. SysML'18.  
[[paper]](http://www.cs.cmu.edu/~beckmann/publications/papers/2018.sysml.sonic.pdf)
3. *Shuffler: Fast and Deployable Continuous Code Re-Randomization*  
David Williams-King, Graham Gobieski, Kent Williams-King, James P Blake, Xinhao Yuan, Patrick Colp, Michelle Zheng, Vasileios P Kemerlis, Junfeng Yang, William Aiello
[[paper]](https://www.usenix.org/system/files/conference/osdi16/osdi16-williams-king.pdf)
4. *Clickable poly (ionic liquids): A materials platform for transfection*  
Jessica Freyer, Spencer Brucks, Graham Gobieski, Sebastian Russell, Carrie Yozwiak, Mengzhen Sun, Zhixing Chen, Yivan Jiang, Jeffrey Bandar, Brent Stockwell, Tristan Lambert, Luis Campos  
[[paper]](https://pdfs.semanticscholar.org/9c16/8b43d6ebe66e1c3e4c4a993dddd56594309b.pdf)

