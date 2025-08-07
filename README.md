## Fine-Tuning with Mistral Model

**1. Pre-requisite**

Training Locally is not **recommended**. One can use [google colab](https://colab.google/) to train the model using T4 runtimes.

**2. Install the requirements and the dependencies**

- Activate the Virtual Enviroments
  
  ```bash
     python -m venv .venv
  ```

  ```
    source .venv/bin/activate #For Linux/Mac users
    source .venv/Scripts/activate #For windows users
  ```

- For users that have the higher performance we need to install [CUDA](https://developer.nvidia.com/cuda-toolkit)
  
  ```bash
    pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
  ```

- and install the requirements:
  ```bash
    pip install -r requirements.txt
  ```
- Install the build wheel
    Note, if you don't want to reinstall our dependencies, append the `--no-deps` flag!

  ```bash
      pip install --force-reinstall 'https://github.com/bitsandbytes-foundation/bitsandbytes/releases/download/continuous-release_multi-backend-refactor/bitsandbytes-0.44.1.dev0-py3-none-win_amd64.whl'
  ```

- For Google Colab user:

  ```bash 
    !pip install -U transformer
    !pip install torch torchvision torchaudio
    !pip install datasets==2.16.0
    !pip install bitsandbytes
    !pip install peft
    !pip install trl
    !pip install wandb
  ```

  Paste this in your NoteBook at the top and run.

**4. Optimization the Training Augmentation**
In this step, I have commented the usage in my notebook.

**5. For Trainer.ipynb is the finally optimization of Fine-Tuning**
Check this one out first as the main.

~~ Thank you! ~~

**Zhang Jiang**


