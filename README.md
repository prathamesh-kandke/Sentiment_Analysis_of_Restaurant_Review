# 🍽️ Sentiment Analysis of Restaurant Reviews

This project analyzes customer reviews for restaurants using machine learning. It includes both a **web-based interface** (using Flask) and a **desktop GUI application** (using Tkinter). The system can classify a review as either **positive** or **negative**, and also helps restaurant owners monitor feedback for specific food items.

---

## 📁 Project Structure

- `web_app.py` — Flask-based web application.
- `GUI_app.py` — Desktop GUI application using Tkinter.
- `cv_rest` — CountVectorizer used for transforming text input (saved as pickle).
- `model_rest` — Trained sentiment classification model (saved as pickle).
- `templates/index.html` — HTML frontend for the web app.
- `rest_review_db` — MySQL database containing food review stats.

---

## 🚀 Features

### Web App (`web_app.py`)
- Enter a restaurant review.
- View whether the review is classified as **Positive** or **Negative**.
- Simple and intuitive HTML interface.

### GUI App (`GUI_app.py`)
- Select food items and give reviews.
- Admin login system (`username: admin`, `password: admin`).
- Track reviews (positive, negative) and customers per item.
- View food-specific sentiment statistics.
- Visualize review trends using matplotlib charts.

---

## 🛠️ Technologies Used

- Python
- Flask
- Tkinter
- Scikit-learn
- CountVectorizer
- Multinomial Naive Bayes
- MySQL (via `pymysql`)
- Matplotlib

---

## 🖥️ Getting Started

### Prerequisites

- Python 3.x
- `scikit-learn`, `flask`, `pymysql`, `matplotlib`, `tkinter`
- MySQL server with `rest_review_db` database and `food_data` table.

### Run the Web App

```bash
python web_app.py
