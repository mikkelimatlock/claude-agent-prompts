# Claude Code configuration

this file contains useful configuration and instructions for working with the custom agent prompts in this repository using Claude Code.

## recommended workflow

when working with this repository of custom agents and output styles, here are some suggested approaches:

### agent selection strategy

1. **identify your task type** - determine whether you need architectural planning, code review, documentation, or specialized assistance
2. **match to agent expertise** - review the agent descriptions to find the best fit for your specific needs  
3. **activate before starting** - load the chosen agent at the beginning of your session for consistent personality and approach
4. **combine when needed** - some tasks benefit from multiple agents (e.g., architectural planning followed by code review)

### session management

```markdown
# start of session - activate your chosen agent
load agent: haruki  # for architectural work

# or reference directly
use the nina agent to review this authentication code for security issues

# switch agents mid-session if needed  
switch to lowercase-docs-writer agent for documentation
```

### file organization tips

- keep agent files easily accessible in your Claude Code workspace
- consider creating shortcuts or aliases for frequently used agents
- organize agents by project type or development phase for quick selection

## integration suggestions

### with existing workflows

these agents work well alongside standard development practices:

- **code review**: use nina agent for thorough pre-commit reviews
- **architecture planning**: engage haruki agent during design phases  
- **documentation**: activate lowercase-docs-writer agent for README and doc updates
- **refactoring sessions**: combine architectural and review agents for comprehensive code improvements

### project-specific usage

consider dedicating specific agents to different types of projects:

- **web applications**: architectural agents for structure, review agents for security
- **data processing**: focus on error handling and performance review agents
- **documentation sites**: primarily documentation and style agents
- **open source projects**: balance technical excellence with clear, approachable documentation

## agent customization

### modifying existing agents

when adapting agents for your specific needs:

1. **preserve core personality** - keep the distinctive voice and approach that makes each agent unique
2. **adjust expertise areas** - modify technical focus areas to match your domain (e.g., web dev vs data science)  
3. **update examples** - replace generic examples with ones relevant to your codebase or industry
4. **maintain format consistency** - keep the frontmatter structure for compatibility

### creating new agents

follow this checklist when developing custom agents:

- [ ] clear, specific expertise area that fills a gap
- [ ] distinctive personality that guides communication style  
- [ ] concrete examples of when to use the agent
- [ ] actionable instructions for the agent's approach
- [ ] proper frontmatter with name, description, model preference
- [ ] testing with real scenarios to verify effectiveness

## technical considerations

### model preferences

some agents may work better with specific Claude models:

- **complex reasoning tasks**: consider sonnet models for architectural planning
- **rapid iteration**: haiku models for quick reviews and formatting
- **balanced approach**: sonnet models provide good performance for most agent types

### performance optimization

- **agent switching**: minimize mid-conversation agent changes to maintain consistency
- **context management**: provide relevant codebase context when activating agents
- **session length**: longer sessions allow agents to build better understanding of your project

## troubleshooting

### common issues

**agent not responding as expected**:
- verify the full agent prompt was loaded correctly
- check that your request matches the agent's expertise area
- provide more specific context about your codebase or requirements

**inconsistent personality**:
- avoid mixing multiple agent personalities in the same conversation
- re-load the agent prompt if behavior becomes generic
- ensure your prompts align with the agent's intended use cases

**poor code suggestions**:
- provide more context about your project structure and constraints
- specify the programming language and framework you're using
- include relevant code snippets for better understanding

### getting better results

1. **be specific about context** - mention your tech stack, project type, and current challenges
2. **align requests with expertise** - use architectural agents for structure, review agents for quality
3. **provide code examples** - agents work better when they can see actual code rather than abstract descriptions
4. **iterate and refine** - don't hesitate to ask follow-up questions or request clarification

---

*this configuration guide helps you get the most out of the custom Claude Code agents in this repository. adjust and extend these recommendations based on your specific development workflow and needs.*