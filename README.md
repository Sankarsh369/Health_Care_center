# healthCareCenter
Health Care Center
# Health Care Center: Personalized Medical Recommendation System

**Health Care Center** is a web-based application designed to assist users in understanding potential health conditions by predicting diseases based on entered symptoms. Beyond prediction, it serves as a personalized medical recommendation system, offering valuable health tips, diet plans, precautionary measures, medication suggestions, and workout recommendations tailored to the predicted illness.

## ✨ Features

* **Symptom-Based Disease Prediction:** Input your symptoms, and the system will predict a possible disease.
* **Speech Recognition (Frontend):** Conveniently input symptoms using voice commands.
* **Comprehensive Health Recommendations:**
    * **Disease Description:** Detailed information about the predicted disease.
    * **Precautions:** Essential measures to take for the identified condition.
    * **Medication Suggestions:** Recommended medications.
    * **Recommended Diet Plans:** Nutritional guidance to aid recovery and management.
    * **Workout Plans:** Exercise suggestions to support overall health.
* **User-Friendly Interface:** Built with a responsive design using Bootstrap.

## 🚀 Technologies Used

This project leverages a combination of Python for the backend logic and web serving, along with standard web technologies for the frontend.

* **Backend:**
    * **Python:** The core programming language.
    * **Flask:** A micro web framework for building the web application.
    * **Pandas:** For data manipulation and loading datasets (symptoms, precautions, diets, medications, workout).
    * **NumPy:** For numerical operations.
    * **Scikit-learn (SVC Model):** A trained Support Vector Classifier model is used for disease prediction.
    * **Pickle:** For loading the pre-trained machine learning model.
* **Frontend:**
    * **HTML5:** For structuring the web content.
    * **CSS3:** For styling the user interface.
    * **JavaScript:** For dynamic client-side interactions, including speech recognition for symptom input.
    * **Bootstrap 5.3.1:** A popular CSS framework for responsive and modern design.

## ⚙️ Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

* Python 3.x
* `pip` (Python package installer)

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [Your Repository URL Here] # Replace with your actual GitHub repo URL
    cd HealthCareCenter # Or whatever your project folder name is
    ```
2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```
3.  **Install the required Python packages:**
    ```bash
    pip install Flask pandas numpy scikit-learn
    ```
4.  **Ensure datasets and model are in place:**
    * Make sure you have the `dataset/` folder containing `symtoms_df.csv`, `precautions_df.csv`, `workout_df.csv`, `description.csv`, `medications.csv`, `diets.csv`.
    * Ensure the `models/` folder contains `svc.pkl` (your trained SVC model).

### Running the Application

1.  **Start the Flask development server:**
    ```bash
    python main.py
    ```
2.  **Access the application:**
    Open your web browser and navigate to `http://127.0.0.1:5000/`.

## 📂 Project Structure

* `main.py`: The main Flask application file, handling routes, disease prediction logic, and rendering templates.
* `index.html`: The primary frontend template for symptom input and displaying results.
* `script.js`: Contains JavaScript for frontend interactivity, including speech recognition.
* `Medicine Recommendation System.ipynb`: Jupyter Notebook detailing the machine learning model training and data processing.
* `dataset/`: Contains CSV files with symptom data, precautions, diets, medications, etc., used by the model.
* `models/`: Stores the pre-trained machine learning model (`svc.pkl`).
* `static/`: (Assumed) Directory for CSS, images, and other static assets.
* `templates/`: (Assumed) Directory for HTML templates.
* `README.md`: This file.

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information. (If you don't have a `LICENSE` file, you should either create one or remove this section.)

---

**Developed with ❤️**
