# LLM Configuration

This document details the Large Language Model (LLM) integration used for AI assistance in the Python Fantasy application.

## AI Provider Details
- **Provider:** OpenTyphoon
- **Base URL:** `https://api.opentyphoon.ai/v1`
- **Model:** `typhoon-v2.5-30b-a3b-instruct`

## API Configuration
```javascript
const OPENAI_API_KEY = "sk-FhFTncXbdxjDjZB9xTxsClgMFNSHpshCMaeJjj9gssnHNujq";
const OPENAI_BASE_URL = "https://api.opentyphoon.ai/v1";
const OPENAI_MODEL = "typhoon-v2.5-30b-a3b-instruct";
```

## AI Features
The application implements the following AI-powered functions within the "Forge" section:
- **Analyze with AI:** Explains the provided Python code to the user.
- **Fix with AI:** Analyzes errors in the console output and suggests fixes for the code.
