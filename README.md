# 🤖 LLM Chatbot on Internet Computer

A powerful and intelligent chatbot built on the Internet Computer Protocol (ICP) that leverages Large Language Models (LLMs) to provide smart, context-aware conversations.

![Chatbot Demo](frontend/public/bot.svg)

## ✨ Features

- 🧠 Advanced Language Understanding: Powered by Large Language Models
- 🔗 Blockchain Integration: Built on Internet Computer Protocol
- 💬 Interactive Conversations: Natural and context-aware responses
- 🚀 Real-time Processing: Quick and efficient response generation
- 🎨 Modern UI: Clean and responsive user interface
- 🔒 Secure: Built with ICP security best practices

## 🛠️ Technology Stack

- **Backend**
  - Internet Computer Protocol (ICP)
  - Motoko programming language
  - Ollama LLM server

- **Frontend**
  - React.js
  - Tailwind CSS
  - Vite build tool

## 🚀 Quick Start

### Prerequisites

1. Install the [Internet Computer SDK (DFX)](https://internetcomputer.org/docs/building-apps/getting-started/install)
2. Install [Node.js](https://nodejs.org/) (version 16 or higher)
3. Install [Ollama](https://ollama.com/) for local LLM processing

### Setting Up Ollama

1. Start the Ollama server:
   ```bash
   ollama serve
   ```
   The server will start listening on port 11434

2. Download and set up the LLM model:
   ```bash
   ollama run llama3.1:8b
   ```
   This will download an 8B parameter model (~4GiB)

### Project Setup

1. **Clone the Repository**
   ```bash
   git clone <repository-url>
   cd LLM-Chatbot
   ```

2. **Install Dependencies**
   ```bash
   npm install
   cd frontend
   npm install
   ```

3. **Deploy Locally**
   ```bash
   dfx start --background --clean
   dfx deploy
   ```

## 🌟 Usage

1. **Start the Development Server**
   ```bash
   npm start
   ```

2. **Access the Application**
   - Open your browser and navigate to `http://localhost:8080`
   - Start chatting with the bot!

## 🎯 Features in Detail

### Smart Contract Integration
The chatbot leverages ICP smart contracts to:
- Process user inputs securely
- Generate contextual responses
- Maintain conversation history
- Ensure data integrity

### LLM Processing
- Uses advanced language models for natural conversations
- Maintains context across multiple exchanges
- Provides informative and relevant responses

### User Interface
- Clean and intuitive design
- Real-time response updates
- Mobile-responsive layout
- Easy-to-use chat interface

## 🔧 Configuration

### Environment Variables
Create a `.env` file in the root directory:
```env
DFX_NETWORK=local
OLLAMA_HOST=http://localhost:11434
```

### Custom Model Configuration
You can configure different LLM models in `dfx.json`:
```json
{
  "llm": {
    "model": "llama2",
    "parameters": {
      "temperature": 0.7,
      "max_tokens": 200
    }
  }
}
```

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 🔍 Troubleshooting

### Common Issues

1. **Ollama Server Connection Issues**
   - Ensure Ollama is running (`ollama serve`)
   - Check if the correct port (11434) is accessible

2. **Deployment Problems**
   - Verify DFX is installed and running
   - Check network connectivity
   - Ensure all dependencies are installed

3. **Frontend Issues**
   - Clear browser cache
   - Update Node.js to the latest version
   - Reinstall node_modules if necessary

## 📚 Additional Resources

- [Internet Computer Documentation](https://internetcomputer.org/docs)
- [Motoko Programming Language Guide](https://internetcomputer.org/docs/language-guide/motoko/)
- [Ollama Documentation](https://ollama.com/docs)
- [React.js Documentation](https://reactjs.org/)

## 🔐 Security Best Practices

We implement several security measures:

1. Input Validation
2. Rate Limiting
3. Secure Communication
4. Data Encryption
5. Access Control

For more details, refer to the [ICP security best practices](https://internetcomputer.org/docs/building-apps/security/overview).

## ⭐ Support the Project

If you find this project helpful, please give it a star on GitHub and share it with others!
