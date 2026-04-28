# 💄 Sephora Review Sentiment Analysis

## Project Overview
This project explores whether negative brand reviews impact all users equally or are concentrated within specific customer segments.

Using a large-scale dataset of **519,409 Sephora product reviews**, we applied NLP and machine learning techniques to uncover patterns in customer dissatisfaction.

---

## Objectives
- Identify the impact of negative reviews on different customer segments
- Detect key drivers of dissatisfaction
- Compare performance of traditional ML vs deep learning models
- Provide actionable business recommendations

---

## Dataset
- **Size:** 519,409 reviews  
- **Source:** Sephora product reviews  
- **Features:**
  - Review text
  - Product metadata
  - Reviewer skin attributes  

### Sentiment Labels
- Positive (4–5 stars): 82%  
- Neutral (3 stars): 7.5%  
- Negative (1–2 stars): 10.4%  

---

## Methodology

### 1. Data Preprocessing
- Lowercasing, stopword removal, lemmatization
- TF-IDF vectorization (top 1000 features)

### 2. Models Used
- Logistic Regression (baseline)
- BERT (bert-base-uncased)

### 3. Topic Modeling
- LDA used to identify key complaint themes

---

## 📈 Key Findings

### 1. Negative reviews are NOT uniform
- Skin types show similar overall negative rates (~10–11%)
- However, **skin tone reveals major disparities**

Dark/Rich skin tones:
- ~14–15% negative reviews  
- ~67% higher dissatisfaction vs fair tones 
---

### 2. Price perception matters
- Worst segment: **Budget + Dry skin (12.3%)**
- Best segment: **Premium + Combination skin (9%)** 

Insight: dissatisfaction is driven by **expectation vs value mismatch**

---

### 3. Model Performance
| Model | Key Strength |
|------|-------------|
| Logistic Regression | Interpretability |
| BERT | Higher accuracy & better negative detection |

- BERT significantly improved negative class F1 score (~0.76)

---

### 4. Key Complaint Themes (LDA)
- Product efficacy
- Dryness & moisturization
- Sensitive skin issues
- Texture & smell
- Acne & time effects

---

## Business Recommendations

### 1. Improve product formulation
- Focus on dry & sensitive skin
- Use hypoallergenic and fragrance-free options

### 2. Expand inclusivity
- Broader shade ranges for deeper skin tones
- Address shade mismatch issues

### 3. Fix value perception
- Offer trial sizes
- Improve product transparency

### 4. Deploy real-time monitoring
- Use BERT for live sentiment tracking
- Detect emerging issues early

---

## Tech Stack
- Python
- Scikit-learn
- Hugging Face Transformers (BERT)
- NLP (TF-IDF, LDA)
- Data Visualization

---

## Future Improvements
- Real-time dashboard (Tableau / Power BI)
- Integration with live review APIs
- Advanced bias detection models
- Recommendation system for product improvements

---

## Team
- Sundus  
- Akshat  
- Susan  
- Rose  
- Erin  
- Adrika  

---

## Key Takeaway
Negative reviews are **not universal** — they are driven by **specific customer segments, expectations, and inclusivity gaps**, making targeted business strategies far more effective than generic improvements.
