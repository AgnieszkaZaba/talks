# 💬 Talks:
### **[FOSDEM'25](https://fosdem.org/2025/schedule/speaker/agnieszka_zaba/):** _open-atmos-jupyter-utils_
[![recording](https://img.shields.io/badge/-recording-lightgrey?style=flat-square)](https://ftp.fau.de/fosdem/2025/k1105/fosdem-2025-6674-lightning-lightning-talks.mp4#t=24:31,28:25)
[![slides locally](https://img.shields.io/badge/-slides-blue?style=flat-square)](https://github.com/AgnieszkaZaba/talks/blob/main/2025_FOSDEM_LLT1.pdf)

Have you ever wondered why Jupyter uses raster (and not SVG) as the inline graphics format by default?\
Or why it does not offer a "Save as PDF/SVG" button below each plot (best if also compatible with Colab)?\
Or why it does not support animated plots that render on GitHub? \
Our feelings exactly!

Here is a solution for Python notebooks using matplotlib: `import open_atmos_jupyter_utils as oaju`, replace `pyplot.show()` with `oaju.show_plot()`, and use `oaju.show_anim()` for animations.
Finally, does integration of research notebooks with automated software testing workflows sound useful? Check out the `oaju.notebook_vars()` function that can be used with pytest fixtures to streamline execution of Jupyter notebook code once per test session. This allows asserting on the final notebook state from multiple fast-executing tests (without modifications to the notebooks themselves, and with plot handling compatible with `show_plot` and `show_anim`). 

### **[SEA Improving Scientific Software Conference](https://sea.ucar.edu/iss/2025/):**  _Continuous Integration with research notebooks: on maintaining reproducibility in atmospheric modeling_
[![recording](https://img.shields.io/badge/-recording-lightgrey?style=flat-square&logo=YouTube&logoColor=%23FF0000)](https://www.youtube.com/watch?v=ErMtewdCY4s&t=16375s)
[![slides](https://img.shields.io/badge/-slides-blue?style=flat-square)](https://github.com/AgnieszkaZaba/talks/blob/main/2025_ISS_Conference.pdf)


The maintenance of research-result reproducibility can support rather than be a challenge of ongoing project development.
The integration of research notebooks with automated software testing workflows is an essential prerequisite for this. 
We present reusable tools and solutions engineered in the development and maintenance of the [PySDM](https://open-atmos.github.io/PySDM) and [PyMPDATA](https://open-atmos.github.io/PyMPDATA) atmospheric modeling projects.
Both packages are developed entirely in Python, using just-in-time compilation tools (Numba \& NVRTC) to enable a single-language HPC tech stack that covers simulation, analysis, and visualization codes.
We will discuss the perspectives of both user and developer on reproducibility.

