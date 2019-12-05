---
layout: post
title:  "HOWTO: Build a modern workstation"
date:   2019-12-04 00:26:47 -0800
categories: hardware
---

Building a workstation is a rite of passage undertaken by almost all coders at some point or another. Many grad students in my department have also started building their own custom systems with beefy GPUs now that GPU computing has become the *de facto* platform for serious machine learning work; both my officemates built their own systems, for example. While building a computer from components can be a lot of fun, it can also be a daunting task for first-timers. In this post I'll outline the main steps to contructing a powerful, silent workstation, from component selection to assembly to troubleshooting.


## Selecting components
The necessary components to construct a workstation are a CPU, a motherboard, 1-4 sticks of RAM, a solid-state drive (SSD), a case, a power supply, CPU cooler and case fans, and (optionally) 1-2 GPUs. Let's consider each component one by one.

**CPU**: This is one of the most important components of your build. There are a few different variables to consider when selecting a processor. The first (and arguably most important) is clockspeed. 

**Motherboard**: Honestly, people make way too big a deal about motherboards; I would strongly recommend investing in your CPU and GPUs instead of spending a lot of money on a fancy motherboard. Basically, there are three things to look for when selecting a motherboard. First, how beefy is the Voltage Regulator Module (VRM)? The VRM is the part of the motherboard that feeds power to your processor; loosely speaking, the more "phases" the VRM has, the better able it is to smooth our irregularities in the power fed into the CPU. This usually only becomes an issue when overclocking; if you are not planning on overlocking, or only planning for a mild overclok, you probably don't need to worry about the VRM. The second factor to consider is the ports and PCI lanes supported by the motherboard.

**RAM**: A modern workstation should have at least 8GB of RAM, with 16GB preferred. There are a few things to keep in mind when selecting RAM. First, you usually want to get at least 2 sticks of RAM instead of one. This is because modern CPUs generally have at least two channels to access RAM (Intel Core processors and AMD Ryzen processors have two; Intel Xeon, Intel Core-X, AMD Epyc, and AMD Threadripper processors generally come with at least 4). By having two sticks of RAM you are thus able to use both channels and achieve full memory bandwidth; if you use only one stick, you are stuck to a single channel with half the memory bandwidth. Thus, all else being equal, it is better to have two 8GB sticks of RAM then one 16GB stick. Another thing to keep in mind is the size of the workloads you intend to run. If you intend to run a lot of video editing or scientific computing workloads, then 32GB or even 64GB might be appropriate; for most other users, 16GB should be more than enough. Don't worry too much about RAM speed or CAS latency; these generally have little impact on real workloads. Most users will be perfectly fine with RAM clocked at 2400 Mhz or 2667 Mhz (or higher). Make sure to buy the right generation of RAM - modern processors usually use DDR4 RAM, not the older DDR3 RAM.

**SSD** Let's get one thing out of the way: if you are building a workstation in 2019, it should have an solid-state drive (SSD) instead of a traditional, spinning-metal-plate Hard Disk Drive (HDD). Going from an HDD to an SSD is probably the single most effective way to upgrade an older, sluggish system.

**Case** I don't have much to say about cases; this is largely a function of your personal aesthetic. Obviously, you want a case that's large enough to house all your components - most cases will explicitly list what size GPUs they can accomodate, so make sure yours will fit before you go out and buy a case. Also, try to select a case with good airlow; you want one with plenty of vents so your case fans can easily flush out hot air. On the basis of sveeral glowing reviews, I ended up picking the **Fractal Design Meshify C** and I have to say, I really love this case. It is relatively compact, has easy to use veclro straps for cable management, and looks fantastic.

**Power supply**


**CPU cooler**


**Case fans**

**GPUs**: You may want to consider investing in a graphics processing unit (GPU) if you intend to do heavy graphical work (video editing, animation, etc.) or high performance computing/scientific computing (machine learning, physics simulations, etc.). In particular, GPUs have now become a standard tool for powering training and inference in deep learning models. Note that if your CPU does not have integrated graphics you will need a GPU just to get any video output. Almost all Intel Core processors have integrated graphics, but Intel Xeon processors and most AMD processors do not feature integrated graphics.
If all you need is video output to make up for your CPU's lack of integrated graphics, a cheap video card like the Nvidia 1030 should work fine (note that AMD cards generally have better open-source driver support and may be better supported on Linux). If you need a higher-power card you should consider 


## Assembling the system




## Troubleshooting
