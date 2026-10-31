# Group-07
Group members:
William (wyuan12)
Tanmay (tanmayg6)

*Project Introduction*
Our project is meant to be a harness for AI agents, with simplicity, minimalism, and modularity in mind.  
We chose to work on this project because we wanted to take the opportunity to get more involved in tinkering with AI agents on a technical level and explore the viability of running AI models locally to get away from some of the limitations that come with subscriptions and telemetrics from large companies. 

*Technical Overview*

We roughly want to model the ReACt loop, described below, to design an effective harness:

----> Reason ----> Act ----> Observe ----> Repeat 

Reason
- The AI model (which we ideally want to let the user pick) is provided context about their objective and conversation history to decide the next course of action

Act
- The AI model acts on its environment, which can look like calling a tool/API, reading/writing to a file, running commands, or prompting the user (this is meant to keep the human in the loop). 

Observe
- Results in the form of the current state are fed back to the AI as context and the harness continues its loop 

We should also design a system prompt for the AI to direct its behavior

Tools
- We would like to keep the number of tools minimal and to avoid adding any more than necessary for the AI to function, but also support modularity for the end-user so they can add whatever tools they please 

Sandbox
- We've found it important to implement an isolated workspace where the AI can execute actions without affecting the user's environment itself in order to maintain user security  

Checkpoint 1 Goals
- Finish building the conversation loop
- Tool management
- Human-in-the-loop capability

Checkpoint 2 Goals
- 

*Possible Challenges*
I anticipate that it might be challenging writing an AI harness in Rust given that they usually tend to be written in Typescript, so it's possible that there are some subtleties that make Typescript better suited for creating an AI agent harness than Rust that need to be addressed for a minimally viable product. 

*References*
https://pi.dev/
