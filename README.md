# 🃏 Playing Card Prediction Django App

This Django app allows users to upload an image of a playing card, and the app predicts the card label (e.g., `"9_of_hearts"`) using a trained model or logic based on a dataset.

---

## 📁 Dataset Info

The app uses a dataset in a `cards.csv` file, which includes:

| Column       | Description                                      |
|--------------|--------------------------------------------------|
| `filepaths`  | Relative path to the image file                  |
| `labels`     | The full label for the card (e.g., `"king_of_spades"`) |
| `card type`  | The rank of the card (`ace`, `queen`, `joker`, etc.) |
| `data set`   | Dataset split (`train`, `test`, or `valid`)      |
| `class index`| Numerical index for the class                    |

---

## 🖼️ How It Works

### 1. **Frontend (UI)**
- A simple HTML form lets users upload an image of a playing card.
- The form sends a POST request to the Django backend with the uploaded image file.
- After submission, the page reloads and displays the predicted card label directly below the form using Django template rendering.
