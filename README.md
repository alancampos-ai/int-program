# Fractional allocation

#### Article: <small><strong>Fractional allocation for batch selection in integer programming</strong> <a href=""><img src="https://cdn.simpleicons.org/doi/2dd4bf" alt="DOI" height="14" align="absmiddle"></a> <a href=""><img src="https://cdn.simpleicons.org/zenodo/2dd4bf" alt="Zenodo" height="14" align="absmiddle"></a> <a href="https://drive.google.com/drive/folders/17tMMDCpuRIOaMo6VtP66p_yGUTWHW7LC?usp=sharing"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/google/google-original.svg" alt="Google Drive" height="14" align="absmiddle"></a></small>

We express the gain of rank-one cuts supported on cliques of odd size as fractional clique allocation (FCA) with residual edge completion. For weighted stable-set edge relaxations, the identity yields an exact budgeted model, independent-set feasibility conditions and sharp numerical bounds. On complete graphs with unit loads, a reserve condition yields triangle-selection hardness and a sharp $1/r$ approximation for size-$r$ cuts. Orbit decomposition gives the minimum entropy under an expected gain constraint. Experiments compare six methods on 1,440 test instances with 20 independent seeds. FCA's mean gain ratios range from $0.729$ to $0.853$ at the validation-selected temperature. At $n=96$, mean selection times are $15.75$ ms on complete graphs and $14.32$ ms on weighted graphs.

#### Dependencies

The experiments used Ubuntu 24.04.4 LTS and Python 3.10.19 with the following dependencies:

* NumPy 1.26.4
* SciPy 1.12.0
* PyTorch 2.2.0
* Matplotlib 3.10.6
* psutil 7.0.0
* PyYAML 6.0.3
* threadpoolctl 3.6.0

#### Installation

Set `FCA_BASE_IMAGE` to an existing image containing Python and the dependencies.

```bash
docker build --pull=false --build-arg FCA_BASE_IMAGE="$FCA_BASE_IMAGE" -f docker/Dockerfile -t fca:1.0.0 .
FCA_BACKEND=docker bash run_main.sh main
```

#### License (MIT)

* Copyright (c) alancampos-ai
* Code released under the MIT License.
