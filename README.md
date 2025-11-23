**🌟 AI Image Recognition Portal**

A sleek and intelligent AI-powered image classification web application built using TensorFlow's VGG19 and a lightweight Flask backend.
Upload any image → instantly get predictions powered by state-of-the-art deep learning.
This project showcases full-stack machine learning deployment: model loading, preprocessing, inference, and user interaction — all inside a clean, production-ready UI.

**🚀 Features**
**🧠 Deep Learning**

- Uses VGG19, a high-performance CNN architecture trained on ImageNet (1,000 classes).
- Automatic image preprocessing & label decoding with TensorFlow/Keras.

**🌐 Web Deployment**
- Clean, user-friendly Flask interface.
- Upload an image and receive the predicted class instantly.

**⚡ Fast & Deployable**
- Lightweight backend suitable for running on local machines, Docker, Render, Heroku, AWS, etc.
- Minimal dependencies — easy to set up and extend.

**🖼️ Demo Workflow**
1. Open the web app
2. Upload an image (PNG/JPG)
3. The app returns a prediction like:
   "golden_retriever"
4. Instant feedback — no page reloads required.

**📁 Project Structure**

AI-Image-Recognition-Portal/
- ├── app.py                # Flask backend
- ├── vgg19.h5              # Pretrained VGG19 model file
- ├── templates/
- │   └── index.html        # Frontend UI
- ├── uploads/              # Temporary image storage
- └── requirements.txt      # Dependencies list

**⚙️ Installation & Setup**

**1️⃣ Clone the repository**
- git clone https://github.com/yourusername/AI-Image-Recognition-Portal.git
- cd AI-Image-Recognition-Portal

**2️⃣ Install dependencies**
- pip install -r requirements.txt

**3️⃣ Add the pretrained model**
- Place vgg19.h5 in the project root directory.

**4️⃣ Run the Flask app**
- python app.py

**5️⃣ Open in browser**
- Visit:http://127.0.0.1:5000

**🧩 How It Works**

🔹 Image Preprocessing
- Resizes uploaded images to 224×224
- Converts to NumPy arrays
- Expands dimensions for batching
- Applies VGG19-specific preprocessing

**🔹 Prediction Pipeline**
- pred = model_predict(file_path, model)
- pred_class = decode_predictions(pred, top=1)

**🔹 Output**
- Returns the predicted ImageNet class label.

**🛡️ Security Notes**
- Safeguarded filename handling using secure_filename()
- Robust request handling for GET/POST
- Easily extendable for authentication, rate limiting, or file validation

**🚀 Future Enhancements**
- Multi-class predictions with confidence scores
- Improved UI/UX
- Docker container support
- REST API endpoints
- Real-time camera capture input
- Cloud deployment templates

**👨‍💻 Author**
- Email: vy5068@gmail.com
- GitHub: https://github.com/yadavJI-vishal
  
Feel free to fork the repo and submit a pull request.
