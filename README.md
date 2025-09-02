# Stable Diffusion from Scratch

This repository provides an implementation of **Stable Diffusion** built from scratch. Follow the steps below to set up the environment, download the model weights, and run the demo.

---

**Environment Setup**

It is recommended to use **Python 3.11.3** for smooth execution.

Step 1: Create a new Python virtual environment.  
On **Windows**: python -m venv venv  
On **macOS/Linux**: python3 -m venv venv  

Step 2: Activate the environment.  
On **Windows**: venv\Scripts\activate  
On **macOS/Linux**: source venv/bin/activate  

Step 3: Install the required libraries using:  
pip install -r requirements.txt  

---

**Model Weights**

You need to download the pretrained model weights to generate images.  
Download **v1-5-pruned-emaonly.ckptfrom**  [https://huggingface.co/stable-diffusion-v1-5/stable-diffusion-v1-5/tree/main] and save it in the data folder.


---

**Running the Demo**

1. Open the file named **demo.ipynb**.  
2. In the code cells, you can modify the prompt to generate different images.  
   Example: Change **"A fantasy castle in the clouds"** to **"A futuristic city at night"**.  
3. Run all cells in order to generate outputs.  

---

**Important Notes**

**Unconditional Prompt:**  
This is used when generating images without a specific description. It helps the model keep balance and avoid overfitting to just one prompt.  

**Strength of Image:**  
If you provide an initial image for image-to-image generation, the strength parameter controls how much of the original image is preserved.  

- **Higher strength** → closer to the original image  
- **Lower strength** → more influence from the new prompt  

---
