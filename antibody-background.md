---
title: Antibody Background
layout: page
image: /assets/images/antibody.jpg
permalink: /antibody-background
---
This page provides a background on what antibodies are, how they are used in research, and state-of-the-art protocols on procuding them. 

## What are antibodies?:
Antibodies are a class of proteins developed by immune cells in the body which act as a biological surveilance system. Whenever a novel protein (or "antigen") enters into the bloodstream, specialized cells such as macrophages and dendritic cells capture the protein and break it down in order to expose its structure. Once this process is complete, the broken-down antigen is presented to cells called Beta-Lymphocytes (or, more simply, "B-cells"). These B-cells produce antibodies with varying structures -- each with a different amino-acid sequence lining the variable region of the antibody -- in attempt to create an antibody with a variable region that is capable of binding specifically to a particular protein subunit of the antigen target. 

{% include image.html url="/assets/images/antibodies.png" description="The location of the antigen-binding site marks the variable region of the antibody. B-cells vary the amino acid sequence at the variable region in attempt to produce an antibody with the correct protein conformation to bind the target antigen. Each B-cell is responsible for generating an antibody to bind just one epitope (binding region) of the target antigen. Collectively, the B-cells to which the antigen is exposed produce antibodies against many components of the same target protein." %}

Once properly-binding antibodies have been generated, B-cells release them into the bloodstream. Whenever the foreign protein enters into the bloodstream, antibodies specific to that foreign protein will bind, alerting the immune system that the foreign protein is present and inciting the appropriate immune response. This system allows the immune system to keep taps on what proteins have entered the blood stream (bacterial proteins, viral proteins, etc.) and respond appropriately. Vaccines leverage this system to pre-expose the body to the protein structure of harmful infections such that antibodies specific to the disease vector are already present in the bloodstream at the time of the a real infection and the "biological surveilance system" is prepared to begin an attack immediately.

## How are they useful?
Scientists can leverage the specificity of antibodies in order to identify proteins of interest in their research. Alterations to the expression of programmed cell death protein 1 (PD1) are known to play a role in cancer. A cancer resarcher, therefore, may want to know the localization and expression-levels of PD1 in their tumor samples in order to better understand the relationship between PD1 and cancer pathology. Using antibodies, the researcher can accomplish this in 3 easy steps.

1. Purchase an anti-PD1 antibody from an antibody company such as Thermo-Fisher or Cell Signaling Technologies
2. Apply the anti-PD1 antibody to the tumor tissue under study. These antibodies will bind to the PD1 protein, wherever it happens to exist in the tissue.
3. Apply a "secondary antibody" flagged with a florescent or colored marker. This antibody will attach to the anti-PD1 antibodies. The florescent or colored tag will illuminate the location of the PD1 protein.
4. Place the tissue of interest under a microscope. Visualize the quantity and localization of the PD1 protein in the tissue.

{% include image.html url="/assets/images/pd1-immunohistochem.jpg" description="DAB staining identifies PD1 localization in various tumor samples (colored brown). Cell bodies are stained in blue." %}

Antibodies can be used in research to visualize proteins in a tissue (as in the above example), quantify proteins in a blood sample, and much more.

## How are research-antibodies produced?
Cell Signaling Technologies' primary buisness is the production of research-grade antibodies. The two ways that we'd go about producing these antibodies are as follows.

**Traditional Approach**: Traditionally, research antibodies are produced by leverging the biology that typically produces them. When CST identified an antigen (protein) that was of interest to reserachers, we would first isolate and purify a sample of that antigen. Next, we would inject the purified serum containing the antigen of interest into an animal, such as a rabbit or mouse. Once the organism had sufficient time to develop antibodies "against" (or specific to) the target antigen, CST would collect the blood of the organism in order to recover the antibodies that had been generated against the target. A rigorous screening process allows the company to identify the "best" (i.e. most specific and consistly binding) antibody of all the antibodies contained in the animal blood. Once a top-notch antibody had been isolated, CST would idenfy the DNA of this antibody, employ CRISPR/Cas9 techniques to mass-produce the antibody. Finally, the antibodies are packaged, sold, and shipped off to research facilities.

![polyclonal_process](/assets/images/Polyclonal-Project-Process.jpg)

**Modern Biotechnological Approach**: The more modern method of antibody production replaces live immune systems with manual design and modern biotechnological techniques. CST and many other antibody companies are beginning to employ a method in which antibody genetics are designed from scratch. In this method, our researchers start with a "template" antibody DNA sequence. They then study the structure of the target antigen, and attempt to modify the amino-acid sequence at the variable region of the template in order to create an antibody that will bind properly. The antibody design process is challenging, and our researchers must rely on their knowledge on the chemical principles of binding affinity, taking into acount the acidity, hydrophobicity, and placement of the amino acids chosen to compose the antibody variable region. Once an amino acid sequence is chosen, our researchers use CRISPR/Cas9 techniques to produce the newly designed antibody. Several testing and redesign phases ensue until a high-quality antibody results. *Overall, this method is both faster and more cost-effective than using live organisms if implemented properly.*

**In-Silico Approach**: The most modern and promising approach to antibody design involves the use of computerized simulations in the antibody design process. The *in-silico* method involves the same general process as the above method, but employs computerized molecular simulations to drive intelligent antibody design rather than relying on human intuition. In-silico approaches have been the driving force behind many modern antibody drugs, such as [Pembrolizumab](http://chemocare.com/chemotherapy/drug-info/Pembrolizumab.aspx)(Keytruda) and [Nivolumab](http://chemocare.com/chemotherapy/drug-info/Nivolumab.aspx)(Opdivo), and is being adopted at a rapid pace in the phamaceutfical industry due to its incredible discovery capabilities.

{% include image.html url="/assets/images/in-silico.jpg" description="The in-silico aproach involves starting with a template antibody and using molecular dynamics tools to test alterations to the variable region. Once researchers settle on an amino acid sequence that appears functional in computer simulations, the antibody genetic sequence is inserted into a plasmid and produced by microorganisms. Finally, the antibody is tested in lab (in-vitro). The process repeats until a superior antibody product is produced." %}


**This completes our review of antibody function and design principles.**
