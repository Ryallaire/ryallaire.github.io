---
title: "Project Description"
authors:
- admin
- Linda J. Cummings
- Lou Kondic
date: "2020-09-14T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: "On efficient asymptotic modelling of thin films on thermally conductive substrates. Submitted to Journal of Fluid Mechanics for Peer Review"
publication_short: ""

abstract: We consider thin films of nanoscale thickness placed on a thin thermally  conductive substrate and exposed to an external heat source. A particular application is to metal films on thin substrates exposed to laser pulses, a setup used in self-assembly of metal droplet patterns. The evolution of the free film surface is coupled to the heat transport in the film and  substrate. Due to the separation of length and time scales, long-wavetheory (LWT) can be applied to derive equations for the free surface motion. The goal of this paper is to compare and  contrast three models of heat conduction, which wecall (F) Full, (A) Asymptotic, and (1D) one-dimensional. The main finding is that (A) agrees well with (F), while being significantly less computationally demanding. Model (1D) does not give good agreement with (F) under many circumstances. Using model (A), we also consider the influence of variations in both viscosity and surface tension with temperature. We find that variations in viscosity can significantly increase the speed of film dewetting whereas accounting for temperature variation of surface tension only doesnot modify significantly the dewetting process.

# Summary. An optional shortened abstract.
summary: Our work seeks to build upon existing hydrodynamics models for collective behaviour by adding 2D and 3D force interactions including slender body flow theory and vortex sheets.

tags:
- Source Themes
featured: false

links:
- name: Arxiv Submission
  url: 'https://arxiv.org/abs/2009.06536'
url_pdf: https://arxiv.org/pdf/2009.06536.pdf
# url_code: '#'
# url_dataset: '#'
# url_poster: '#'
# url_project: ''
# url_slides: ''
# url_source: '#'
# url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/s9CC2SKySJM)'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
# - internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
#  Supplementary notes can be added here, including [code and 
# math](https://sourcethemes.com/academic/docs/writing-markdown-latex/).
# 
---

In short, we compare and contrast 3 models representing heat transport in a liquid film, placed upon a thin thermally conductive substrate. Among these models, is the asymptotic model, denoted (A), which better representative of the full model (F), than one that neglects lateral diffusion (1D) is the most computationally efficient of the bunch. The partial differential equation for (A) is:

$h Pe_{\rm f} \partial_t T_{\rm f} = \nabla_2 \cdot \left( h \nabla_2 T_{\rm f} \right) - \mathcal{K} \left( \partial_z T_{\rm s} \right)\vert_{z=0} + h \overline{Q}$

$Pe_{\rm s} \partial_t T_{\rm s} = \partial_z^2 T_{\rm s}$

where $T_{\rm f}, T_{\rm s}$ are the fluid and substrate temperatures, respectively, and the boundary conditions are omitted for brevity here. Along with the equations of heat transport is the equation describing the evolution of the free surface $z=h(x,y,t)$. This equation, commonly referred to as the thin-film equation is derived with asymptotics (long-wave approximation) which exploits the small aspect ratio of the problem, $\epsilon=H/L \ll 1$. Including temperature variation of viscosity and surface tension, the thin film equation is given by:

\begin{align}
    \partial_t h + \nabla_2 \cdot \left[ \frac{1}{\mathcal{M}} \left(  h^3  \nabla_2 \left( \Gamma \nabla_2^2 h + \Pi(h) \right) + h^2 {\rm Ma} \nabla_2 \left( \Delta T \right)  \right) \right]  = 0.
\end{align}
An example simulation is given below where random perturbations are imposed on the free surface, the domain is 20 times the wavelength of maximum growth, and viscosity is allowed to vary with temperature.

---

{{< youtube EuzoCaWUIeA >}}




