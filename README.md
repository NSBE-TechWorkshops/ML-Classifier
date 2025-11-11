# 🧠 Teachable Machine Image Classifier Integration

This project demonstrates how to **create, train, and integrate an image classification model** built with [Google’s Teachable Machine](https://teachablemachine.withgoogle.com/) into a simple **HTML + CSS web page**.  

If you couldn’t attend the live workshop session, follow these steps to complete the project and get your model running locally.

---

## 🚀 What You’ll Need

- A computer with a webcam  
- Internet access  
- A modern web browser (Chrome recommended)  
- Basic familiarity with HTML (optional)

---

## 🧩 Part 1: Train Your Model with Teachable Machine

1. **Go to Teachable Machine**  
   👉 [https://teachablemachine.withgoogle.com/](https://teachablemachine.withgoogle.com/)

2. **Start a new project**  
   - Click **“Get Started”**  
   - Select **“Image Project”** → **“Standard Image Model”**

3. **Train your classes**  
   - For each object you want to recognize, click **“Webcam”** and capture **at least 100 images**.  
   - Vary the **backgrounds** and **lighting** conditions for best results.  
   - Give each class a meaningful name (e.g., `Cup`, `Pen`, `Notebook`).  
   - Repeat for all objects you want to classify.

4. **Add a “Nothing” class**  
   - Capture images of your backgrounds **without any objects**.  
   - This helps the model recognize when no object is present.

5. **Train your model**  
   - Click **“Train Model”** when ready.  
   - Be patient — your browser may freeze for a few seconds during training.

6. **Test your model**  
   - Once training finishes, you can use the built-in preview on Teachable Machine to test it live.

---

## 🌐 Part 2: Integrate Your Model into a Web Page

1. **Export your model**  
   - Click **“Export Model”**  
   - Under **TensorFlow.js**, choose **“Upload (Shareable link)”**  
   - Click **“Upload my model”**

2. **Copy your shareable link**  
   - You’ll get a unique URL ending in something like `/model.json`

3. **Update the HTML file**  
   - Open the provided `index.html` file.  
   - Replace the URL on **line 23** with your model’s link.  

   ```html
   const URL = "https://teachablemachine.withgoogle.com/models/YOUR_MODEL_URL/";

4. **Update your class names**
    - On lines 87–93, replace the sample class names (Porky, Chompy, Noelle, David) with the names you used in Teachable Machine.

5. **Open the page in a browser**
    - Double-click index.html or open it via your code editor’s live server.
    - Allow camera access when prompted.

**Your model should now detect and classify objects in real-time!**
