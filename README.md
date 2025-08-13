# 🩺 General Health Query Chatbot

This repository contains a **Python-based chatbot** powered by the **Mistral-7B-Instruct-v0.2** language model.  
The chatbot provides **general health information** in a friendly and informative manner, while incorporating **basic safety filters** to avoid giving specific medical advice.

---

## 🎯 Objective
The primary objective of this project is to:
- Answer **general health-related questions** in a safe and helpful way.
- Use **prompt engineering** to guide the language model’s behavior.
- Implement **basic safety measures** to avoid harmful or personalized medical advice.

---

## 📂 Dataset
- **Dataset Used:** None    
- It leverages the **pre-trained capabilities** of the [`mistralai/Mistral-7B-Instruct-v0.2`](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2) model, accessed via the **Hugging Face Inference Client**.
- Responses are generated based on:
  - The **model's built-in knowledge**.
  - A **system message** that defines the chatbot's role and behavior.

---

## 🤖 Model & Approach
- **Model:** `mistralai/Mistral-7B-Instruct-v0.2`
- **Access Method:** Hugging Face Inference Client
- **Core Features:**
  - **Prompt Engineering:** A carefully crafted system message instructs the model to:
    - Provide **clear and general health information**.
    - Avoid giving **personalized medical advice**.
    - Encourage users to **consult healthcare professionals**.
  - **Basic Safety Filter:**  
    - A regex-based `filter_response` function scans the chatbot's replies for phrases resembling specific medical advice.
    - If such patterns are detected, they are replaced with a **warning message**.

---

## 📊 Key Results & Findings
- **Effective Prompt Engineering:** The chatbot consistently follows safety and helpfulness guidelines.
- **Basic Safety Filtering:** The regex-based filter can flag potentially unsafe advice.
- **Interactive Chat Loop:** Users can continuously ask health questions and get filtered, safe responses.

---

## ⚠️ Important Note
> This chatbot is intended for **general informational purposes only**.  
> It is **not a substitute** for professional medical advice, diagnosis, or treatment.  
> Always seek the advice of a qualified healthcare professional for any health concerns.

---

## 🛠️ Technologies Used
- Python  
- Hugging Face Inference Client  
- Mistral-7B-Instruct-v0.2  
- Regular Expressions (for safety filter)  

---

## 📜 License
This project is open-source and available under the [MIT License](LICENSE).
