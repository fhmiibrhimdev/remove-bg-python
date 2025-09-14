# Background Removal Tool using Rembg

This project provides a simple and efficient solution for removing image backgrounds using Python. Built for use within a **Jupyter Notebook** environment, it leverages the power of the `rembg` library and `Pillow` to process multiple images and optionally preview the output.

---

## Features

- ✅ **Batch background removal** from images (`.png`, `.jpg`, `.jpeg`)
- 📁 **Automatic folder management** for inputs and outputs
- 🖼️ **Optional preview** of results within Jupyter Notebook
- 💾 **Saves processed images** in `.png` format with transparent background

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/fahmiibrahimdevs/remove-bg-python.git
cd remove-bg-python
```

### 2. Install Dependencies
Make sure you have Python 3.7+ and run:
```bash
pip install rembg pillow matplotlib
```

### 3. Prepare Input Images
Place your source images inside a folder, e.g., Photo/:
```bash
Photo/
├── image1.jpg
├── image2.png
```

### Usage
Run the notebook in Jupyter and update the input/output folder paths:
```bash
input_folder = 'Photo'
output_folder = 'Output_rembg'

process_all_images(input_folder, output_folder, preview=False)
```
Set ```preview=True``` to view the result of each processed image.

### Folder Structure
```bash
remove-bg-python/
├── batch_remove_bg.ipynb     # Notebook for removing backgrounds from multiple images in batch mode
├── preview_removed_bg.ipynb  # Notebook for removing background from a single image with preview display
├── remove_bg_center.ipynb    # Notebook that removes background and centers the image on a transparent canvas
├── Photo/                    # Input folder containing original images (.jpg, .png, .jpeg) to be processed
├── Output_rembg/             # Output folder automatically created to store background-removed images (.png format)
└── README.md                 # Project documentation
```

### Dependencies
- `rembg` - background removal engine
- `Pillow` - image processing
- `matplotlib` - for preview display in notebook

### Example Output
> Input image → Background removed → Transparent PNG centered

If `preview=True`, results will be shown inline in Jupyter Notebook.
