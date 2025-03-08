# Disease Prediction Web App

This is a Streamlit web application that predicts various diseases based on user input. It uses pre-trained machine learning models to provide predictions for diabetes, heart disease, Parkinson's disease, lung cancer, and hypothyroidism.

## Features

* **Disease Prediction:** Predicts diabetes, heart disease, Parkinson's disease, lung cancer, and hypothyroidism.
* **User-Friendly Interface:** Utilizes Streamlit for an interactive and easy-to-use interface.
* **Customizable Styling:** Custom CSS is used to style the app with a dark background and red text, providing a distinctive look.
* **Background Image:** A medical-themed background image enhances the app's visual appeal.
* **Model Integration:** Pre-trained machine learning models (saved as pickle files) are used for predictions.

## Technologies Used

* **Python:** The core programming language.
* **Streamlit:** For creating the web application.
* **Pickle:** For serializing and deserializing machine learning models.
* **Scikit-learn (sklearn):** For the machine learning models (implicitly used in the pickled models).
* **streamlit-option-menu:** for the option menu(even though this code uses selectbox)

## Setup and Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/Gorav22/Medical-Diagnosis
    cd Medical-Diagnosis
    ```

2.  **Create a virtual environment (recommended):**

    ```bash
    python -m venv venv
    venv\Scripts\activate  # On Windows
    source venv/bin/activate  # On macOS and Linux
    ```

3.  **Install the required packages:**

    ```bash
    pip install -r requirements.txt
    ```

4.  **Place your machine learning models:**
    * Ensure you have the following pickle files in a folder named `Models` in the same directory as your `app.py`(or the name you save your python file as) file:
        * `diabetes_model.sav`
        * `heart_disease_model.sav`
        * `parkinsons_model.sav`
        * `lungs_disease_model.sav`
        * `Thyroid_model.sav`

5.  **Run the Streamlit app:**

    ```bash
    streamlit run app.py
    ```

## Usage

1.  Open the Streamlit app in your web browser.
2.  Select a disease from the dropdown menu.
3.  Enter the required input values.
4.  Click the "Test Result" button to get the prediction.
5.  The prediction result will be displayed on the screen.

## Note

* The accuracy of the predictions depends on the quality and training of the machine learning models.
* This application is for informational purposes only and should not be used for medical diagnosis. Always consult with a healthcare professional for medical advice.
* The streamlit_option_menu import is in the code, but a streamlit selectbox is used. If you want to use the option menu, you will need to change the code.

## Customization

* You can customize the styling of the app by modifying the CSS in the `hide_st_style` and `page_bg_img` variables.
* Replace the background image URL with your own image.
* Modify the machine learning models and input fields as needed.
* To use the option menu, install the library, and replace the selectbox with the option menu code from the streamlit option menu documentation.