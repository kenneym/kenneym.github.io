---
title: Bioinformatics at Cell Signaling Technologies
image: 
  path: /assets/images/bioinfo-summary.jpg
  thumbnail: /assets/images/bioinfo-summary_thumb.png
---
---
Freshman Summer (2018), I worked a 12-week internship as a bioinformatics intern for [Cell Signaling Technologies](https://www.cellsignal.com), a mid-size biotechnology company which creates antibodies and information technology for biological research. Through this experience, I took my first major step into the world of computer science.

While at CST I Worked to spearhead CST’s exploration of computational chemistry for antibody development, performed extensive research and code development in the drug discovery space, developed key enterprise and academic partners for CST’s further exploration of molecular dynamics, and wrote advisory documentation for the company to move forward. Further, I built upon and containerized existing molecular dynamics softwares for use on GPU-enabled cloud services. **For more background on my work, read ahead. For a visual, check out my [poster](/assets/pdfs/bioinfo-poster.pdf) for the summer**

If you would like a background on antibodies and modern techniques for antibody design, head over to the [background page](/antibody-background).

---

# My Projects:
My summer work centered around developing software, workflows, and partnerships to allow CST to move forward into the **in-silico** antibody design space (see [background](/antibody-background) for details. Embracing computational design will allow the company to rapidly accelerate their workflows and product quality.

## Learning the Ropes
My mentor for the summer, Ivan Gregoretti, PhD, prepared me for the summer by training me in basic software development skills, system administration skills, and additional skillsets specific to my assigned work. I spent my first few weeks on the job learning the following:

**Software Development**:
- Familiarity with the linux command line
- Full proficiency in the `vim` editor
- Using python bioinformatics pacakages, such as `biopython`, as well as data science pacakges such as `NumPy`
- Markdown language

**System Administration**:
- Took a full course on `Docker`. Learned how to design containers from scratch, deploy them, and manage multiple container instances.
- Learned deployment tools such as `docker-compose`, `docker-swarm`, and some `kubernetes`
- Learned essential server managment skills. How to manage user namespaces across multiple machines, `scp/ssh` protocols, etc.

**Specialized Skills**:
- Gained familiarity in parallel computing and GPU processing
- Learned how to build GPU-enabled containerized applicaitons, and how to leverage the `nvidia-docker` tool
- Built a NVIDIA GPU machine from scratch. This excercise allowed me to develop and test GPU containers and codes I had written locally and on a native graphical interface, and also provided me a basic understanding of computer architechture. Througout the process of building the GPU machine, a fellow intern and I realized that many data scientists were unaware of how to properly install a GPU or how to install the proper drivers & software to run NVIDIA GPUs on their linux system. As such, we decided to write a guide in the Fedora Magazine on how to properly install GPU hardware and drivers on a Fedora linux system. Over the past year, this post has helped approximately 70,000 viewers. See the post [here](https://fedoramagazine.org/install-nvidia-gpu/)

---

## Molecular Dynamics Containers
![nvidia-docker-logo](/assets/images/nvidia-docker-banner.png)
Molecular dynamics is an extremely expensive process from a computational pepspective. In order to use it effectively to improve our antibody design process, our company needed to be able to deploy molecular dynamics software across our company server network and across cloud platforms. In order to make this possible, my first task as an intern was to develop configurable Docker containers for the popular molecular dynamics programs `VMD` (a visual molecular modelling program) and `NAMD` (a molecular dynamics engine).

GPU Acceleration allows these programs to run up to 50X faster than on normal CPU servers, so I additionally built several containers ready for GPU workloads. These containers now allow CST to easily deploy molecular dynamics programs quickly and effectively, and to leverage the benefits of parallel computing.

As part of the open source initiatives of my mentor, we decided to publish the containers I created to [**Github**](https://github.com/kenneym/vmd-namd-gpu-containers).


### Structural Antibody Design using Alanine Scanning
{% include image.html url="/assets/images/viral-capsid.png" description="Simulation of a viral capsid immersed in water" %}

As a part of my work, I developed a molecular dynamics workflow to improve our antibody design process. I developed guidelines, wrote scripts, and worked with industry experts in order to develop a method for CST to leverage molecular dynamics simulations for better antibody design. For this leg of my work, I employed my `NAMD` and `VMD` containers to leverage cloud resources.

The procedure I developed involves a process called **computational alanine scanning** to help guide our researchers as they design the antibody varible region to properly bind a target antigen. Computational alanine scanning, in essence, is a method to determine the contribution of any given amino acid to the structure of the overall protein. The process is as follows:

1. Start with a 3-dimensional structure of the template antibody. This structure contains the location of the atoms composing the template antibody in 3D space.

2. Run energy minimization and hydrolization simulations. These simulations will expose the modeled antibody to water and calibrate it such that it takes on a natural stucture.

3. Loop through each of the amino acids at the antibody variable region, and mutate them, one at a time, into alanine (another amino acid with a very simple structure)

4. Using a technique called Free-Energy-Perterbation, determine the change in the stability of the antibody. By replacing one residue with another, and measuring change in Gibbs free energy, we can discern the importance of the original residue.

Using this process, researchers can determine whether or not they should make a change to a given residue contained within the antibody variable region. The computational alanine scanning protocols identifies whether or not any given amino acid is amenable to design changes. If a given amino acid in the template antibody is determined to be highly important to structural stablity, then researchers know not to alter it. On the other hand, if a given amino acid is found to be detrimental or unimportant to structural stablity, researchers know they may alter that amino acid in order to produce a superior antibody. In this way, computational alanine scanning provides highly valuable information to guide the antibody design process. Although it is just a first step, developing this workflow was an important first step for CST to transition into in-silico design.

---

## Antibody Homology Modelling
{% include image.html url="/assets/images/homology.png" description="Homology modeling involves using predictive softwares to infer protein structure from DNA sequence alone" %}
In order to leverage molecular dynamics softwares, one must begin with a digital model of the protein or drug they are attempting to design. In order to obtain such a model, oftentimes, companies must use expensive techniques such as X-ray crystallography in order to image the molecule of interest. Novel methods of developing models, however, employ machine learning and first-principles techniques to predict 3-dimensional protein structure using DNA sequences alone.

In order to make molecular dynamics workflows more accessable and cost-effective for use at my company, as the final leg of my 12-week internship at CST, I began to develop a methodology for CST to transition antibody genetics sequences into full-fledged stuctural models for use in molecular dynamics programs. My work on this project involved significant research, writing numerous python scripts, and developing key academic and institutional partenrs for CST to pursue this goal further. Institutional partners whom I spoke with and brought on-board include the [OSPREY Lab at Duke](https://www2.cs.duke.edu/donaldlab/osprey.php), and researchers at the [Kellog Cancer Center](https://www.northshore.org/kellogg-cancer-center/). Unfortunately, I cannot share the code or advisory documentation I completed for this poriton of my work as it is proprietary for the time being.


## Poster:
As part of my internship, I made a poster to present to the company. Click on the poster below to see a visual summmary of my work.
[![poster](/assets/pdfs/bioinfo-poster.jpg)](/assets/pdfs/bioinfo-poster.pdf)
