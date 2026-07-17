# Collaborative ChatGPT prompts

This repository holds my ongoing work to create a working LLM prompt to do collaborative work on poor and/or unreliable documentation.

### Overview

- protocol.md sets the overall goal, a collaborative session where available sources are tested before they are added to the knowledge base. Basically it defines HOW we reason-
- RATIONALE.md explains WHY the protocol is structured as it is.
- project-state.md and session-log.md are placeholders on top level. As you work you record information about your findings in them.
- projects contain work done on TECO and Macro assembler on TOPS-20. 

### Instruction

To start a new project, upload protocol.md, RATIONALE.md and top level project-state.md and session-log.md. The LLM should be able to pick up from there and get going once you provide information on what you want to research, or dig into.  
The prompt works really good when you "learn as you go along", assisted by the LLM.

For existing projects you can restart a prompt with the protocol, RATIONALE and updated project state/session log that capture where you are in the project.

### Development

Using the protocol will allow the LLM to add domain-specific knowledge in new files, such as mental-model.md, architecture.md etc. It should, however, hold off from such changes until clear patterns emerge.  
Do assist it to make good decisions on this matter.
