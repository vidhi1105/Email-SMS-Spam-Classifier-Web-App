 ** Email/SMS Spam Classifier Web App** 



## 🗂 Folder Structure (Visual Overview)

```
Spam-Classifier-WebApp/
│
├── app.py                  # Flask backend app
├── model.pkl               # Trained ML model (Naive Bayes)
├── vectorizer.pkl          # TF-IDF Vectorizer
├── spam.csv                # Dataset used to train the model
├── requirements.txt        # Python dependencies
├── README.md               # Project documentation
│
└── templates/
    └── index.html          # Frontend UI
```

---

## ✅ Files & Their Purposes

### 🔹 `app.py`

* This is your **Flask server** code.
* It loads the trained model and vectorizer.
* Renders the web UI (`index.html`) and returns spam prediction results.

### 🔹 `model.pkl`

* The trained Naive Bayes classifier model.
* Created using scikit-learn on the `spam.csv` dataset.

### 🔹 `vectorizer.pkl`

* TF-IDF vectorizer to transform the input messages for the model.

### 🔹 `spam.csv`

* Dataset containing real-world SMS messages labeled as `ham` or `spam`.
* Used to train the model.

### 🔹 `templates/index.html`

* Simple UI where users can enter messages.
* Form submission sends data to Flask backend for prediction.

### 🔹 `requirements.txt`

```txt
flask
sklearn
pandas
numpy
```

* You can generate it by running:

  ```bash
  pip freeze > requirements.txt
  ```

---

## 📄 Sample `README.md`

```markdown
# 📬 Email/SMS Spam Classifier - Flask Web App

This is a machine learning-powered web application that classifies input text messages as **Spam** or **Not Spam (Ham)** using a Naive Bayes classifier trained on real-world SMS data.

---

## 🚀 Features

- User-friendly web interface
- Instant spam prediction using ML model
- Built with Python, Flask, and Scikit-learn
- Trained on real SMS data (`spam.csv`)
- Fully offline, privacy-respecting app

---

## 🔧 Technologies Used

| Technology | Purpose |
|------------|---------|
| Python     | Programming Language |
| Flask      | Web App Backend |
| HTML/CSS   | Frontend |
| Pandas     | Data processing |
| Scikit-learn | ML Model & Vectorizer |

---

## 📁 Project Structure

```

Spam-Classifier-WebApp/
│
├── app.py
├── model.pkl
├── vectorizer.pkl
├── spam.csv
├── requirements.txt
└── templates/
└── index.html

````

---

## 🧪 Getting Started

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/Spam-Classifier-WebApp.git
cd Spam-Classifier-WebApp
````

### 2️⃣ Create Virtual Environment (Optional)

```bash
python -m venv venv
venv\Scripts\activate   # Windows
source venv/bin/activate  # Mac/Linux
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Run the Flask Server

```bash
python app.py
```

### 5️⃣ Open in Browser

Go to `http://127.0.0.1:5000`

---



## 📚 Dataset Information

* Source: UCI SMS Spam Collection
* Columns:

  * `v1`: label (`ham` or `spam`)
  * `v2`: actual message

---

## 👩‍💻 Author

* Vidhi Krishna Mandhana

---

## 🏷️ License

This project is licensed under the [MIT License](LICENSE).

````

---

## ✅ Final Steps for GitHub

1. Go to: [https://github.com/new](https://github.com/new)
2. Create a new repo (e.g., `Spam-Classifier-WebApp`)
3. On your system (in project folder), run:

```bash
git init
git add .
git commit -m "Initial commit: Spam classifier web app"
git remote add origin https://github.com/yourusername/Spam-Classifier-WebApp.git
git branch -M main
git push -u origin main
````

