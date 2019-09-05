---
title: RSA Key Generation + Encryption on FPGA
image:
  path: /assets/images/fpga-project.jpg
  thumbnail: /assets/images/fpga-project_thumb.jpg

---
As part of our Digital Electronics (CS50) course at Dartmouth, my partner, Jake Epstein, and I decided to build an RSA security hardware module using an [FPGA](https://en.wikipedia.org/wiki/Field-programmable_gate_array). We implemented both RSA key generation and encryption/decryption functionalities from scratch on the [Xilinx](https://www.xilinx.com/) Basys3 Board using the [VHDL](https://en.wikipedia.org/wiki/VHDL) hardware description language. This research project involved extensive research, approx. 4000 lines of code development in VHDL, and hands-on hardware testing.

As a part of the project, we generated a ~60 page research report, complete with simulation figures from Xilinx Vivado (a software used to simulate FPGA codes before they are placed on harware), and logic diagrams describing logic flow in our RSA module. Click a link above to learn more about VHDL and FPGAs, or visit the {% include icon-github.html username='kenneym/cs56' label='github page'%} to read our research report or view our code.
