# 📚 NLP & Language Modeling Repository  

Welcome to the **NLP & Language Modeling Repository**! This repository contains multiple Jupyter notebooks focusing on various aspects of natural language processing (NLP) and language modeling.  

Below is an overview of each notebook, its purpose, and key functionalities.  

---

## 📒 Notebooks  

### 1️⃣ **`auto-correct-using-lm.ipynb`**  
🚀 Implements an autocorrect feature using a language model.  

**Key Features:**  
- 🗂 **Data Processing:**  
  - `process_data()`: Reads and tokenizes text from a file.  
  - `get_vocabulary()`: Extracts vocabulary from data.  
  - `get_count()`: Counts word frequencies.  
  - `get_probs()`: Converts word counts into probabilities.  

- 🔧 **Edit Distance Functions:**  
  - Includes functions like `delete_letter()`, `switch_letter()`, `replace_letter()`, and more to generate possible corrections.  

- 🧠 **Language Model & Correction:**  
  - `build_language_model()`: Calculates word probabilities.  
  - `candidates()`: Generates possible corrections.  
  - `correction()`: Returns the most probable correction for a given word.  

**Example:**  
- **Input:** `speling`  
- **Output:** `spelling`  

---

### 2️⃣ **`estimate-word-probability.ipynb`**  
📊 Focuses on estimating word probabilities using n-grams.  

**Key Features:**  
- 🗂 **Data Preparation:**  
  - `split_to_sentences()`, `count_words()`, and filtering low-frequency words.  
- 🔢 **N-Gram Counting:**  
  - `count_n_grams()`: Counts n-grams.  
  - `estimate_probability()`: Estimates next-word probabilities.  
- 🤔 **Perplexity Calculation:**  
  - Evaluates the model using sentence perplexity.  

**Example:**  
- **Input Sentence:** `The quick brown`  
- **Prediction:** `fox`  

---

### 3️⃣ **`Minimum Edit Distance.ipynb`**  
🔤 Implements a minimum edit distance algorithm with adjacency costs for keyboard-based corrections.  

**Key Features:**  
- 🔧 **Edit Distance Calculation:**  
  - `min_edit_distance()`: Computes minimum edit distance between strings.  
  - `backtrace()`: Identifies optimal operation sequence.  
- 🎹 **Adjacency Costs:**  
  - Utilizes QWERTY keyboard adjacency for cost adjustments.  

**Example:**  
- **Input:** `teh`  
- **Output:** `the`  

---

### 4️⃣ **`Trying Using chunks.ipynb`**  
🧩 Implements an n-gram model with efficient chunked data processing for large corpora.  

**Key Features:**  
- 📂 **Chunked File Processing:**  
  - Processes large files in manageable chunks.  
  - Builds vocabulary and counts n-grams efficiently.  
- ✍️ **Text Generation:**  
  - Generates text sequences using n-gram probabilities.  

**Example:**  
- **Input:** `Once upon`  
- **Output:** `a time in a land far away.`  

---

### 5️⃣ **`Find best Correction.ipynb`**  
🔍 Determines the most probable correction for misspelled words using probabilistic methods.  

**Key Features:**  
- 🛠 **Candidate Generation:**  
  - Generates corrections using functions like `delete_letter()` and `switch_letter()`.  
- 📚 **Language Model Integration:**  
  - Calculates probabilities based on corpus frequency.  
- ⚡ **Optimization:**  
  - Filters candidates by initial letter, length similarity, and phonetic similarity.  

**Example:**  
- **Input:** `hetre`  
- **Output:** `there`  

---

## 🛠 **How to Use**  
1. Clone the repository: `git clone <repository-url>`  
2. Open the desired notebook in **Jupyter Notebook** or **Jupyter Lab**.  
3. Follow the instructions and run the cells sequentially.  

---

## 📝 **Requirements**  
- **Python 3.x**  
- **Jupyter Notebook**  
- Required Libraries: `numpy`, `pandas`, `re`, `json`  

---

## 🎯 **Conclusion**  
This repository is a comprehensive resource for learning and implementing NLP tasks like:  
- 🔧 Autocorrect  
- 📊 Word probability estimation  
- 🔤 Spell checking with advanced features (e.g., adjacency costs, chunk processing for large datasets).  

Happy Coding! ✨
