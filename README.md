# IOB Electrophysiology & Channels - Analysis Bootcamp

Welcome to the Analysis Bootcamp for the IOB ePhys and Channels PhD course (Fall 2025). This repository contains materials, example data, and Jupyter notebooks to help you learn how to analyze electrophysiology data using Python.

## 📂 Contents

This folder contains the following materials:

### Notebooks
- **Day5.ipynb** - Main tutorial notebook covering:
  - Loading electrophysiology data (HDF5 and ABF formats)
  - Signal processing and filtering
  - Spike detection
  - Creating animations and audio/video from recordings

### Data
- **data_example/** - Contains example HDF5 files:
  - `Chevalier_data_human_retina_example.hdf5` - Sample human retina recording
  
- **patch_data_2024/** - Contains additional example files:
  - `CheRiff current.abf` - Patch-clamp current recordings
  - `CheRiff test.xlsx` - Excel file with experimental parameters
  - `Spike recording.abf` - Example spike recording

### Media Files
- `Juxta_Som_Human_retina_audio.wav` - Audio output example
- `Juxta_Som_Human_retina_video.mp4` - Video visualization example
- `Juxta_Som_Human_retina_merge.mp4` - Merged audio+video example

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
2. Navigate to this folder:
   ```bash
   cd "/Users/gts/Library/CloudStorage/GoogleDrive-guilherme.silva@iob.ch/My Drive/Courses/IOB ePhys and Channels - PhD course Fall 2025/Analysis_bootcamp"
   ```
   Or navigate to wherever you downloaded/saved this folder.

3. Install the required packages:
   ```bash
   conda install -c conda-forge ffmpeg
   pip install ipympl scipy pyabf moviepy pandas pytables
   ```

### For Windows:

1. Open **Anaconda Prompt**
2. Navigate to this folder:
   ```bash
   cd "PATH\TO\YOUR\FOLDER\Analysis_bootcamp"
   ```
   (Replace `PATH\TO\YOUR\FOLDER` with the actual path where you saved this folder)

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
2. Navigate to this folder (if you're not already there):
   ```bash
   cd "/Users/gts/Library/CloudStorage/GoogleDrive-guilherme.silva@iob.ch/My Drive/Courses/IOB ePhys and Channels - PhD course Fall 2025/Analysis_bootcamp"
   ```

3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

4. Your default web browser will open automatically showing the Jupyter interface
5. Click on **Day1.ipynb** to open the notebook

### For Windows:

1. Open **Anaconda Prompt**
2. Navigate to this folder:
   ```bash
   cd "PATH\TO\YOUR\FOLDER\Analysis_bootcamp"
   ```

3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

4. Your default web browser will open automatically showing the Jupyter interface
5. Click on **Day1.ipynb** to open the notebook

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

The **Day5.ipynb** notebook covers:

1. **Loading electrophysiology data** from HDF5 and ABF files
2. **Visualizing raw traces** using matplotlib
3. **Filtering signals** with Bessel filters
4. **Detecting spikes** using peak detection algorithms
5. **Creating animations** of your data
6. **Generating audio** from spike recordings
7. **Merging audio and video** for presentations

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