# 2025 IOB Electrophysiology & Channels - Analysis Bootcamp

Welcome to the Analysis Bootcamp for the IOB ePhys and Channels PhD course (Fall 2025). This repository contains comprehensive materials, example datasets, and step-by-step Jupyter notebooks to teach you how to analyze electrophysiology data using Python. You'll learn to work with both HDF5 files (retina recordings) and ABF files (patch-clamp data), perform spike detection, create visualizations, and generate multimedia outputs from your recordings.

## 📂 Contents

This folder contains the following materials:

### Notebooks
- **Day5_Introduction.ipynb** - Main tutorial notebook with complete examples covering:
  - Loading electrophysiology data (HDF5 and ABF formats)
  - Signal processing and filtering
  - Spike detection and visualization
  - Creating animations and audio/video from recordings
  - Working with human retina juxtacellular recordings
  
- **Day5_Your_Analysis.ipynb** - Practice notebook for you to work on your own analysis (exercises to complete)

- **Day5_Analysis_SolvedProblems.ipynb** - Solutions notebook with complete answers to the practice exercises:
  - Loading and analyzing patch-clamp data from the patch_data_2024 folder
  - Working with ABF files (current clamp and voltage clamp recordings)
  - Analyzing spike recordings from HEK cells
  - Signal processing and spike detection on patch-clamp data

### Data
- **data_example/** - Contains example HDF5 files for the main tutorial:
  - `Chevalier_data_human_retina_example.hdf5` - Human retina juxtacellular recording (used in Day5_Introduction.ipynb)
  
- **patch_data_2024/** - Contains patch-clamp ABF files for practice exercises:
  - `Spike recording.abf` - Current clamp recording from spiking HEK cells (used in practice exercises)
  - `CheRiff current.abf` - Voltage clamp recording with optogenetic stimulation
  - `CheRiff test.xlsx` - Excel file with experimental parameters and metadata

### Media Files
Example outputs generated from the Day5_Introduction.ipynb tutorial demonstrating visualization techniques:
- `Juxta_Som_Human_retina_audio.wav` - Audio representation of spike activity (spikes converted to sound)
- `Juxta_Som_Human_retina_video.mp4` - Animated visualization of the electrophysiology recording
- `Juxta_Som_Human_retina_merge.mp4` - Combined audio-video output showing synchronized spike activity

---

## 🚀 Getting Started

### For Complete Beginners

If you have **no prior experience with Python**, don't worry! Follow these step-by-step instructions.

---

## 📥 Step 1: Install Python

We recommend using **Anaconda**, which includes Python and many scientific packages pre-installed.

### For Mac Users:

1. **Download Anaconda:**
   - Go to [https://www.anaconda.com/download](https://www.anaconda.com/download)
   - Download the installer for macOS (choose the version for your chip: Intel or Apple Silicon/M1/M2)

2. **Install Anaconda:**
   - Open the downloaded `.pkg` file
   - Follow the installation wizard (accept defaults)
   
3. **Verify Installation:**
   - Open **Terminal** (find it in Applications → Utilities)
   - Type: `conda --version` and press Enter
   - You should see a version number (e.g., `conda 23.7.4`)

### For Windows Users:

1. **Download Anaconda:**
   - Go to [https://www.anaconda.com/download](https://www.anaconda.com/download)
   - Download the Windows installer (64-bit recommended)

2. **Install Anaconda:**
   - Run the downloaded `.exe` file
   - Follow the installation wizard
   - **Important:** Check "Add Anaconda to my PATH environment variable" if asked

3. **Verify Installation:**
   - Open **Anaconda Prompt** (search for it in the Start menu)
   - Type: `conda --version` and press Enter
   - You should see a version number

---

## ⚙️ Step 2: Set Up Your Environment

After installing Anaconda, you need to install additional packages required for the analysis.

### For Mac:

1. Open **Terminal**
2. Navigate to the Analysis_bootcamp folder:
   ```bash
   cd /path/to/your/Analysis_bootcamp
   ```
   **Tip:** You can drag the folder from Finder into Terminal to automatically type the path.

3. Install the required packages:
   ```bash
   conda install -c conda-forge ffmpeg
   pip install ipympl scipy pyabf moviepy pandas pytables
   ```

### For Windows:

1. Open **Anaconda Prompt**
2. Navigate to the Analysis_bootcamp folder:
   ```bash
   cd C:\path\to\your\Analysis_bootcamp
   ```
   (Replace with the actual path where you saved this folder)

3. Install the required packages:
   ```bash
   conda install -c conda-forge ffmpeg
   pip install ipympl scipy pyabf moviepy pandas pytables
   ```

**Note:** Installation may take a few minutes. Answer 'y' (yes) if prompted to proceed.

---

## 📓 Step 3: Open and Run Jupyter Notebook

### For Mac:

1. Open **Terminal**
2. Navigate to the Analysis_bootcamp folder (if you're not already there):
   ```bash
   cd /path/to/your/Analysis_bootcamp
   ```

3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

4. Your default web browser will open automatically showing the Jupyter interface
5. Click on **Day5_Introduction.ipynb** to open the tutorial notebook

### For Windows:

1. Open **Anaconda Prompt**
2. Navigate to the Analysis_bootcamp folder:
   ```bash
   cd C:\path\to\your\Analysis_bootcamp
   ```

3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

4. Your default web browser will open automatically showing the Jupyter interface
5. Click on **Day5_Introduction.ipynb** to open the tutorial notebook

---

## 🎯 Step 4: Running the Notebook

Once you have the notebook open in your browser:

1. **Run a single cell:**
   - Click on a cell (the boxes with code)
   - Press **Shift + Enter** to run the cell
   - The output will appear below the cell

2. **Run all cells:**
   - Go to the menu: **Cell → Run All**

3. **Important Tips:**
   - Run cells in order from top to bottom
   - Some cells may take a few seconds to complete
   - If you see `[*]` next to a cell, it's still running
   - If you see `[1]`, `[2]`, etc., the cell has finished running

---

## 📚 What You'll Learn

### Learning Path

**1. Start with Day5_Introduction.ipynb** (Main Tutorial)
   - Loading electrophysiology data from HDF5 and ABF files
   - Visualizing raw traces using matplotlib
   - Filtering signals with Bessel filters
   - Detecting spikes using peak detection algorithms
   - Creating animations of your data
   - Generating audio from spike recordings
   - Merging audio and video for presentations
   - Working with human retina juxtacellular recordings

**2. Practice with Day5_Your_Analysis.ipynb** (Your Turn!)
   - Apply what you learned to analyze patch-clamp data
   - Work through exercises at your own pace
   - Explore the ABF files in the patch_data_2024 folder
   - Analyze current clamp and voltage clamp recordings

**3. Check Day5_Analysis_SolvedProblems.ipynb** (Solutions)
   - See complete solutions to all practice exercises
   - Learn best practices for patch-clamp data analysis
   - Compare your approach with the provided solutions
   - Understand spike detection in HEK cell recordings

---

## 🆘 Troubleshooting

### Common Issues:

**Problem:** "conda: command not found" or "jupyter: command not found"
- **Solution:** Restart your Terminal/Anaconda Prompt after installing Anaconda, or close and reopen it.

**Problem:** Import errors when running cells (e.g., "No module named 'pyabf'")
- **Solution:** Make sure you ran the installation commands in Step 2. You can install missing packages individually:
  ```bash
  pip install pyabf
  ```

**Problem:** "No such file or directory" when loading data
- **Solution:** Make sure you're running the notebook from the correct folder (this Analysis_bootcamp folder).

**Problem:** Video/audio files not being created
- **Solution:** Make sure ffmpeg is installed correctly:
  ```bash
  conda install -c conda-forge ffmpeg
  ```

---

## 📖 Additional Resources

- **Python Basics:** [https://www.learnpython.org/](https://www.learnpython.org/)
- **Jupyter Notebook Tutorial:** [https://jupyter.org/try](https://jupyter.org/try)
- **NumPy Tutorial:** [https://numpy.org/doc/stable/user/quickstart.html](https://numpy.org/doc/stable/user/quickstart.html)
- **Matplotlib Gallery:** [https://matplotlib.org/stable/gallery/index.html](https://matplotlib.org/stable/gallery/index.html)

---

## 📧 Questions?

If you encounter any issues or have questions, please reach out during the course sessions or contact the course instructors.

**Good luck and happy coding! 🎉**