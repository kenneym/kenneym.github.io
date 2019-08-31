---
title: Bioinformatics at Cell Signaling Technologies
image: 
  path: /assets/images/bioinfo-summary.jpg
  thumbnail: /assets/images/bioinfo-mini.jpg
---
---
Freshman Summer (2018), I worked as a bioinformatics intern for [Cell Signaling Technologies](https://www.cellsignal.com), a mid-size biotechnology company which creates antibodies and information technology for biological research. Through this experience, I took my first major step into the world of computer science.

While at CST I Worked to spearhead CST’s exploration of computational chemistry for antibody development, performed extensive research and code development in the drug discovery space, developed key enterprise and academic partners for CST’s further exploration of molecular dynamics, and wrote advisory documentation for the company to move forward. Further, I built upon and containerized existing molecular dynamics softwares for use on GPU-enabled cloud services. **For more background on my work, read ahead. For a visual, check out my [poster](/assets/pdfs/bioinfo-poster.pdf) for the summer**

---
## Background:

### What are antibodies?:
Antibodies are a class of proteins developed by immune cells in the body which act as a biological surveilance system. Whenever a novel protein (or "antigen") enters into the bloodstream, specialized cells such as macrophages and dendritic cells capture the protein and break it down in order to expose its structure. Once this process is complete, the broken-down antigen is presented to cells called Beta-Lymphocytes (or, more simply, "B-cells"). These B-cells produce antibodies with varying structures -- each with a different amino-acid sequence lining the variable region of the antibody -- in attempt to create an antibody with a variable region that is capable of binding specifically to a particular protein subunit of the antigen target. 

{% include image.html url="/assets/images/antibodies.png" description="The location of the antigen-binding site marks the variable region of the antibody. B-cells vary the amino acid sequence at the variable region in attempt to produce an antibody with the correct protein conformation to bind the target antigen. Each B-cell is responsible for generating an antibody to bind just one epitope (binding region) of the target antigen. Collectively, the B-cells to which the antigen is exposed produce antibodies against many components of the same target protein." %}

Once properly-binding antibodies have been generated, B-cells release them into the bloodstream. Whenever the foreign protein enters into the bloodstream, antibodies specific to that foreign protein will bind, alerting the immune system that the foreign protein is present and inciting the appropriate immune response. This system allows the immune system to keep taps on what proteins have entered the blood stream (bacterial proteins, viral proteins, etc.) and respond appropriately. Vaccines leverage this system to pre-expose the body to the protein structure of harmful infections such that antibodies specific to the disease vector are already present in the bloodstream at the time of the a real infection and the "biological surveilance system" is prepared to begin an attack immediately.

### How are they useful?
Scientists can leverage the specificity of antibodies in order to identify proteins of interest in their research. Alterations to the expression of programmed cell death protein 1 (PD1) are known to play a role in cancer. A cancer resarcher, therefore, may want to know the localization and expression-levels of PD1 in their tumor samples in order to better understand the relationship between PD1 and cancer pathology. Using antibodies, the researcher can accomplish this in 3 easy steps.

1. Purchase an anti-PD1 antibody from an antibody company such as Thermo-Fisher or Cell Signaling Technologies
2. Apply the anti-PD1 antibody to the tumor tissue under study. These antibodies will bind to the PD1 protein, wherever it happens to exist in the tissue.
3. Apply a "secondary antibody" flagged with a florescent or colored marker. This antibody will attach to the anti-PD1 antibodies. The florescent or colored tag will illuminate the location of the PD1 protein.
4. Place the tissue of interest under a microscope. Visualize the quantity and localization of the PD1 protein in the tissue.

{% include image.html url="/assets/images/pd1-immunohistochem.jpg" description="DAB staining identifies PD1 localization in various tumor samples (colored brown). Cell bodies are stained in blue." %}

Antibodies can be used in research to visualize proteins in a tissue (as in the above example), quantify proteins in a blood sample, and much more.

## How are research-antibodies produced?

**The Traditional Way**: 




Cell Signaling Technologies' primary buisness is the production of research-grade antibodies. As such, my work for the summer focused around improving the antibody production process







[![poster](/assets/pdfs/bioinfo-poster.jpg)](/assets/pdfs/bioinfo-poster.pdf)
