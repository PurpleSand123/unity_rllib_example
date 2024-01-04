# unity_rllib_example
Reinforcement learning example using rllib  and unity ml agent

## Installation
1. Follow ml-agents [installation guide](https://unity-technologies.github.io/ml-agents/Installation/) to install ml-agents.
    > **In step of Install the mlagents Python package** 
    >
    > do Advanced: Local Installation for Development
    > ```bash
    > conda create -n ml-agents python=3.10.12
    > conda activate ml-agents
    > conda install -c conda-forge onnx=1.12.0 swig=4.0.2
    > cd ml-agents
    > pip install torch -f https://download.pytorch.org/whl/torch_stable.html
    > pip install -e ./ml-agents-envs
    > pip install -e ./ml-agents
    > ```

2. Follow rllib [installation guide](https://docs.ray.io/en/latest/ray-contribute/development.html#preparing-to-build-ray-on-linux) to install rllib.

    Follow **Building Ray (Python Only)**
    ```bash
    # For example, for Python 3.10, MacOS M1:
    pip install -U "ray[all] @https://s3-us-west-2.amazonaws.com/ray-wheels/latest/ray-3.0.0.dev0-cp310-cp310-macosx_11_0_arm64.whl" protobuf==3.19.6
    pip install "gymnasium[all]"
    
    # This replaces `<package path>/site-packages/ray/<package>`
    # with your local `ray/python/ray/<package>`.
    cd ray
    python python/ray/setup-dev.py -y --skip _private dashboard
    ```