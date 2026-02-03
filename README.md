# 🎌 Anime Recommendation System

An AI-powered anime recommendation system built with Python that uses **collaborative filtering** and **content-based filtering** to suggest anime based on user preferences and anime similarities.

## 📊 Features

- **Content-Based Filtering**: Recommends anime based on genre similarity using TF-IDF and cosine similarity
- **Collaborative Filtering**: Recommends anime based on similar users' preferences
- **Hybrid Approach**: Combines both methods for better recommendations
- **Data Visualization**: Interactive plots showing anime trends and distributions

## 🛠️ Technologies Used

- **Python 3.x**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations
- **Scikit-learn** - Machine learning algorithms (TF-IDF, Cosine Similarity)
- **Matplotlib & Seaborn** - Data visualization
- **Jupyter Notebook** - Interactive development

## 📁 Dataset

This project uses the [Anime Recommendations Database](https://www.kaggle.com/datasets/CooperUnion/anime-recommendations-database) from Kaggle, which contains:
- 12,294 anime entries
- 7,813,737 user ratings

### To use this project:
1. Download the dataset from Kaggle (link above)
2. Extract `anime.csv` and `rating.csv` to the project directory

## 🚀 Installation

1. Clone this repository:
```bash
git clone https://github.com/YOUR_USERNAME/anime-recommendation-system.git
cd anime-recommendation-system
```

2. Create a virtual environment (optional but recommended):
```bash
python -m venv .venv
.venv\Scripts\activate  # Windows
# or
source .venv/bin/activate  # Mac/Linux
```

3. Install required packages:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

4. Download the dataset from Kaggle and place `anime.csv` and `rating.csv` in the project directory

## 📖 Usage

1. Launch Jupyter Notebook:
```bash
jupyter lab
```

2. Open `anime_recommender.ipynb`

3. Run all cells to:
   - Load and explore the data
   - Build the recommendation models
   - Get personalized anime recommendations

## 💡 Example Output
```python
# Content-based recommendation
content_rec.get_recommendations('Death Note', n=5)

# Output:
#                    name                          genre  rating
# Code Geass      Action, Military, Sci-Fi, Super Power   8.83
# Psycho-Pass     Action, Police, Psychological, Sci-Fi  8.45
# Steins;Gate     Sci-Fi, Thriller                       9.17
```

## 🎯 How It Works

### Content-Based Filtering
1. Converts anime genres into TF-IDF vectors
2. Calculates cosine similarity between anime
3. Recommends anime with similar genre profiles

### Collaborative Filtering
1. Creates user-anime rating matrix
2. Finds users with similar taste
3. Recommends anime highly rated by similar users

## 📈 Results

- Successfully recommends anime based on genre similarity
- Identifies popular anime trends in the dataset
- Provides personalized recommendations based on user history

## 🔮 Future Improvements

- [ ] Add deep learning model (Neural Collaborative Filtering)
- [ ] Implement user interface with Flask/Streamlit
- [ ] Add seasonal anime recommendations
- [ ] Include anime studio-based filtering
- [ ] Deploy as web application

## 👨‍💻 Author

**Joe** - Computer Science Student at German International University

## 📝 License

This project is open source and available under the MIT License.

## 🙏 Acknowledgments

- Dataset provided by [CooperUnion on Kaggle](https://www.kaggle.com/datasets/CooperUnion/anime-recommendations-database)
- Inspired by real-world recommendation systems like Netflix and Crunchyroll
