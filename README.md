# optimal transport

notebooks and code around optimal transport: theory (Monge, Kantorovich, Wasserstein) and an application to color transfer between images.

## contents

**Wasserstein Metric / Intro2OT.ipynb**  
intro to the subject: Monge problem (moving mass at minimum cost), Kantorovich relaxation, Brenier’s theorem and the Monge–Ampère equation. includes a numerical section with the Sinkhorn algorithm and a small demo (matching two 1D Gaussians). implemented with PyTorch and matplotlib.

**Color Transfer / Color_Transfer.ipynb**  
color transfer between images via optimal transport: Sinkhorn matching first, then sliced OT, with a side-by-side comparison at the end. needs PyTorch, NumPy, Pillow (PIL), matplotlib, and IPython.

## setup

python 3.x with a virtual environment is enough. install PyTorch, matplotlib, Pillow, and NumPy (e.g. `pip install torch matplotlib pillow numpy`). the notebooks assume a kernel named `.venv`; point your Jupyter kernel at your env if you use another name.

## references

the intro notebook cites Brenier (1987) and uses a figure by Marco Cuturi. the color transfer material follows the usual Sinkhorn and sliced-OT setup you see in imaging and ML.
