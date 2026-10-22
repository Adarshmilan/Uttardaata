# 📞 Uttardaata – AI Phone Call Assistant

> 🚧 **Status: planning stage.** This repository currently holds the project plan and learning roadmap – no code yet.

**Uttardaata** (उत्तरदाता, "the one who answers") is an AI that answers phone calls. Someone calls a number, the AI picks up, listens, thinks and replies out loud like a human.

## 🧠 How it will work

```
📱 Caller dials number
      │
      ▼
☎️  Twilio receives the call
      │
      ▼
🎙️  Speech-to-Text (Whisper / Google)   →  caller's words as text
      │
      ▼
🤖  LLM generates a reply
      │
      ▼
🔊  Text-to-Speech (gTTS / pyttsx3 / Amazon Polly)
      │
      ▼
📱 Caller hears the answer
```

## 🛠️ Planned tech stack

| Tool | Why |
|------|-----|
| HTML, CSS | Simple website / dashboard |
| Python + Flask | Backend server that handles Twilio webhooks |
| Twilio | Phone number and incoming calls |
| Whisper / Google Speech-to-Text (`SpeechRecognition`) | Convert the caller's voice to text |
| OpenAI GPT (or another LLM) | Generate a smart reply |
| gTTS / pyttsx3 / Amazon Polly | Convert the reply back to speech |
| Render or Railway | Host the app online |

## 🌱 Roadmap

- [ ] Learn the basics: HTML, CSS, Python, Flask
- [ ] Set up a Twilio number and answer a call with a fixed message
- [ ] Add speech-to-text for the caller's words
- [ ] Connect an LLM to generate replies
- [ ] Add text-to-speech and play the reply on the call
- [ ] Support multi-turn conversations
- [ ] Deploy to Render / Railway

## 📚 Learning resources

- Python, HTML, CSS, Flask – beginner tutorials on YouTube
- [Twilio Voice docs](https://www.twilio.com/docs/voice)
- [SpeechRecognition (Python)](https://pypi.org/project/SpeechRecognition/)
- [OpenAI API docs](https://platform.openai.com/docs)
