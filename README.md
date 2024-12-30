# LLM-walkthrough
This repo consists of an overview of LLMs and how we can detect generated texts

# Material
Overview on LLMs (BERTs, GPTs, Usage): https://github.com/Mooler0410/LLMsPracticalGuide
Visual explanation of common LLM networks: https://bbycroft.net/llm
Detecting generated texts: https://github.com/junchaoIU/LLM-generated-Text-Detection

# Conda Setup 

## Windows

Follow steps mentioned in https://docs.conda.io/projects/conda/en/latest/user-guide/install/windows.html to install conda

## MacOS

1. Download and install Homebrew from https://brew.sh. Follow the steps it prompts you to go through after installation.
2. Download Miniforge3 (https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-MacOSX-arm64.sh) for macOS arm64 chips.
3. Install Miniforge3 into home directory with the commands below.

''' 
chmod +x ~/Downloads/Miniforge3-MacOSX-arm64.sh
sh ~/Downloads/Miniforge3-MacOSX-arm64.sh
source ~/miniforge3/bin/activate
'''

4. Restart terminal.
5. Create a directory to setup TensorFlow environment.

'''
mkdir tensorflow-test
cd tensorflow-test
'''

# Create Environment

1. Open terminal (for mac, change directory to miniforge directory)
2. conda create --name myenv
3. conda activate myenv
4. for MacOS only
   '''
   conda install -c apple tensorflow-deps
   python -m pip install tensorflow-macos
   python -m pip install tensorflow-metal
   python -m pip install tensorflow-macos
   
   '''
5. Install packages
   '''
   conda install jupyter pandas numpy matplotlib scikit-learn
   '''
