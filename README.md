## Array API Demo

This notebook reproduces key plots in the data guide paper (https://arxiv.org/abs/1908.11170) in python. The demo focuses on gravitational wave event GW150914, and covers issues such as windowing and Fourier transforms, power spectral estimation, maximizing the likelihood for numerical relativity templates and exploring correlations in the data and residuals.  For code used to
produce published figures, see https://github.com/gw-odw/Data-Guide-Paper. This demo is inspired and built on top of https://github.com/losc-tutorial/Data_Guide. We would like to extend credits to the original implementation. We use the https://jupyterbook.org/ to build the executable notebooks.

The main idea behind this demo is to showcase the use of PyTorch Tensors with SciPy modules. This is possible with [NEP 47](https://numpy.org/neps/nep-0047-array-api-standard.html) or [Array API](https://data-apis.org/array-api/latest/).

Please use [this](https://github.com/AnirudhDagar/scipy/tree/array-api-demo) SciPy branch for this demo.

### Build & Deploy Instructions

First build the jupyter book html files using the following command. This will execute all the markdown and ipynb files and create a `_build/html` dir with the website built.
```bash
jupyter-book build .
```

Branch `gh-pages` holds the deployed website. To update the deployment, use `ghp-import`. Inside the repo, run the following to update the deployed website with the current build.
```
ghp-import -n -p -f _build/html
```

For more information, please refer to https://jupyterbook.org/start/your-first-book.html.

