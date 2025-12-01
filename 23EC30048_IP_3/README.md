# README: Running assignment3_i.py on Google Colab

## Quick Setup Instructions

1. **Open Google Colab** – Go to [colab.research.google.com](https://colab.research.google.com) and create a new notebook

2. **Upload Files** – Use the Files panel (left sidebar) or run this code to upload `assignment3_i.py` and your grayscale image:
   ```python
   from google.colab import files
   files.upload()
   ```

3. **Run the Script** – Execute in a cell:
   ```python
   !python assignment3_i.py
   ```

4. **Enter Image Filename** – When prompted, type your image name with extension (e.g., `pic1.jpg`)

5. **Enter Kernel Size** – Provide an odd integer for morphological operations (e.g., `5`)

6. **Enter Closing Sizes** – Comma-separated odd integers for successive closings (e.g., `3,5,7,9`)

7. **Enter Opening Size** – Odd integer, typically larger than closing sizes (e.g., `11`)

8. **Set Threshold Factor** – Enter a decimal value or press Enter for default `0.3`

9. **View Results** – All processed images display automatically and save to `/content/` with descriptive filenames

10. **Download Outputs** – Right-click any saved image in the Files panel to download (equalized, erosion, dilation, gradient, segmentation results)

## Notes
- No additional libraries needed (NumPy, Pillow, Matplotlib pre-installed)
- Script performs histogram equalization, morphological operations, and texture segmentation
- All sizes must be odd integers for proper morphological processing
