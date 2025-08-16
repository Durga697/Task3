🗨️ NLP Chatbot (NLTK + optional spaCy)

A simple, single-file chatbot built with classic NLP techniques (not an LLM).
It demonstrates text preprocessing, intent recognition, FAQ retrieval, and basic utilities.

✨ Features

Text preprocessing: tokenization, stopword removal, lemmatization

Intent recognition: TF-IDF + cosine similarity (scikit-learn if available)

Falls back to keyword matching if scikit-learn is missing

FAQ knowledge base: answers common NLP questions

Rule-based utilities:

Greetings / Goodbye / Thanks

Time & Date

Simple arithmetic calculations

Optional spaCy NER: adds detected entities to responses

🚀 Run
1. Clone and install requirements
git clone <your-repo-url>
cd <repo-folder>
pip install -r requirements.txt

2. Start chatbot (CLI mode)
python nlp_chatbot.py


Type your messages. To quit, type exit or quit.

⚙️ Configuration

You can customize the chatbot by editing the following in nlp_chatbot.py:

INTENTS → intent patterns & responses

KNOWLEDGE_BASE → FAQ dictionary

THRESHOLDS → minimum confidence for intent/FAQ matching

📦 Dependencies

Core:

nltk (for tokenization, stopwords, lemmatization)

Optional:

scikit-learn (for TF-IDF + cosine similarity)

spacy (for Named Entity Recognition)

en_core_web_sm model (if spaCy is installed)

Install optional extras
pip install scikit-learn spacy
python -m spacy download en_core_web_sm

🧑‍💻 Examples
You: hello
Bot: Hi there! What can I do for you?

You: what is nlp
Bot: NLP (Natural Language Processing) is a field of AI focused on enabling computers to understand and generate human language.

You: what is (2+3)*4
Bot: (2+3)*4 = 20

📝 Notes

This is not a generative AI — it’s a retrieval & rule-based demo chatbot.

Perfect for learning NLP fundamentals and coursework submissions.
