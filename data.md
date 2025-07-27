---
layout: default
title: Data
permalink: /data/
---
# Data Cleaning

---

We primarily collect data from the Fair Disclosure (FD) Wire corpus on Nexis. A regulatory change in August 2000 (“Regulation Fair Disclosure”) led to mandatory public reporting requirements around how companies disclose information. Fair Disclosure (FD) Wire began in April 2001 as a press release service to disseminate information for companies in response to this regulatory change. One service FD Wire provides is the dissemination of earnings call transcripts, which companies opt into. We are searching for FD Wire transcripts on LexisNexis, using the Nexis API. It appears that earnings calls are not consistently available before 2005, though for some companies, call transcripts are available back to 2001. As a result, we are not only looking at earnings calls from 2005 to 2024.

<img src="https://juliocedillo.github.io/neweconomy/assets/images/GICS.svg">

We are looking at three sectors of the Global Industry Classification Standard (GICS®). GICS® is an industry analysis framework that helps investors understand the key business activities for companies around the world. MSCI and S&P Dow Jones Indices developed this classification standard to provide investors with consistent and exhaustive industry definitions. The three sectors include _financial_, _energy_, and _materials_. From here, we filter out irrelevant companies from the dataframe based on PERMNO–a unique stock (share class) level identifier, sort them by date, and verify if we have the earnings calls from the desired timeframe, flag duplicates, and retrieve missing earnings calls in either Nexis Lexis or Factiva.

# Natural Language Processing

---

Our approach involves leveraging Natural Language Processing (NLP) techniques to systematically analyze mentions of _"China"_ or _"Chinese"_ within financial call transcripts. Relevant sentences were converted into numerical representations (embeddings) using a pre-trained BERT model—specifically, `sentence-transformers/all-distilroberta-v1`—to capture their semantic meaning. To assess sentiment, custom "semantic axes" were defined for key concepts such as Economic Sentiment and Labor Costs, by contrasting sets of positive phrases (e.g., "strong economic growth") with negative ones (e.g., "economic downturn"). Sentiment scoring was performed by calculating the cosine similarity of each sentence to these axes. To ensure robustness, sentiment trends derived from these custom axes were compared against outputs from FinBERT, a finance-specific sentiment model. Finally, average sentiment scores are visualized over time to track shifts in corporate discourse.

# In-Depth Interviewing

---

_forthcoming_
