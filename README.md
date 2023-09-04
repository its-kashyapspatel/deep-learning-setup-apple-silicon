<h1 align="center">Deep Learning Setup for Apple Silicon</h1>

---

<h3 align="center">Miniforge3 Setup</h3>

---

- brew install wget

- wget -O ~/Downloads/Miniforge3-MacOSX-arm64.sh https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-MacOSX-arm64.sh

- chmod +x ~/Downloads/Miniforge3-MacOSX-arm64.sh

- sh ~/Downloads/Miniforge3-MacOSX-arm64.sh

---

<h3 align="center">PyTorch Setup</h3>

---

- source ~/miniforge3/bin/activate

- create a new directory and move to the new directory (using mkdir and cd)

- conda create --prefix ./ENV_NAME python=3.8

- conda activate ./ENV_NAME

- pip3 install torch torchvision torchaudio

- conda install jupyter pandas numpy matplotlib scikit-learn

---

<h3 align="center">TensorFlow Setup</h3>

---

- source ~/miniforge3/bin/activate

- create a new directory and move to the new directory (using mkdir and cd)

- conda create --prefix ./ENV_NAME python=3.8

- conda activate ./ENV_NAME

- conda install -c apple tensorflow-deps

- python -m pip install tensorflow-macos

- python -m pip install tensorflow-metal

- if chardet is not found: pip install chardet

- conda install jupyter pandas numpy matplotlib scikit-learn