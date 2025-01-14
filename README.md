
![Characterizing Noise](https://raw.githubusercontent.com/ashwinkk23/Characterizing_noise/master/.fig.jpg)
# PyDaddy

## Python Data Driven Dynamics
A Python package to discover stochastic differential equations from time series data.

[![Documentation Status](https://readthedocs.org/projects/pydaddy/badge/?version=latest)](https://pydaddy.readthedocs.io/en/latest/?badge=latest) [![](https://img.shields.io/github/license/tee-lab/PyDaddy) ](https://github.com/tee-lab/PyDaddy/blob/master/LICENSE.txt)  [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tee-lab/PyDaddy.git/master?filepath=notebooks) [![](https://img.shields.io/badge/arXiv-preprint-red)](https://arxiv.org/abs/2205.02645)

PyDaddy is a comprehensive and easy to use python package to discover data-derived stochastic differential equations from time series data. PyDaddy takes the time series of state variable $x$, scalar or 2-dimensional vector, as input and discovers an SDE of the form:
$$ \frac{dx}{dt} = f(x) + g(x) \cdot \eta(t) $$

where $\eta(t)$ is uncorrelated white noise. The function $f$ is called the _drift_, and governs the deterministic part of the dynamics. $g^2$ is called the _diffusion_ and governs the stochastic part of the dynamics.

PyDaddy offers rich functionality to visualize the time series data and discover the drift and diffusion components. PyDaddy can also discover symbolic equations (such as polynomials) to the drift and diffusion functions using sparse regression.

| ![](https://github.com/tee-lab/PyDaddy/blob/docs/docs/source/tutorials/2/output_3_1.png?raw=true) |
| :---: |
| An example summary plot generated by PyDaddy, for a vector time series dataset. |

PyDaddy also provides a range of functionality such as equation-learning for the drift and diffusion functions using sparse regresssion, a suite of diagnostic functions, etc.. For more details, check out the PyDaddy [tutorials](https://pydaddy.readthedocs.io/en/latest/tutorial.html), [example notebooks](./notebooks) and [documentation](https://pydaddy.readthedocs.io/) for more details on how to use the package.

## Installation
PyDaddy is available both on PyPI and anaconda cloud and requires an environment with python3 environment.

### Using pip
![PyPI](https://img.shields.io/pypi/v/pydaddy?color=blue) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/pydaddy) ![PyPI - Status](https://img.shields.io/pypi/status/pydaddy)

	pip install pydaddy
or

    pip install git+https://github.com/tee-lab/PyDaddy.git

### Using anaconda
![](https://anaconda.org/tee-lab/pydaddy/badges/version.svg) ![](https://anaconda.org/tee-lab/pydaddy/badges/latest_release_date.svg) ![](https://anaconda.org/tee-lab/pydaddy/badges/platforms.svg)

    conda install -c tee-lab pydaddy

### Manual installation
Alternatively, the package can also be installed by cloning/downloading the git repository and running setup.py file.

    git clone https://github.com/tee-lab/PyDaddy.git
    cd PyDaddy
    python setup.py install
    
<!---
   *Click [here](https://github.com/tee-lab/PyDaddy/archive/master.zip) to download source repository zip file.*
--->

## Documentation
For more information about PyDaddy, check out the [package documentation](https://pydaddy.readthedocs.io/).

## Citation
If you are using this package in your research, please cite the repository and the associated [paper](https://arxiv.org/abs/2205.02645) as follows:

Nabeel, A., Karichannavar, A., Palathingal, S., Jhawar, J., Danny Raj, M., & Guttal, V. (2022). PyDaddy: A Python Package for Discovering SDEs from Time Series Data (Version 0.1.5) [Computer software]. https://github.com/tee-lab/PyDaddy

Nabeel, A., Karichannavar, A., Palathingal, S., Jhawar, J., Danny Raj, M., & Guttal, V. (2022). PyDaddy: A Python package for discovering stochastic dynamical equations from timeseries data. arXiv preprint [arXiv:2205.02645](https://arxiv.org/abs/2205.02645).

## Licence
PyDaddy is distributed under the [**GNU General Public License v3.0**](./LICENSE.txt).

