# Crop360 | Holistic Plant & Crop Management
(Diagnose | Decide | Predict)
Live Output: Oct 2024 – Dec 2024

# Description
Crop360 is an AI-driven agricultural platform that provides comprehensive support to farmers and agronomists. It helps them diagnose plant diseases, recommend suitable crops, and predict crop yields by analyzing data such as soil pH, sunlight exposure, geolocation, temperature, and humidity.
Trained on 200,000+ datasets, Crop360 delivers actionable insights with a 97% disease detection accuracy, aiming to reduce crop losses by up to 30%.

# Key Features
Plant Disease Detection: Uses Convolutional Neural Networks (CNNs) to detect and classify plant diseases from leaf images with 97% accuracy.

Crop Recommendation: Suggests the best crop to cultivate based on:

Soil characteristics: pH, type, nutrients

Climate data: rainfall, temperature, humidity

Geocoordinates and sunlight exposure

Yield Prediction: Estimates crop productivity using regression models trained on historical agricultural data.

User Interface: Built with Flask and Streamlit for a smooth and accessible user experience.

# Technologies Used
1. Python: Core programming language

2. Jupyter Notebook: Model development and testing

3. TensorFlow, Keras: Deep learning model implementation

4. scikit-learn: Machine learning and data modeling

5. NumPy, Pandas: Data preprocessing and manipulation

6. Matplotlib, Seaborn: Data visualization

7. Streamlit, Flask: Web-based deployment

8. CNNs: For image-based disease detection

9. SDLC: Follows structured software lifecycle design

## Folder Structure Explanation
csharp
Copy
Edit
Crop360/
│
├── app.py
├── requirements.txt
│
├── static/
│   └── img.jpg         # Store images, stylesheets, etc.
│
├── templates/
│   └── index.html      # Store HTML templates for rendering
│
└── model/
    └── crop_model.pkl  # Trained ML model
Image & Template Integration in Flask
In your HTML (inside templates/index.html):

html
Copy
Edit
<img src="{{ url_for('static', filename='img.jpg') }}" alt="Crop Image">
In your Flask route (inside app.py):

python
Copy
Edit
from flask import Flask, render_template
app = Flask(__name__)

@app.route('/')
def home():
    return render_template('index.html')
Installation and Usage
bash
Copy
Edit
# Step 1: Clone the repository
git clone https://github.com/UMAR-ALAM-786/Crop360.git

# Step 2: Navigate to the project directory
cd Crop360

# Step 3: Install dependencies
pip install -r requirements.txt

# Step 4: Run the application
python app.py

# Step 5: Access it via browser
http://localhost:5000
Future Enhancements
Integration of real-time weather APIs

Inclusion of crop market prices to guide economically viable decisions

Development of mobile application (Android/iOS)

User feedback loops to continuously retrain and improve model accuracy

Multilingual support for broader accessibility

Contributions
Contributions are highly welcome!
Feel free to submit suggestions, issues, or pull requests via GitHub Issues.

Acknowledgements
We acknowledge the support of the agricultural research community, data contributors, and farmers who helped shape the foundation of Crop360.

Contact
Email: alamumar91@gmail.com

GitHub: UMAR-ALAM-786
