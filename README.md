readme = '''# Zomato CSAO Rail Recommendation System

## 🎯 Problem Statement
Build an intelligent recommendation system for Zomato's Cart Super Add-On (CSAO) rail to suggest relevant items that increase AOV while maintaining high customer satisfaction.

## 🚀 Quick Start

```bash
# Install dependencies
pip install -r requirements.txt

# Run the demo app
streamlit run app.py
```

## 📊 Solution Overview

### Approach
- **Problem Framing**: Sequential ranking problem with meal completion logic
- **Model**: Random Forest Classifier with 48 engineered features
- **Hybrid System**: Rule-based + ML + contextual personalization

### Performance
- **AUC**: 0.756
- **Precision@8**: 0.65
- **NDCG@8**: 0.75
- **Latency**: <150ms (well under 300ms requirement)
- **Projected AOV Lift**: 18%

### Key Features
1. **Meal Completion Rules**: Biryani → Raita → Dessert → Drink
2. **Contextual Awareness**: Time, city, user segment
3. **Cold Start Handling**: Rule-based fallbacks for new users
4. **Dynamic Updates**: Recommendations change as items are added

## 📁 Files

- `app.py` - Interactive Streamlit demo
- `csao_recommender_model.pkl` - Trained model
- `zomato_cart_sessions.csv` - Synthetic training data (15K sessions)
- `items_database.json` - 23 food items with metadata
- `meal_completion_rules.json` - Expert rules
- `model_results.json` - Evaluation metrics
- `feature_importance.csv` - Top features

##  Submission Checklist

✅ Data Generation (realistic, messy, city-wise)
✅ Feature Engineering (48 features across 5 entities)
✅ Model Training (RF with temporal split)
✅ Evaluation (AUC, Precision@K, NDCG@K)
✅ System Design (latency <150ms)
✅ Business Impact (18% AOV lift projection)
✅ Interactive Demo

## 👨‍💻 Author
Mohit Kumar | IIT Kharagpur
'''
