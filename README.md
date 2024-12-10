
# **Sports Video Analysis - Setup Guide**  

This repository contains code for training a YOLOv5 object detection model and running inference on soccer game videos. Follow the steps below to set up the environment, train the model, and run inference.

---

## **1. Setup the Environment**  

You can either create a new Conda environment or skip this step if you prefer using your existing Python environment.  

### **Create a Conda Environment (Optional):**  
```bash
conda create -n soccer_analysis python=3.9
conda activate soccer_analysis
```

### **Install Required Packages:**  
```bash
pip install -r requirements.txt
```

---

## **2. Input Videos**  

- Add the videos you want the model to process into the `input_videos` directory. Ensure the videos are in a standard format like `.mp4`.  

---

## **3. Train the Model**  

> **Note:** The trained model is not uploaded due to file size limitations. Follow these steps to train the model:  

1. Open the `football_training_yolo_v5.ipynb` Jupyter Notebook.  
2. Run all the cells to train the YOLOv5 model on the provided dataset.  
3. Save the model weights in the `models` directory after training.  

---

## **4. Run Inference**  

Once the model is trained, run the inference using:  

```bash
python main.py
```

- The model will process videos from the `input_videos` directory.  
- The output videos with detection annotations will be saved in the `output_videos` directory.  

---

## **5. Check Results**  

- Navigate to the `output_videos` directory to see the object-detected videos with bounding box annotations.  
- The system automatically annotates soccer players, referees, and balls.

---

### **Troubleshooting:**  

- If you encounter package-related issues, double-check your environment setup.  
- Ensure you’ve correctly installed the libraries specified in `requirements.txt`.  

---

Let me know if you need additional details or customization! 🚀
