# Grunty - Computer AI Agent

Self-hosted desktop app to have AI control your computer, powered by the new Claude computer use capability. Allow Claude to take over your laptop and do your tasks for you (or at least attempt to, lol). Written in Python, using PyQt.

## ⚠️ Important Disclaimers

1. **This is experimental software** - It gives an AI control of your mouse and keyboard. Things can and will go wrong.

2. **Tread Lightly** - If it wipes your computer, sends weird emails, or orders 100 pizzas... that's on you. 

Anthropic can see your screen through screenshots during actions. Hide sensitive information or private stuff.

## 🎯 Features
- Literally ask AI to do ANYTHING on your computer that you do with a mouse and keyboard. Browse the web, write code, blah blah.

# 💻 Platforms
- Anything you can run Python on: MacOS, Windows, Linux, etc.

## 🛠️ Setup

Get an Anthropic API key [here](https://console.anthropic.com/keys).

```bash
# Python 3.10+ recommended
python -m venv venv
source venv/bin/activate  # or `venv\Scripts\activate` on Windows
pip install -r requirements.txt

# Add API key to .env
echo "ANTHROPIC_API_KEY=your-key-here" > .env

# Run
python run.py
```

## 🔑 Productivity Keybindings
- `Ctrl + Enter`: Execute the current instruction
- `Ctrl + C`: Stop the current agent action
- `Ctrl + W`: Minimize to system tray
- `Ctrl + Q`: Quit application

## 💡 Tips
- Claude really loves Firefox. You might want to install it for better UI detection and accurate mouse clicks.
- Be specific and explicit, help it out a bit
- Always monitor the agent's actions

## 🐛 Known Issues

- Sometimes, it doesn't take a screenshot to validate that the input is selected, and types stuff in the wrong place.. Press CMD+C to end the action when this happens, and quit and restart the agent. I'm working on a fix.

## 🤝 Contributing

Issues and PRs are most welcome! Made this is in a day so don't really have a roadmap in mind. Hmu on Twitter @ishanxnagpal if you're got interesting ideas you wanna share. 

## 📄 License

[Apache License 2.0](LICENSE)

---