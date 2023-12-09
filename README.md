# chatgpt_political_bias
Using NLP methods to investigate the political bias of ChatGPT for INF385T Fall 2023

This GitHub repo holds the code to our research investigating the implicit bias of ChatGPT's responses to questions about news topics. We leveraged the CC-News dataset from HuggingFaces for our dataset and existing research/resources (e.g. Pew Research, AllSides) to annotate our data with a political lean label: ```liberal```, ```moderate```, and ```conservative```. 

Our hypotheses for this research were:
1. ChatGPT will defer to “facts” and be “moderate” or “neutral” for many topics, especially for those that are less politically polarized (i.e. natural disasters, sports events, etc.).
2. ChatGPT will have a slight left-leaning bias for more highly polarized US-based topics (i.e. gun control) or issues–especially if asked to elaborate.
3. For international news and conflict, ChatGPT will be pro-american / pro-West which we will equate to a right-leaning slant. 

For our methodology, we first started by preparing our dataset to be a mapping of news text to a political label (see ```political_label.ipynb```), qualitatively and quantitatively extracting news topics to prompt ChatGPT with (see ```topic_modelling.ipynb```), training our classifier on our labeled dataset (see ```INSERT.ipynb```), preparing and inputting our ChatGPT prompts, and finally qualitatively and quantitatively analyzing how the ChatGPT responses are classified by our model (see ```INSERT.ipynb```). 
 
