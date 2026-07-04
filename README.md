# Project README

## Overview
This is a Python-based local system assistant designed to help with system tasks and occasional research. It features a strict tool usage policy to ensure safe and efficient operation.

## Key Features
- **System Task Automation**: Executes shell commands, manages files, and interacts with the environment.
- **Research Capabilities**: Utilizes DuckDuckGo search and Wikipedia for external information.
- **Interactive Shell**: Maintains persistent state across sessions with safety checks for sensitive operations.
- **Modular Architecture**: Core components are separated into distinct modules for maintainability.

## Project Structure
```
.
├── data/                # Directory for research outputs and persistent data
├── .env                  # Environment variables configuration
├── .git/                # Git version control files
├── main.py               # Primary application logic and agent setup
├── old/                  # Directory for deprecated or archived files
├── __pycache__/         # Python compiled bytecode
├── readme.md             # This README file (to be renamed to README.md)
├── requirements.txt      # Python package dependencies
├── shell.py              # Persistent shell management implementation
├── tools.py              # Tool implementations and safety checks
└── ui.py                 # Terminal user interface formatting and prompts
```

## Getting Started
1. **Setup**: Ensure Python virtual environment is activated and dependencies are installed (`pip install -r requirements.txt`)
2. **Configuration**: Set environment variables in `.env` file (e.g., API keys for LLM services)
3. **Execution**: Run the assistant with `python main.py`

## Safety Policies
- **Tool Usage**: Tools are only called when strictly necessary; most responses are generated without external calls
- **Interactive Commands**: Commands requiring keyboard input must be run manually in a terminal
- **Sensitive Operations**: Commands that modify the system or data require explicit user confirmation

## Dependencies
- Python 3.x
- LangChain
- OpenAI API (for LLM functionality)
- DuckDuckGo Search API
- Wikipedia API
- Python-dotenv
- Pydantic
- Subprocess execution capabilities

## Contributing
Contributions are welcome! Please ensure:
- Code follows PEP8 conventions
- New features include unit tests
- Documentation is updated accordingly

## License
This project is licensed under the MIT License.

## Contact
For questions or support, please contact the project maintainer at [insert contact information].