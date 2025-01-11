# Image Compression  

This project leverages **unsupervised machine learning** techniques to compress images effectively using **K-Means Clustering**.  

## Overview  
The core idea behind this project is to reduce the size of an image by decreasing the number of clusters in its pixel data. This approach leads to **lossy compression**, where the image loses some quality but retains its essential features.  

## Key Features  
- **Unsupervised Learning:** Implements K-Means clustering for pixel grouping.  
- **Lossy Compression:** Reduces the number of unique pixel values, minimizing file size while maintaining visual quality.  
- **Scalable Solution:** Works with images of varying resolutions and formats.  

## How It Works  
1. **Image Representation:**  
   - Each pixel is treated as a data point in a 3D space (R, G, B values).  
2. **Clustering:**  
   - K-Means algorithm groups similar pixels into a defined number of clusters (K).  
3. **Reconstruction:**  
   - Each pixel is replaced with the centroid of its respective cluster.  
4. **Compression:**  
   - The reduced number of unique pixel values results in a smaller file size.  

## Why K-Means for Compression?  
- K-Means clustering efficiently groups similar pixel values, making it ideal for reducing redundant information.  
- It strikes a balance between image quality and compression ratio.  

## Prerequisites  
- Basic understanding of Python.  
- Familiarity with libraries like NumPy, Pandas, Matplotlib, and Scikit-learn.  

## How to Run  
1. Clone the repository:  
   ```bash  
   git clone <repository-url>  
   ```  
2. Install the required libraries:  
   ```bash  
   pip install -r requirements.txt  
   ```  
3. Run the script with the desired image file:  
   ```bash  
   python image_compression.py --image <image-path> --clusters <number-of-clusters>  
   ```  

## Example  
To compress an image to 16 clusters:  
```bash  
python image_compression.py --image sample.jpg --clusters 16  
```  

## Project Outcome  
This project provides a practical introduction to unsupervised learning and showcases how machine learning can be applied to real-world problems like image compression.  
