# Clinton Math — deployable starter

This project contains a mobile-friendly maths solver interface and a Node.js backend.

## Deploy free with Render

You will need a GitHub repository to connect your code to Render.

1. Extract this ZIP file.
2. Create a GitHub repository named `clinton-math`. Keep it private if you prefer.
3. Upload the contents of this folder to the repository. Make sure `render.yaml`, `server.js`, `package.json`, and the `public` folder are at the top level.
4. In Render, choose **New → Blueprint** and connect the GitHub repository.
5. Render reads `render.yaml`. Confirm the free web service creation.
6. In the Render service settings, add `OPENAI_API_KEY` as an environment variable using a key managed by a parent/guardian. Never put the key in website code, a public repository, a screenshot, or a chat.
7. Wait for deployment to finish. Render will show your public `https://clinton-math.onrender.com`-style URL (the exact address depends on availability).

Official guide: https://render.com/docs/blueprint-spec
Node/Express guide: https://render.com/docs/deploy-node-express-app

## Local run (optional)

1. Install Node.js.
2. Run `npm install`.
3. Create `.env` from `.env.example` and set `OPENAI_API_KEY` privately.
4. Run `npm start`, then open `http://localhost:3000`.

## Important notes

- Render's free web services are free to host within the platform's limits, but they sleep after 15 minutes without traffic and can take about a minute to wake up.
- AI API usage is separate from hosting and may cost money. Check current pricing and usage limits with a parent/guardian before enabling it.
- Keep API keys private. The backend has a simple per-IP request limit, but this is not a substitute for monitoring API usage.
- The website is a starter project. AI-generated maths solutions can make mistakes; verify important work.
- Image uploads are sent to the configured AI model for analysis.
- The question history is currently kept only in the browser session and is not a shared online database.
