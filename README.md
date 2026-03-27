# Claude Style CLI

![cli](https://img.shields.io/badge/cli-blue?style=flat-square) ![ui](https://img.shields.io/badge/ui-blue?style=flat-square) ![ux](https://img.shields.io/badge/ux-blue?style=flat-square)

A rich CLI for agents featuring progress bars, markdown rendering, and interactive prompts.

## Overview
Claude Style CLI is a Python-based framework designed to bring the polished user experience of modern AI web interfaces to the terminal. It provides a robust suite of UI components specifically tailored for autonomous agents and LLM-powered applications, ensuring that complex background tasks are communicated clearly to the user through elegant visual feedback.

## Features
*   **Live Markdown Rendering:** Beautifully formatted text outputs with support for syntax highlighting and tables.
*   **Dynamic Progress Tracking:** Multi-stage progress bars and spinners to visualize long-running agentic workflows.
*   **Interactive Prompts:** User-friendly input handling including confirmation dialogs and selection menus.
*   **Rich Layouts:** Panel-based output to separate system logs from primary agent responses.

## Installation
Ensure you have Python 3.8+ installed. Clone the repository and install the necessary dependencies:

```bash
git clone https://github.com/yourusername/claude-style-cli.git
cd claude-style-cli
pip install -r requirements.txt
```

## Usage
Run the main demonstration script to see the UI components in action:

```bash
python main.py
```

Example integration in your code:
```python
from claude_cli import UI

ui = UI()
ui.print_markdown("# Agent Status\nProcessing your request...")
with ui.progress("Thinking...") as p:
    # Your agent logic here
    p.update(completed=100)
```

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request, report bugs via Issues, or suggest new UI components that could improve the agentic terminal experience.

## License
This project is licensed under the [MIT License](LICENSE).