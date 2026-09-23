# OpenKernel

«An experimental Python-powered operating environment.»

OpenKernel is a small experimental project exploring how an operating-system-like environment can be built using Python.

It includes its own shell, system information tools, boot concepts, and an experimental desktop environment called dekx.

# 🚧 Status

OpenKernel is currently experimental and under development.

It is not a real operating-system kernel. The project is primarily an educational and experimental environment built with Python.

Things may change, break, or get completely redesigned. That's part of the fun. :)

# ✨ Features

- 🐚 Custom OpenKernel shell
- 🖥️ System and hardware information
- ⚡ CPU and display detection
- ⏱️ System uptime information
- 🖼️ Experimental "dekx" desktop environment
- 🚀 Experimental boot system
- 🧩 Modular project structure
- 🐍 Python-powered

# 📁 Project Components

Component| Description
"openkernel-core"| Core functionality
"openkernel-shell"| OpenKernel command-line shell
"openkernel-boot"| Experimental boot functionality
"openkernel-dekx"| Experimental desktop environment
"openkernel-utils"| Utility and helper functions

# 🖥️ dekx

dekx is OpenKernel's experimental graphical desktop environment.

The goal is to eventually provide a lightweight graphical interface for interacting with OpenKernel while keeping the project modular.

# 🛠️ Built With

- Python
- Standard Python libraries
- Additional Python packages where required

# 🚀 Getting Started

Clone the repository:

git clone https://github.com/uhwhatamityping/OpenKernel.git
cd OpenKernel

Create a virtual environment:

python -m venv .venv

Activate it on Linux/macOS:

source .venv/bin/activate

On Windows:

.venv\Scripts\activate

Install the dependencies:

pip install -r requirements.txt

Then run the project using the appropriate entry point.

«The project is still changing, so the exact startup command may change between versions.»

# 🗺️ Roadmap

- [x] Basic project foundation
- [x] CPU information
- [x] Display information
- [x] Initial shell
- [ ] Improve shell commands
- [ ] Improve hardware detection
- [ ] Develop "dekx"
- [ ] Improve boot system
- [ ] Add configuration system
- [ ] Improve modularity
- [ ] Add documentation
- [ ] Create a proper release system

# 🤝 Contributing

OpenKernel is an experimental project, and contributions are welcome.

If you want to experiment with the project:

1. Fork the repository
2. Create a branch
3. Make your changes
4. Test them
5. Open a pull request

# 📜 License

This project is currently experimental.

See the repository for the current license information.

# 💙 About

OpenKernel started as a small experiment in creating an operating-system-like environment with Python.

The project is about learning, experimenting, and seeing how far a Python-based environment can go.
