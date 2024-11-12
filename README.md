# 🤖 Azure Intelligent Chatbot

## Objective
To create an interactive and intelligent **Azure-based chatbot** using **Azure Bot Service**, **LUIS**, and **QnA Maker** to understand and respond to natural language queries.

## Technologies
- **Azure Bot Service**
- **Language Understanding (LUIS)**
- **QnA Maker**
- **Azure Speech SDK (optional)**
- **Azure Functions (optional)**

---

<div align="center">
    <svg width="100%" height="30">
        <rect width="100%" height="100%" fill="#4CAF50"/>
    </svg>
</div>

## Key Features

### 💬 Natural Language Processing
- Understands user queries using **LUIS** (Language Understanding Intelligent Service) to detect intent and entities.

<div align="center">
    <svg width="100%" height="30">
        <rect width="100%" height="100%" fill="#2196F3"/>
    </svg>
</div>

### 🧠 Knowledge Base Integration
- Leverages **QnA Maker** for fast, accurate responses to frequently asked questions.

<div align="center">
    <svg width="100%" height="30">
        <rect width="100%" height="100%" fill="#FFC107"/>
    </svg>
</div>

### 🎤 Voice Interaction (Optional)
- Integrates **Azure Speech SDK** to allow users to interact with the chatbot through voice commands, both voice-to-text and text-to-voice.

---

## Getting Started

### Prerequisites
- An **Azure account** to create and manage Azure resources.
- Familiarity with **Azure Bot Service** and **LUIS**.
- Basic knowledge of **Node.js** (or **C#** if you prefer .NET).

### Installation Steps

1. **Create an Azure Bot Service**
   - Log in to the Azure portal and navigate to **Bot Services**.
   - Click **Create** and fill in the necessary details to create a new bot service.
   - Choose the programming language (Node.js or C#) and the Bot Framework template.
   
2. **Create a Language Understanding (LUIS) Application**
   - Navigate to **LUIS** in the Azure portal and click on **Create a new LUIS app**.
   - Define **intents** (the purpose of the user's query) and **entities** (key pieces of information like names, dates, or places) for your bot.
   - Train and publish the LUIS model after defining intents and entities.

3. **Create a QnA Maker Knowledge Base**
   - Go to the **QnA Maker** portal and create a new knowledge base.
   - Add common questions and answers to the knowledge base that the bot can reference for quick responses.

4. **Configure the Bot**
   - Clone the repository and navigate to the project directory.
   - In the `.env` file, add your **LUIS** and **QnA Maker** credentials:
     ```plaintext
     LUIS_APP_ID=your_luis_app_id
     LUIS_API_KEY=your_luis_api_key
     LUIS_API_HOST_NAME=your_luis_endpoint
     QNA_KNOWLEDGE_BASE_ID=your_qna_knowledge_base_id
     QNA_ENDPOINT_KEY=your_qna_endpoint_key
     QNA_ENDPOINT_HOST=your_qna_endpoint_host
     ```

5. **Run the Bot Locally**
   - Install the required dependencies:
     ```bash
     npm install
     ```
   - Start the bot:
     ```bash
     npm start
     ```
   - Use the **Bot Framework Emulator** to test the bot locally by connecting to `http://localhost:3978/api/messages`.

6. **Deploy the Bot to Azure**
   - Once the bot works locally, deploy it to Azure via the Azure portal or using **GitHub Actions** for continuous integration and deployment.
   - Optionally, configure additional channels like **Microsoft Teams**, **Facebook Messenger**, or **Slack** to deploy your bot to multiple platforms.

---

## Contributing
Contributions are welcome! Feel free to submit issues or pull requests for any improvements or suggestions.

## License
This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

## Acknowledgments
- **Microsoft Azure** for providing the cloud services.
- **LUIS** and **QnA Maker** for making NLP and FAQ management easier.

---

## Contact
For inquiries or support, feel free to reach out to me at [mohammedrashwan.com](https://mohammedrashwan.com).
