# DroughtVision: Satellite-Based Drought Detection System  

Developed a U-Net model to segment water bodies from land and track temporal water-level changes, enabling early drought alerts through a threshold-based monitoring pipeline.

---

## Overview  

DroughtVision is a computer vision-based system that leverages satellite imagery to monitor water bodies over time and detect early signs of drought.

The pipeline works by:
- Segmenting water bodies using a U-Net model  
- Tracking changes in water body area across time  
- Triggering alerts when significant depletion is detected  

---

## System Architecture  

This diagram illustrates the architecture of the U-Net model used in DroughtVision.  

![System Architecture](git/Unet-Architecture.png)

---

## Model Performance  

Below is a visualization of model performance on sample images.  

![Model Performance](git/performance.png)

---

## Drought Monitoring Methodology  

Drought detection is performed using a computer vision-based temporal analysis pipeline:

1. **Water Body Segmentation**  
   Satellite images are processed using the U-Net model to separate water bodies from land.

2. **Temporal Area Tracking**  
   The segmented outputs are used to compute the **water body area over time**.

3. **Change Detection**  
   The system compares current water area against its **initial baseline levels**.

4. **Threshold-Based Alerting**  
   If the water body area drops below a predefined threshold relative to its original size, the system triggers a **drought alert**.

---

## Real-Time Output  

A screenshot showing how the model performs on real satellite imagery, highlighting segmented water bodies and detected drought signals.  

![Real-Time Output](git/real-time-performance.png)

---

## Key Insight  

By combining **semantic segmentation with temporal analysis**, the system moves beyond static detection and enables **continuous environmental monitoring**, making it suitable for real-world drought prediction scenarios.

---

## Tech Stack  

- Python  
- TensorFlow / Keras  
- U-Net Architecture  
- OpenCV  
- NumPy, Matplotlib  
