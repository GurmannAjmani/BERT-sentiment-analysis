# BERT sentiment-analysis
 Finteuned bert from huggingface to perform sentiment analysis.
 Dataset:A dataset of English Twitter messages with six basic emotions: anger, fear, joy, love, sadness, and surprise.
Can be accessed by 
# Use a pipeline as a high-level helper
from transformers import pipeline

pipe = pipeline("text-classification", model="RapidOrc121/BERt")

## OR

# Load model directly
from transformers import AutoTokenizer, AutoModelForSequenceClassification

tokenizer = AutoTokenizer.from_pretrained("RapidOrc121/BERt")
model = AutoModelForSequenceClassification.from_pretrained("RapidOrc121/BERt")