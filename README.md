# Retina U-Net - Retinal Vessel Detection

This project is based on retinal vessel segmentation using the U-Net architecture.  
The main goal is to identify and highlight blood vessels in retinal images which can help in the early detection of diseases like diabetic retinopathy and hypertension.

I worked on this project to understand how deep learning can be applied in the medical field, especially in image segmentation tasks. The U-Net model is quite effective here since it performs pixel-level classification and gives accurate results even for thin vessel structures.

<img width="2825" height="1752" alt="image" src="https://github.com/user-attachments/assets/2b131d1e-2be4-45ed-8446-35d78ba71f3a" />


---

## How it works

The model takes retinal fundus images as input and outputs a segmented image showing the blood vessels.  
It uses a U-Net architecture which has two main parts:
- **Encoder:** to extract important features from the image
- **Decoder:** to reconstruct the image and highlight the vessel regions

During training, the model learns from datasets like DRIVE or CHASE_DB1, where both the original and labeled images are available.

---

## Technologies and Libraries

- Python  
- TensorFlow / Keras  
- NumPy  
- OpenCV  
- Matplotlib  

---

## Steps to run the project

1. Clone the repository:
   ```bash
   git clone https://github.com/JayeshDambale/retina-unet.git
   cd retina-unet
2. pip install -r requirements.txt <!-- Install the required packages-->
3. python train.py <!--Train the model-->
4. python predict.py <!-- Run predictions-->

   <!--The results will be saved in the output directory, where you can compare original and segmented images-->


## Folder structure
retina-unet/
│
├── data/          -> contains the dataset
├── src/           -> contains model and training code
├── models/        -> saved model weights
├── utils/         -> helper functions
└── README.md

## Results
After training, the model performs well in segmenting blood vessels from retinal images.
Even the smaller and thinner vessels are detected quite accurately.
Further improvement can be done by increasing dataset size or fine-tuning the model parameters.

## About
This project helped me gain hands-on experience in deep learning for healthcare applications.
It’s a step towards combining AI with medical image analysis, and I plan to explore it more in the future.

