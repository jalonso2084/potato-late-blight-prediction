# Potato Late Blight Prediction in Huancavelica, Peru

Using machine learning and LLaMA 2–7B to predict potato late blight outbreaks in Huancavelica, Peru.

---

## 🌱 Project Description

This project combines structured agronomic data, weather variables, and large language models (LLMs) to predict the **risk of potato late blight (Phytophthora infestans)** in the highlands of **Huancavelica, Peru**.

The goal is to create a scalable, local-language-aware tool that:
- Provides **early warnings** of late blight outbreaks
- Integrates with local agricultural calendars and climatic patterns
- Demonstrates how **LLaMA 2–7B** can support agronomists and farmers

---

## 📁 Project Structure

```
.
├── data/                         # Core dataset + synthetic prompts
│   ├── Lateblight_Data_UNIQUE_Planting_Months.csv     # Final training dataset
│   ├── LLaMA_Prompts_Lateblight.csv                   # Natural language prompts (English)
│   ├── LLaMA_Prompts_Lateblight_ES.csv                # Prompts (Spanish)
│   ├── GPT_Evaluation_Lateblight_Spanish.csv          # GPT evaluation results
│   └── ...                                             # Other cleaned sources
│
├── notebooks/                   # Jupyter and Colab notebooks
│   └── Lateblight_SMOTE_RF_Colab_Notebook.ipynb       # Full model training pipeline
│
├── models/                      # Model artifacts (future use)
│
├── docs/                        # Papers and supporting documents
│   ├── Final Project Outline.pdf
│   ├── Scientific background papers
│   └── Related LLM & AI research
│
├── README.md                    # Project overview
└── .gitignore                   # Git exclusions (coming soon)
```

---

## 🔍 Main Features

- **Data Cleaning**: Consistent formatting, missing value handling, and planting season inference
- **Feature Engineering**: Added seasonal, varietal, and humidity metrics
- **Modeling**: Random Forest + SMOTE baseline model
- **Evaluation**: Confusion matrix, classification report, feature importance
- **Prompt Engineering**: LLaMA-style natural language prompts
- **Multilingual Support**: Prompts in English and Spanish
- **GPT Evaluation**: Manually tested prompt quality using GPT-4 predictions

---

## 🚀 How to Run (Colab Recommended)

1. Upload the dataset `Lateblight_Data_UNIQUE_Planting_Months.csv` to your Colab session
2. Open the notebook `notebooks/Lateblight_SMOTE_RF_Colab_Notebook.ipynb`
3. Follow the steps:
   - Install libraries
   - Load & clean data
   - Apply SMOTE
   - Train and evaluate model
4. View results and export prompt sets or model artifacts

---

## 🤖 LLM Integration (Next Phase)

- Fine-tuning a LLaMA 2–7B model using the structured + prompt-based data
- Evaluate performance against domain expert labels
- Deploy locally using a Beelink Mini PC or host inference in the cloud

---

## 📚 References

- [Large language models surpass human experts in predicting neuroscience results](https://doi.org/10.1101/2023.06.20.545742)
- [LLM See, LLM Do: Leveraging Active Inheritance to Target Non-Differentiable Objectives](https://arxiv.org/abs/2402.08381)
- Participatory varietal selection, INIA–CIP documents, and regional climate reports

---

## 👤 Author
**Jorge Alonso** – Agronomic data specialist exploring the intersection of AI and sustainable agriculture.

GitHub: [@jalonso2084](https://github.com/jalonso2084)

---

## 📌 Acknowledgments
- LLaMA 2 team (Meta)
- Researchers and agronomists working on Peruvian potato improvement
- Open-source contributors in the ML & NLP community
