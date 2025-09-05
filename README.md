<!-- This is an image banner. It's a great way to make a big, custom title. -->
#SOUNIC -AI CHATBOT
A personal AI chat assistant built from scratch with a modern UI, a secure serverless backend, and powered by the high-speed Groq API. This project was built as a hands-on learning experience to understand the full lifecycle of a modern web application, from frontend design to backend deployment.

Check out the live demo: https://sounicai.netlify.app/ (<- Replace with your actual Netlify link)

Key Features
Interactive & Modern UI: A clean, professional, and fully responsive user interface inspired by today's leading AI platforms.

Blazing Fast Responses: Integrated with the Groq API and Llama 3.1 model for near-instantaneous AI-generated text.

Custom AI Persona: The AI has a unique, pre-defined personality and custom knowledge base, configured via server-side prompt engineering.

Secure Serverless Backend: Uses Netlify Functions to manage API calls, ensuring the secret API key is never exposed on the client-side.

Full Functionality: Includes a sleek Dark/Light mode toggle, a "New Chat" button to reset the conversation, and clickable prompt suggestions.

Dynamic UI Elements: Features an auto-resizing text input and a "typing" effect for AI responses to create a fluid user experience.

Tech Stack
This project is built with a focus on simplicity and modern web standards, without relying on heavy frameworks.

Frontend: HTML5, CSS3 (with CSS Variables for theming), Vanilla JavaScript (ES6+)

Backend: Serverless Functions on Netlify (Node.js runtime)

AI Model: Llama 3.1 via the Groq API

Deployment: Hosted on Netlify

The Learning Journey
This project started as a simple question: "How does an API actually work?" It evolved from a basic fetch call to a full-stack application.

The most significant learning experience was encountering and overcoming real-world development challenges. Initially built on the Google Gemini API, the project faced hard rate limits (429 errors). This led to a crucial pivot: I researched alternative services and successfully migrated the entire backend to the Groq API, learning how to adapt to different API structures while dramatically improving performance. Debugging server-side function logs on Netlify to solve deployment and environment variable issues was also a critical part of the learning process.

How to Run This Project Locally
To run SounicAI on your own machine, follow these steps:

1. Clone the Repository

git clone [https://github.com/your-username/sounic-ai-assistant.git](https://github.com/your-username/sounic-ai-assistant.git)
cd sounic-ai-assistant

2. Install Dependencies
This project requires node-fetch for the serverless function. You'll also need the Netlify CLI to run the development environment.

# Install node-fetch
npm install

# Install Netlify CLI globally if you haven't already
npm install netlify-cli -g

3. Set Up Your Environment Variables

Create a new file in the root of the project folder named .env.

Get your free API key from Groq.

Add your key to the .env file like this:

GROQ_API_KEY=gsk_YourSecretApiKeyGoesHere

4. Start the Development Server
Use the Netlify CLI to run the local server. This will serve your HTML and run your serverless function simultaneously.

netlify dev
