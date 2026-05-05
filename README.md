# Real-Time Retail Feedback Intelligence

A Generative AI pipeline that transforms unstructured customer reviews into actionable retail insights using prompt engineering.

## Business Problem
Fashion retailers like ChicStyle receive thousands of reviews during peak seasons. A single delayed response to a complaint can cost customer loyalty. This project automates feedback analysis at scale.

## What This Project Does
- **Sentiment Analysis** — classifies each review as Positive, Neutral, or Negative
- **Category Detection** — identifies which product or issue the feedback refers to
- **Urgency Scoring** — flags high-priority issues for the retail team
- **Personalized Responses** — auto-generates customer reply messages
- **Retail Insights** — surfaces actionable recommendations per review

## Techniques Compared

| Technique | Avg Judge Score |
|---|---|
| Zero-Shot V1 | 0.833 |
| Zero-Shot V2 | 0.810 |
| Few-Shot V1 | 0.845 |
| Few-Shot V2 | 0.845 |
| CoT V1 | — |
| **CoT V2 Best** | **0.903** |

Chain-of-Thought prompting outperforms all others — especially on mixed or ambiguous reviews.

## Tech Stack
- Python, Pandas, Matplotlib, Plotly, Seaborn
- OpenAI API (`gpt-4o-mini`)
- Prompt Engineering (Zero-Shot, Few-Shot, Chain-of-Thought)
- LLM-as-a-Judge evaluation framework
- scikit-learn (classification metrics)

## Files
| File | Description |
|---|---|
| `Real_Time_Retail_Feedback_Intelligence_Portfolio.ipynb` | Main notebook |
| `Dataset_-_Real-Time_Retail_Feedback_Intelligence.csv` | Women's e-commerce clothing reviews |

## How to Run
1. Clone this repo
2. Install dependencies: `pip install pandas matplotlib seaborn openai wordcloud plotly tqdm scikit-learn`
3. Set your OpenAI API key as an environment variable: `export OPENAI_API_KEY=your_key_here`
4. Open the notebook in Jupyter or Google Colab

## Key Findings
- Sizing and fit are the #1 pain point across all departments
- 3-star reviews behave like negative feedback — most don't recommend the product
- CoT prompting detects nuanced dissatisfaction that Zero-Shot and Few-Shot miss
- Recommendation behavior alone is not a reliable signal for customer satisfaction

## 📬 Contact
[LinkedIn](https://www.linkedin.com/in/luisa-correa-data/)
