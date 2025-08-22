# claude code agent prompts

a collection of custom Claude Code agents and output styles to enhance your coding workflow with specialized personas and formatting options.

## what's inside

this repository contains two main categories of prompts:

- **agents/** - custom Claude Code agent configurations with distinct personalities and specializations
- **output-styles/** - formatting and presentation styles that modify how Claude presents information

each agent has a unique personality and expertise area, from architectural planning to rigorous code review. the output styles provide different ways to format and present Claude's responses to match your preferences or project needs.

## directory structure

```
claude-agent-prompts/
├── agents/
│   ├── koivisto.md         # modular architecture specialist
│   ├── iseri.md            # code quality enforcer
│   ├── rupert.md           # audio pipeline engineer
│   └── aki.md              # documentation specialist
└── output-styles/
    ├── koivisto.md         # architectural presentation style
    └── iseri.md            # direct review formatting
```

## usage

### with Claude Code CLI

to use these agents and styles with Claude Code, you have a few options:

1. **copy content directly**: copy the content from any `.md` file and paste it into your Claude conversation to activate that persona or style

2. **reference in prompts**: mention which agent you want to use in your prompts (e.g., "use the koivisto agent to help me restructure this code")

3. **system configuration**: if Claude Code supports agent files, place the desired agent file in your Claude Code configuration directory

### choosing the right agent

- use **architectural agents** when planning project structure or refactoring messy codebases
- use **review agents** when you need thorough code analysis and quality enforcement  
- use **documentation agents** when creating or improving project documentation
- mix and match agents based on your specific needs for each task

## agent format

each agent file follows this structure:

```markdown
---
name: agent-name
description: when and how to use this agent
model: preferred-model
color: display-color (optional)
---

[detailed agent persona and instructions]
```

## installation

1. clone this repository:
   ```bash
   git clone https://github.com/yourusername/claude-agent-prompts.git
   ```

2. browse the `agents/` and `output-styles/` directories to find prompts that match your needs

3. copy and use the prompts directly in your Claude Code sessions

## contributing

we welcome contributions of new agents and output styles! when contributing:

1. follow the existing file format and structure
2. ensure your agent has a clear, specific purpose and expertise area
3. provide helpful examples in the description frontmatter
4. test your agent thoroughly before submitting
5. add meaningful commit messages that describe what the agent does

### adding new agents

1. create your agent file in the `agents/` directory
2. follow the frontmatter format with name, description, and optional model/color
3. write clear, specific instructions that define the agent's personality and capabilities
4. include concrete examples of when and how to use the agent

### adding output styles

1. create your style file in the `output-styles/` directory
2. focus on presentation and formatting rather than personality
3. ensure the style enhances readability and usability

## license

this project is released under the MIT license - feel free to use, modify, and distribute these prompts as needed.

## questions or issues

if you have questions about using these agents or want to suggest improvements, please open an issue or start a discussion. we're always looking to improve the collection and make it more useful for developers.

---

*these prompts are designed to work with Claude Code and enhance your development workflow through specialized AI assistance.*