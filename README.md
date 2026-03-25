# AI-Powered-Code-Companion
Your personal coding assistant that suggests improvements, finds bugs, and writes documentation using NLP.
How to use it:
Open it in your web browser.
Click the "🔑 Set API Key" button and paste your OpenAI API key (it saves locally to your browser, never to a server).
Paste some messy code into the left panel and click Find Bugs, Refactor, or Write Docs!

What makes this code awesome:
Prompt Engineering: Instead of just sending raw code to the AI, it uses a dictionary object (prompts) to inject "System Prompts". This tells the AI to roleplay as an "expert debugger" or a "Senior Software Engineer," ensuring high-quality, formatted responses.
Markdown Injection: The AI returns raw text with triple backticks (```javascript). This code utilizes marked.js and highlight.js via CDN to instantly intercept that raw text and render it into beautiful, colorful code blocks right inside your sidebar.
Local Storage Security: Building API apps usually requires a backend server to hide the API key. Because this is a standalone HTML file, it prompts you for the key and uses localStorage to keep it safe in your own browser instance.
Architecture Simulation: This two-pane layout (Code on the left, Assistant on the right) is exactly how VS Code extensions (like GitHub Copilot Chat or Continue.dev) work. They take the text from the active editor window and pipe it into a Webview running JavaScript!
