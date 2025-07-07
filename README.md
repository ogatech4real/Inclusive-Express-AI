# Inclusive Express AI — Voice-Driven, Accessible Design Add-on for Adobe Express

[Inclusive Express AI](https://www.youtube.com/watch?v=Yd8-qJpBL6Y)

Inclusive Express AI is an AI-powered, voice-driven Add-on for Adobe Express that helps anyone — regardless of ability, technical skill, or experience — create stunning, accessible designs simply by speaking.

Millions of people, including parents, teachers, community leaders, and individuals with disabilities, struggle with design tools due to complexity, time constraints, or accessibility limitations. Inclusive Express AI eliminates those barriers, enabling effortless, inclusive design for all.

---

## What It Does

Inclusive Express AI integrates directly into Adobe Express, providing:

-  **Voice-Driven Design Interaction** — Users speak naturally, and the AI listens, understands, and generates designs  
-  **Built-in Accessibility Features** — The Add-on applies WCAG accessibility standards like proper color contrast, readable fonts, and layout improvements  
-  **Conversational AI Intelligence** — Using OpenAI’s API, the AI understands complex requests, asks follow-up questions, and personalizes design suggestions  
-  **Real-Time Design Preview** — See live updates as you interact with the Add-on through voice  
-  **Inclusive for All Users** — Designed for parents, teachers, busy individuals, and disabled users who need simple, effective design tools  
-  **Hands-Free Control** — Users with mobility or visual impairments can design without using traditional input methods  

---

##  How It Works

1. Launch Inclusive Express AI within Adobe Express  
2. The AI assistant welcomes the user with a voice prompt  
3. The user describes their design needs (e.g., "Create a colorful flyer for our school fundraiser, accessible to elderly parents")  
4. The AI processes the request with speech recognition, applies accessibility best practices, and shows a real-time design preview  
5. OpenAI's API powers conversational intelligence — the AI provides suggestions, asks clarifying questions, and guides the user to completion  
6. Users can continue editing by voice or finalize the design with confidence  

---

##  Live Demo & Testing

-  [Deployed Prototype on Netlify](https://inclusive-express-ai.netlify.app/)  
-  [Adobe Express Playground](https://developer.adobe.com/express/add-ons/playground/) — Load with HTTPS on port `5241` for local testing  

---

##  Tech Stack & Tools

- [React](https://react.dev/) — Frontend framework  
- [Vite](https://vitejs.dev/) — Development tooling and bundler  
- [Tailwind CSS](https://tailwindcss.com/) — Utility-first styling  
- [Web Speech API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Speech_API) — Speech-to-Text (STT) and Text-to-Speech (TTS)  
- [OpenAI API](https://platform.openai.com/) — Conversational AI integration  
- [Adobe Express Add-ons Framework](https://developer.adobe.com/express/add-ons/) — Official Add-on environment  

---

##  Project Structure

```plaintext
inclusive-express-ai/
├── .bolt/               # Bolt.new project config
├── dist/                # Production build output
├── src/                 # Application source code
├── index.html           # Main HTML entry
├── manifest.json        # Required for Adobe Express Add-ons
├── vite.config.ts       # Dev server and HTTPS config
├── package.json         # Project metadata and scripts
└── README.md            # Project documentation

---

🏁 Getting Started (Local Development)

1️⃣ Clone the Repository
bash
git clone https://github.com/yourusername/inclusive-express-ai.git
cd inclusive-express-ai

2️⃣ Install Dependencies
bash
npm install

3️⃣ Generate Trusted Local Certificates (For HTTPS Testing)
bash
mkcert -install
mkcert localhost
Place localhost.pem and localhost-key.pem in the project root directory.

4️⃣ Configure Development Server
Ensure vite.config.ts includes:

ts

server: {
  https: {
    key: fs.readFileSync('./localhost-key.pem'),
    cert: fs.readFileSync('./localhost.pem'),
  },
  port: 5241,
}

5️⃣ Run the Development Server
bash
npm run dev
Access the Add-on at:

plaintext
https://localhost:5241

6️⃣ Load in Adobe Express Playground
Go to https://developer.adobe.com/express/add-ons/playground/

Enter your https://localhost:5241 URL

---

## Future Improvements

Expand AI reasoning with deeper OpenAI integration
Enhanced accessibility checks based on WCAG standards
More design templates and inclusive content options
Real-world testing with parents, teachers, disabled users, and community groups
Mentor collaboration for production-ready Adobe Express Add-on deployment

---

## Acknowledgments

Thanks to:
Adobe Express Add-ons Team
OpenAI
React, Vite, and Tailwind Communities

---

👤 About the Author
Adewale Ogabi — AI and Accessibility Enthusiast, Developer passionate about empowering users through inclusive technology.
