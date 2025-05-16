# 🧠 AI Agent for Loan Data Insights using OpenAI API

This project demonstrates how to build an AI-powered data assistant that answers natural language questions about a structured loan dataset. It uses **OpenAI's GPT-4o model** and **pandas** to simulate an intelligent agent that understands data context and generates human-like answers.

---

## 📊 Project Objective

Enable users to:
- Ask natural language questions about a dataset (e.g., "Who has the highest income?")
- Receive accurate, dynamic answers using both programmatic logic and GPT
- Explore practical applications of AI agents in data analytics

---

## 📁 Repository Structure

```
AI-Agent-Loan-Insights/
├── AI_Agent_using_OpenAI_API.ipynb     # Jupyter Notebook with agent logic
├── data/
│   └── loan_prediction.csv             # Sample dataset (Loan Application Data)
├── requirements.txt                    # Dependencies for the project
└── README.md                           # Documentation (this file)
```

---

## 🛠️ Technologies Used

- Python
- OpenAI GPT-4o (chat.completions API)
- Pandas
- Jupyter Notebook

---

## 🚀 How to Use This Project

### 1. Clone the repository

```bash
git clone https://github.com/achyuthkumarmiryala/AI-Agent-Loan-Insights.git
cd AI-Agent-Loan-Insights
```

### 2. Set up the environment

Install dependencies:

```bash
pip install -r requirements.txt
```

### 3. Add your OpenAI API key

In the notebook, insert your API key where indicated:

```python
client = OpenAI(api_key="your_openai_api_key")
```

### 4. Run the notebook

```bash
jupyter notebook AI_Agent_using_OpenAI_API.ipynb
```

You’ll see a prompt like:

```text
Welcome to Loan Review AI Agent!
You can ask anything about the loan applicants data.
Type 'exit' to quit.
```

Enter questions like:
- “What is the average loan amount?”
- “Who has the highest applicant income?”
- “How many applicants are self-employed?”

---

## 💡 Example Logic Built-In

The AI agent can:
- Calculate average values (`df['LoanAmount'].mean()`)
- Identify maximums and associated rows (`df[df['Income'] == max]`)
- Count categorical values (e.g., number of "Self_Employed" = "Yes")
- Use GPT-4o to handle open-ended or complex queries it can't match with logic

---

## 📌 Notes

- The assistant uses **keyword-based routing** to determine if a question can be answered programmatically.
- If not, it uses **OpenAI's GPT-4o** with a context prompt built from the dataset schema.
- This approach minimizes token usage while keeping answers relevant.

---

## 🔄 Example Interactions

**Q:** What is the average loan amount?  
**A:** The average loan amount applied for by all applicants is ₹146.41 thousand.

**Q:** Who has the highest applicant income?  
**A:** The applicant with the highest income has ₹81,000 and their Loan ID is LP002317.

**Q:** How many applicants are self-employed?  
**A:** The number of applicants who are self-employed is 82.

---

## 📜 License

This project is licensed under the **MIT License** — you’re free to use, modify, and distribute it.

---

## 👨‍💻 Author

**Achyuth Kumar Miryala**  
📍 Denton, TX  
📧 achyuthkumar286@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/achyuthkumarmiryala)  
🔗 [GitHub](https://github.com/achyuthkumarmiryala)

---

## 🙋‍♀️ Contributing

Feel free to fork the repo and contribute improvements:
- Extend the agent to support more query types
- Build a Streamlit UI
- Integrate LangChain for more natural query processing

PRs are welcome!

---

## ⭐ If you like this project...

Don’t forget to ⭐ star the repo and share it with others!
