# 🎭 Emotion-Based Media Player 🎵  

## 📌 About  
The **Emotion-Based Media Player** is an AI-powered application that detects facial emotions in real-time and plays music based on the user's mood. It leverages **deep learning** for **emotion recognition** and **computer vision** for face detection. The system categorizes emotions into **Happy, Neutral, Sad, Angry, and Surprise**, then selects music accordingly.  

## 🚀 Features  
✅ **Real-time Facial Emotion Detection** using OpenCV & Keras  
✅ **AI-Driven Music Selection** based on facial expressions  
✅ **Spotify Integration** (Automatically opens relevant playlists)  
✅ **Automatic Playlist Handling** for different emotions  
✅ **Lightweight & User-Friendly Interface**  

---

## 🛠 Installation  

### **📌 Prerequisites**  
Ensure you have the following installed before proceeding:  
- **Python 3.7 - 3.9** (Not compatible with Python 3.10+)  
- **TensorFlow & Keras** (For deep learning models)  
- **OpenCV** (For face detection)  
- **Spotipy** (Spotify API integration)  
- **NumPy** (Array processing)  
- **pygame** (For local media playback)  

### **📌 Setup Steps**  

#### **1️⃣ Clone the Repository**  
```bash  
git clone https://github.com/girishchowdary0208/EmotiTune.git  
cd EmotiTune
```  

#### **2️⃣ Set Up a Virtual Environment**  
(Only needed if Python is not between versions 3.7 - 3.9)  

- **For Windows:**  
  ```bash  
  python -m venv env  
  env\Scripts\activate  
  ```  
- **For macOS/Linux:**  
  ```bash  
  python3 -m venv env  
  source env/bin/activate  
  ```  

#### **3️⃣ Install Dependencies**  
```bash  
pip install -r requirements.txt  
```  

#### **4️⃣ Install Python 3.9 (If Required)**  
Ensure your system is using **Python 3.9**, as the project is not compatible with Python 3.10+.  

#### **5️⃣ Set Up Spotify API Credentials**  
Create a `.env` file and add your credentials:  
```ini  
SPOTIFY_CLIENT_ID=your_client_id  
SPOTIFY_CLIENT_SECRET=your_client_secret  
SPOTIFY_REDIRECT_URI=http://localhost:8888/callback  
```  
(You can obtain these credentials from the [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/).)  

#### **6️⃣ Ensure Required Files Are Available**  
Make sure the following files exist in your project directory:  
- `haarcascade_frontalface_default.xml` (Face detection model)  
- `Emotion_Detection.h5` (Pre-trained emotion detection model)  
- `playlists.txt` (Contains playlists mapped to different emotions)  

---

## 🎮 Usage  
To start the application, run:  
```bash  
python main.py  
```  
The application will:  
1️⃣ **Open the webcam feed** and detect faces.  
2️⃣ **Analyze facial expressions** and classify the detected emotion.  
3️⃣ **Play music** from local files or Spotify playlists based on the detected emotion.  

---

## 🎵 Controls  
- **Press 'q'** → Exit the program  
- **Press 'p'** → Pause music  
- **Press 'r'** → Resume music  

---

## 📂 Project Structure  
```  
📂 EmotiTune  
├── 📜 main.py                  # Main application script  
├── 📜 requirements.txt         # Required dependencies  
├── 📜 way.env                  # Spotify API credentials (not included in repo)  
├── 📜 playlists.txt            # Emotion-based playlist mappings  
├── 📜 haarcascade_frontalface_default.xml  # Face detection model  
├── 📜 Emotion_Detection.h5     # Trained emotion detection model    
```  

---

## 📝 Sample `playlists.txt`  
This file maps emotions to playlists:  
```ini  
Happy = Happy Hits, Party Time, Feel Good Vibes  
Neutral = Chill Vibes, Relaxing Music, Study Playlist  
Sad = Sad Songs, Melancholy Mix, Deep Feels  
Angry = Rock Anthems, Metal Hits, Workout Motivation  
Surprise = Trending Now, Discover Weekly, Fresh Finds  
```  

---

## 🤝 Contributing  
Feel free to submit **issues**, suggest **improvements**, or create a **pull request**.  

---

## 📜 License  
This project is licensed under the **MIT License**.  

---

## 📬 Contact  
For any questions or feedback, reach out via [GitHub Issues](https://github.com/girishchowdary0208/EmotiTune/issues).

