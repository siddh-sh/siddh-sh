<div align="center">

<img src="https://raw.githubusercontent.com/siddh-sh/siddh-sh/main/banner.svg" alt="Siddh Shah — Data Science · Applied ML" width="100%" />

<br/>

[![Email](https://img.shields.io/badge/siddhshah47929@gmail.com-0B1017?style=for-the-badge&logo=gmail&logoColor=5EEAD4&labelColor=0B1017)](mailto:siddhshah47929@gmail.com)

</div>

---

## `01` &nbsp;·&nbsp; hey, i'm siddh

I build machine learning systems for domains where being wrong is expensive — markets and supply chains.

What I've come to care about is the unglamorous half of the work. Anyone can fit a model on a clean CSV. The interesting problems start after: where does the label actually come from, does the validation split lie to you, and can someone who isn't you run this thing and get an answer they'd act on. That's the part I keep choosing.

So my projects tend to look the same shape from a distance — collect the data myself, label it against something real, train something honest, then put an API or a dashboard in front of it. A model that nobody can query is a notebook, not a system.

Final year of B.Tech Data Science at **NMIMS**. Currently deep in time-series forecasting and financial NLP.

---

## `02` &nbsp;·&nbsp; what i've built

| | Project | What it does | My part |
|---|---|---|---|
| 🚚 | **[FreightIQ](https://github.com/siddh-sh/LoRRI)** | Freight procurement that explains itself. XGBoost predicts carrier delay risk, PuLP allocates volume across carriers under cost and capacity constraints, and an LLM turns the resulting optimization into plain-English justification. Scrapes live news to penalize routes hit by weather or strikes. | Top contributor — 32 of 69 commits. ML engine, scoring, market-intel agent, Flask app, map UI, deployment. |
| 📈 | **[SentimentIQ](https://github.com/siddh-sh/Financial-sentiment)** | Bullish/bearish classifier for financial headlines. The labels aren't from a sentiment lexicon — each of 353 articles is labelled by what the stock's next-day close *actually did*. TF-IDF + linear SVM behind a FastAPI service with a charting frontend. | Solo. Whole pipeline: collection, labelling, training, API, frontend. |
| 🎓 | **[EdWise](https://github.com/siddh-sh/SIH_BitWise)** | Academic suite for Smart India Hackathon — QR attendance, adaptive quizzing, AI curriculum planning. | Built the resource recommendation module: FastAPI controllers and routes, difficulty-tiered catalogue across 8 subject tracks, Jinja2 views and frontend. |
| ⚖️ | **[Pairs Trading Dashboard](https://github.com/siddh-sh/ATSA-Project)** | Statistical arbitrage on KO/PEP. ADF and Engle-Granger tests establish cointegration, then ARIMA, LSTM and Random Forest each forecast the spread so their signals can be compared. | Wrote the inference layer — model loading, live spread reconstruction from saved β, cached data fetching. |

---

## `03` &nbsp;·&nbsp; the toolkit

**core**

![Python](https://img.shields.io/badge/Python-0B1017?style=flat-square&logo=python&logoColor=5EEAD4)
![NumPy](https://img.shields.io/badge/NumPy-0B1017?style=flat-square&logo=numpy&logoColor=5EEAD4)
![Pandas](https://img.shields.io/badge/Pandas-0B1017?style=flat-square&logo=pandas&logoColor=5EEAD4)
![Jupyter](https://img.shields.io/badge/Jupyter-0B1017?style=flat-square&logo=jupyter&logoColor=5EEAD4)
![Git](https://img.shields.io/badge/Git-0B1017?style=flat-square&logo=git&logoColor=5EEAD4)

**modelling**

![scikit-learn](https://img.shields.io/badge/scikit--learn-0B1017?style=flat-square&logo=scikitlearn&logoColor=5EEAD4)
![XGBoost](https://img.shields.io/badge/XGBoost-0B1017?style=flat-square&logo=xgboost&logoColor=5EEAD4)
![TensorFlow](https://img.shields.io/badge/TensorFlow-0B1017?style=flat-square&logo=tensorflow&logoColor=5EEAD4)
![Keras](https://img.shields.io/badge/Keras-0B1017?style=flat-square&logo=keras&logoColor=5EEAD4)
![statsmodels](https://img.shields.io/badge/statsmodels-0B1017?style=flat-square&logo=python&logoColor=5EEAD4)
![PuLP](https://img.shields.io/badge/PuLP_·_LP-0B1017?style=flat-square&logo=python&logoColor=5EEAD4)

**shipping it**

![FastAPI](https://img.shields.io/badge/FastAPI-0B1017?style=flat-square&logo=fastapi&logoColor=5EEAD4)
![Flask](https://img.shields.io/badge/Flask-0B1017?style=flat-square&logo=flask&logoColor=5EEAD4)
![Streamlit](https://img.shields.io/badge/Streamlit-0B1017?style=flat-square&logo=streamlit&logoColor=5EEAD4)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-0B1017?style=flat-square&logo=postgresql&logoColor=5EEAD4)
![Supabase](https://img.shields.io/badge/Supabase-0B1017?style=flat-square&logo=supabase&logoColor=5EEAD4)
![Render](https://img.shields.io/badge/Render-0B1017?style=flat-square&logo=render&logoColor=5EEAD4)

---

## `04` &nbsp;·&nbsp; how i think about the work

- **Label from reality, not from vibes.** SentimentIQ scores headlines against realised next-day returns rather than a sentiment dictionary, because the question isn't "does this sound positive" — it's "what happened next."
- **A model that can't be queried isn't finished.** Every project here ends in an API or a dashboard, not a final notebook cell.
- **Say what's broken.** My repo READMEs list their own known issues — including a validation split of mine that leaks lookahead bias. I'd rather you read it from me than find it yourself.
- **Optimization beats prediction, often.** FreightIQ's forecast is only useful because a linear program turns it into an actual allocation decision.

---


<div align="center">

**open to data science and ML internships / new-grad roles**

[![Email](https://img.shields.io/badge/get_in_touch-0B1017?style=for-the-badge&logo=gmail&logoColor=5EEAD4&labelColor=0B1017)](mailto:siddhshah47929@gmail.com)

</div>

<!--
  STATS CARDS: removed. github-readme-stats.vercel.app (the free shared instance)
  was timing out, so the cards rendered as broken images. To bring them back,
  deploy your own instance of github-readme-stats to Vercel (5 min, free) and
  swap the hostname, then re-add:

  ## `05`  ·  the numbers
  ![Stats](https://YOUR-INSTANCE.vercel.app/api?username=siddh-sh&show_icons=true&include_all_commits=true&count_private=true&hide_border=true&bg_color=0B1017&title_color=5EEAD4&icon_color=2DD4BF&text_color=8B98A5&ring_color=FBBF24)
  ![Top languages](https://YOUR-INSTANCE.vercel.app/api/top-langs/?username=siddh-sh&layout=compact&langs_count=8&hide_border=true&bg_color=0B1017&title_color=5EEAD4&text_color=8B98A5)

  TO ADD YOUR LINKEDIN: paste this next to each Email badge, with your slug swapped in.

  [![LinkedIn](https://img.shields.io/badge/LinkedIn-0B1017?style=for-the-badge&logo=linkedin&logoColor=5EEAD4&labelColor=0B1017)](https://linkedin.com/in/YOUR-SLUG)

  A location badge can go in the same row if you want one:
  [![Location](https://img.shields.io/badge/Mumbai,_India-0B1017?style=for-the-badge&logo=googlemaps&logoColor=5EEAD4&labelColor=0B1017)](#)

  banner.svg must stay at the root of this repo or the header image 404s.
-->
