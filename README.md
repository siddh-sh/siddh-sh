<img src="https://raw.githubusercontent.com/siddh-sh/siddh-sh/main/banner.svg" alt="Siddh Shah — Data Science · Applied ML" width="100%" />

Final-year B.Tech Data Science at NMIMS. I build ML for markets and logistics — domains where a wrong answer costs somebody money, which makes it harder to avoid the question of whether the model is actually right.

Most student ML projects are a model fitted to a clean CSV someone else labelled. Mine are organised around the part before that: deciding what "correct" means, and getting the label from something real rather than something convenient.

<img src="https://raw.githubusercontent.com/siddh-sh/siddh-sh/main/pipeline.svg" alt="Four projects, one shape: collect, establish ground truth, model, serve" width="100%" />

---

### FreightIQ

*LogisticsNow hackathon · team of five · 32 of 69 commits mine* — [repo](https://github.com/siddh-sh/LoRRI)

XGBoost scores carrier delay risk; a PuLP linear program turns those scores into an actual volume allocation across carriers under cost and capacity constraints; an LLM writes the justification in plain English. The forecast on its own would be a number nobody can act on — the optimisation is what makes it a decision, and the explanation is what makes it trustable.

I wrote the ML engine, the scoring and market-intelligence modules, the Flask application, the map UI, and the deployment config.

### SentimentIQ

*solo* — [repo](https://github.com/siddh-sh/Financial-sentiment)

353 financial headlines across seven large-cap tickers, each labelled by what the stock's next-day close *actually did* — not by a sentiment dictionary. TF-IDF into a linear SVM, served over FastAPI behind a charting frontend.

The model is deliberately boring. The labelling is the project: "does this headline sound positive" and "what happened the next session" are different questions, and only the second one is worth anything.

### Pairs trading dashboard

*team · I wrote the inference layer* — [repo](https://github.com/siddh-sh/ATSA-Project)

ADF and Engle-Granger tests establish that KO and PEP are cointegrated; the fitted β, μ and σ are persisted so inference never has to refit. ARIMA, an LSTM, and a Random Forest each forecast the spread so their signals can be compared head to head.

My part loads all four saved artefacts, reconstructs the live spread from the stored β, and caches aggressively enough that a session touches the network at most once every fifteen minutes.

### EdWise

*Smart India Hackathon · team* — [repo](https://github.com/siddh-sh/SIH_BitWise)

I built the Curriculum Planner's resource recommendation module — the FastAPI controllers and routes, a difficulty-tiered catalogue spanning eight subject tracks, and the Jinja2 views and frontend on top of it.

---

### What's currently wrong with my own code

Listed here because you'd find it anyway, and I'd rather you heard it from me:

**SentimentIQ's validation is optimistic.** The train/test split is random, over data spanning June 2024 to November 2025. On time-ordered financial data that leaks future information into training — so any accuracy figure I quoted from it would be inflated. A chronological split is the fix, and the honest number goes up when I've run it.

**`collect_data.py` in that repo doesn't run.** It imports `fetch_alpha_daily` from a module where that function no longer exists. The committed dataset and trained model work fine, but you couldn't regenerate the data from scratch.

Neither is hard to fix. I'm flagging them because the first one is the failure mode that actually matters — a model that looks good because the evaluation is wrong is worse than one that looks bad honestly.

---

### Now

Chronological validation and a FinBERT baseline for SentimentIQ. Finishing the Streamlit layer on the pairs-trading dashboard.

**siddhshah47929@gmail.com** · [linkedin.com/in/siddh-shah11](https://linkedin.com/in/siddh-shah11)

Open to data science and ML internships and new-grad roles.

<!--
  Deliberately no shields.io badges, no stats cards, no emoji.
  banner.svg and pipeline.svg must stay at the root of this repo or the images 404.
-->
