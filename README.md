# 📚 Book Recommendation System

A web-based book recommendation system built with Flask that provides personalized book recommendations based on collaborative filtering. The system displays top 50 popular books and recommends similar books based on user input.

## ✨ Features

- **Top 50 Books Display**: Browse the most popular and highly rated books
- **Personalized Recommendations**: Get book recommendations based on a book title you like
- **Modern UI**: Beautiful gradient design with responsive layout
- **Book Details**: View book titles, authors, ratings, and vote counts
- **Error Handling**: User-friendly error messages for invalid book titles

## 🛠️ Technologies Used

- **Backend**: Python, Flask
- **Frontend**: HTML, CSS, Bootstrap 3, Font Awesome
- **Data Processing**: NumPy, Pandas
- **Machine Learning**: Collaborative Filtering (Cosine Similarity)

## 📋 Prerequisites

- Python 3.7 or higher
- pip (Python package installer)

## 🚀 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/book-recommendation-system.git
   cd book-recommendation-system
   ```

2. **Install required packages**
   ```bash
   pip install -r requirements.txt
   ```

3. **Ensure data files are present**
   - `popular.pkl` - Popular books dataset
   - `books.pkl` - Complete books dataset
   - `pt.pkl` - Pivot table for recommendations
   - `similarity_scores.pkl` - Precomputed similarity scores

## 💻 Usage

1. **Run the Flask application**
   ```bash
   python app.py
   ```

2. **Open your browser**
   - Navigate to `http://127.0.0.1:5000` or `http://localhost:5000`

3. **Explore the application**
   - **Home Page**: View the top 50 popular books with ratings and vote counts
   - **Recommend Page**: Enter a book title to get personalized recommendations

## 📁 Project Structure

```
book-recommendation-system/
│
├── app.py                 # Main Flask application
├── requirements.txt       # Python dependencies
├── README.md             # Project documentation
│
├── templates/            # HTML templates
│   ├── index.html       # Home page (Top 50 books)
│   └── recommend.html   # Recommendation page
│
└── Data files (pickle)
    ├── popular.pkl      # Popular books data
    ├── books.pkl        # Books dataset
    ├── pt.pkl           # Pivot table
    └── similarity_scores.pkl  # Similarity matrix
```

## 🎯 How It Works

1. **Data Loading**: The application loads preprocessed data from pickle files
2. **Popular Books**: Displays top 50 books based on ratings and votes
3. **Recommendations**: 
   - User enters a book title
   - System finds the book in the dataset
   - Uses cosine similarity to find similar books
   - Returns top 6 most similar books

## 🔧 API Routes

- `GET /` - Home page displaying top 50 books
- `GET /recommend` - Recommendation search page
- `POST /recommend_books` - Process recommendation request

## 📦 Dependencies

- `flask` - Web framework
- `numpy` - Numerical computing
- `pandas` - Data manipulation
- `gunicorn` - Production WSGI server (optional)

## 🎨 Features

- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Modern UI**: Gradient backgrounds, card-based layout, smooth animations
- **Error Handling**: Graceful handling of invalid book titles
- **Fast Performance**: Precomputed similarity scores for quick recommendations

## 🔮 Future Improvements

- [ ] User authentication and personalization
- [ ] Book search with autocomplete
- [ ] Book details page with reviews
- [ ] Multiple recommendation algorithms
- [ ] User rating system
- [ ] Database integration
- [ ] API endpoints for external integration

## 📝 Notes

- The application uses precomputed similarity scores for fast recommendations
- Ensure all pickle files are in the same directory as `app.py`
- The application runs in debug mode by default (change in production)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the MIT License.

## 👤 Author

Your Name - [GitHub](https://github.com/yourusername)

## 🙏 Acknowledgments

- Book dataset used for training the recommendation model
- Flask community for excellent documentation
- Bootstrap and Font Awesome for UI components

---

⭐ If you like this project, please give it a star!
