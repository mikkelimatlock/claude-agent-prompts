# Claude Code agent prompts

A collection of custom Claude Code agents and output styles to enhance your coding workflow with specialized personas and formatting options.

## What's inside

This repository contains two main categories of prompts:

- **agents/** - custom Claude Code agent configurations with distinct personalities and specializations
- **output-styles/** - formatting and presentation styles that modify how Claude presents information

Each agent has a unique personality and expertise area, from architectural planning to rigorous code review. The output styles provide different ways to format and present Claude's responses to match your preferences or project needs.

## Directory structure

```
claude-agent-prompts/
├── agents/
│   ├── koivisto.md         # modular architecture specialist
│   ├── iseri.md            # code quality enforcer (*WIP*)
│   ├── rupert.md           # audio pipeline engineer (*WIP*)
│   └── aki.md              # documentation specialist (kind of functional)
└── output-styles/
    ├── koivisto.md         # architectural presentation style
    ├── koivisto-poet.md    # contemplative finnish forester-poet voice 
    └── iseri.md            # direct review formatting (*WIP*)
```

## Usage

### With Claude Code CLI

To use these agents and styles with Claude Code, you have a few options:

1. **copy content directly**: Copy the content from any `.md` file and paste it into your Claude conversation to activate that persona or style

2. **reference in prompts**: Mention which agent you want to use in your prompts (e.g., "use the koivisto agent to help me restructure this code")

3. **system configuration**: If Claude Code supports agent files, place the desired agent file in your Claude Code configuration directory

### Choosing the right agent

- Use **architectural agents** when planning project structure or refactoring messy codebases
- Use **review agents** when you need thorough code analysis and quality enforcement  
- Use **documentation agents** when creating or improving project documentation
- Mix and match agents based on your specific needs for each task

## Agent format

Each agent file follows this structure:

```markdown
---
name: agent-name
description: when and how to use this agent
model: preferred-model
color: display-color (optional)
---

[detailed agent persona and instructions]
```

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/claude-agent-prompts.git
   ```

2. Browse the `agents/` and `output-styles/` directories to find prompts that match your needs

3. Copy and use the prompts directly in your Claude Code sessions

## Contributing

We welcome contributions of new agents and output styles! When contributing:

1. Follow the existing file format and structure
2. Ensure your agent has a clear, specific purpose and expertise area
3. Provide helpful examples in the description frontmatter
4. Test your agent thoroughly before submitting
5. Add meaningful commit messages that describe what the agent does

### Adding new agents

1. Create your agent file in the `agents/` directory
2. Follow the frontmatter format with name, description, and optional model/color
3. Write clear, specific instructions that define the agent's personality and capabilities
4. Include concrete examples of when and how to use the agent

### Adding output styles

1. Create your style file in the `output-styles/` directory
2. Focus on presentation and formatting rather than personality
3. Ensure the style enhances readability and usability

## License

This project is released under the MIT license - feel free to use, modify, and distribute these prompts as needed.

## Questions or issues

If you have questions about using these agents or want to suggest improvements, please open an issue or start a discussion. We're always looking to improve the collection and make it more useful for developers.

---

*These prompts are designed to work with Claude Code and enhance your development workflow through specialized AI assistance.*