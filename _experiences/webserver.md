---
title: Building a GPU Server
image:
  path: /assets/images/tf.png
  thumbnail: /assets/images/tf_thumb.png
---

As a way to become better versed in computer architechture, I decided to build a personal GPU server from scratch. This server offers me the capability to run accelerated machine learning workloads using NVIDIA's CUDA, host web applications, and work on "the cloud" without leaving my own machine. To build the server, I used an Intel Xeon E5 Processor, a 1080Ti NVIDIA GPU, and a heavy-duty server motherboard complete with 32GB of memory. 

In addition, I built several docker containers and automation scripts to help run web services on the server. Overall, working with this machine has vastly improved my understanding of both hardware and networking.

# Web Services:
As part of my work on this server, I built several docker containers to run appliccations such as the following:
* Jupyter Lab
* Rocketchat
* Nextcloud private cloud
* Onlyoffice Document editing
* Gitlab

Through this process, I designed a unique and simple methodology to deploy a container-based NGINX reverse proxy, complete with SSL encryption, automatically-generated CA certficiates, and more. Using my NGINX reverse proxy strategy, a user can easily deploy a website or service and host it securely on the web within minutes. *Note that documentation is forthcoming*, but you can find all of my docker-compose files and web service containers {% include icon-github.html username='kenneym/personal-server-containers' label='here.'%}

# Current Build:
To build the server, a friend and I sourced materials off of Ebay and Amazon, and I constructed the machine from scratch. Overall, we spent about 80% below normal market price. Below is our current hardware configuration.

* Processor: **Intel Xeon E5-2667 V3 (SR203 3.2GHz / 8 Core CPU)**
 
* Motherboard: **ASRock - Fatal1ty X99 Professional Gaming i7 ATX LGA2011-3 Motherboard**

* Memory: 32GB - **2x2 of Ballistix Sport LT 16GB Kit (8GBx2) DDR4 3000 MT/s (PC4-24000) SR x8 DIMM 288-Pin Memory**

* Storage **2 x WD Black 500GB High-Performance NVMe PCIe M.2 2280 SSD - Gen3, 8 Gb/s**

* GPU **ZOTAC NVIDIA GeForce GTX 1080 TI 11GB GDDR5X Graphics Card**
 
* PSU: **EVGA SuperNOVA 850 G1+, 80 Plus Gold 850W, Fully Modular** 

* CPU Cooler: **Noctua NH-D9DX i4 3U for Intel LGA2011-0 & LGA2011-3 (Square ILM & Narrow ILM), LGA1356, LGA1366 (wtih Xeon Backplate)**

* Case: **EVGA DG-76 Matte Black Mid-Tower**
