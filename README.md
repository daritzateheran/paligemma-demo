# Demo

## Requirements

- [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)
- [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit) (optional, for GPU-accelerated training)

## Create and Activate the Conda Environment**

1. **Create the Conda environment:**:
    ```bash
    conda create --name hug_tf python=3.9
    conda activate hug_tf
    ```

2. **Install dependencies:**
    ```bash
    conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia # GPU support
    pip install -r requirements.txt
    ```

## Configure HuggingFace Token
To use HuggingFace models, you need an access token. Save it in a .env file in the root directory of the project with the following format:

```env
HF_TOKEN=your_token_here
