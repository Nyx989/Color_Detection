🎨 Color Detection & Text-to-Speech Tool
Repo: Nyx989/Color_Detection
Main Script: tts1.py
This project detects colors from an image, extracts any visible text using OCR, and converts both to audio using Google Text-to-Speech (gTTS).

📂 Files in This Repository
tts1.py — Main Python script

colors.csv — Dataset containing color names, hex codes, and RGB values

output.txt — Generated output (color + text)

output.mp3 — Audio output (played on click)

💡 Features
✅ Detects color name by double-clicking on the image
✅ Displays RGB values and matching color name
✅ Extracts text from the image using Tesseract OCR
✅ Converts results to speech using gTTS
✅ Plays the result using your system's media player

🛠️ Requirements
Install dependencies using pip:
pip install opencv-python pytesseract numpy pandas pillow gTTS
Also install Tesseract OCR:

Windows: Tesseract Download
After installation, set the path in your script:


pytesseract.pytesseract.tesseract_cmd = 'C:\\Program Files\\Tesseract-OCR\\tesseract.exe'
▶️ How to Run
python tts1.py --image path_to_your_image.jpg
Example:

python tts1.py --image cloud1.jpg
🖱️ How It Works
Opens the image window

You double-click on a region to detect color

Color name + RGB values are displayed

Any visible text in the image is read using OCR

All this information is:

Written to output.txt

Converted to speech via gTTS

Played aloud with your system's default media player

📘 colors.csv Format
Ensure this file is present in the folder. 

🔊 Output
output.txt — Contains: Color name is <DetectedColor>

output.mp3 — Audio message (auto-played)
