<h1> Ishara: Real-Time Sign Language to Text Translator</h1>
<br>
SignSpeak is a web-based application that translates hand gestures into text in real time. Unlike traditional sign language datasets that are limited to alphabets or numbers, SignSpeak is designed for real-world communication. It recognizes full words such as "hello", "thank you", "please", etc., and dynamically threads them into meaningful sentences — enabling smoother, natural interaction for people who rely on sign language.

🔊 This tool is developed with accessibility in mind, especially for the Deaf and Hard-of-Hearing community, helping bridge communication gaps in everyday conversations.

🛠️ Features
✅ Real-time hand gesture recognition via webcam

✅ Word-level sign detection (not just letters or digits)

✅ Sentence stitching from recognized words

✅ Web-based: No installation required, runs directly in the browser

✅ MediaPipe + TensorFlow.js integration for efficient and fast landmark detection and classification

✅ Robust against background variations and performs in natural settings

🧠 Tech Stack
Frontend: HTML, CSS, JavaScript

ML Framework: TensorFlow.js

Hand Tracking: MediaPipe Hands

Model Training: Teachable Machine + custom post-processing

🚀 How It Works
Hand Detection: Uses MediaPipe to identify 21 hand landmarks in real-time.

Gesture Classification: Landmarks are fed into a Teachable Machine model trained on a curated dataset of meaningful hand signs.

Prediction Smoothing: Filters out noisy predictions by tracking class confidence and stability over frames.

Sentence Building: Accumulates predicted words and threads them into readable sentences (e.g., "Please help me").

Display: Recognized sentence is shown on screen in real-time for clear communication.

📸 Screenshots
Detection in Action	Sentence Output

🔍 Project Motivation
Most open-source datasets and models focus on character-based sign language, which is slow and unnatural for actual communication. This project addresses that by focusing on word-level gestures and contextual sentence formation.

Our aim was to build something closer to how real signers communicate — fluid, quick, and expressive — not letter-by-letter spelling.

📂 Folder Structure
bash
Copy
Edit
├── index.html
├── style.css
├── script.js
├── model/              # Exported Teachable Machine model
├── media/              # Screenshots and GIFs
├── README.md
🧪 Try It Out
Clone this repo:

bash
Copy
Edit
git clone https://github.com/yourusername/signspeak.git
Open index.html in a browser.

Allow webcam permissions.

Start signing!

📚 Learnings & Takeaways
Understanding of computer vision workflows for gesture recognition

Integrated MediaPipe with TF.js effectively for performance gains

Improved UX by smoothing predictions and building contextual output

Worked under real-world constraints like background interference and webcam quality

Bridged theoretical ML into usable, accessible tech for a real-world audience

💡 Future Enhancements
Add more signs (verbs, emotions, commands)

Multilingual gesture datasets

Voice output for recognized sentences (speech synthesis)

Mobile support and PWA deployment

Option to export conversations as text logs

🤝 Contributors
Clark (Developer, ML Model Trainer, Integration Engineer)

[Your team members if any]
