# Agentic AI App Hackathon Template

Welcome! This repository is your starting point for the **Agentic AI App Hackathon**. It includes:

- A consistent folder structure  
- An environment spec (`environment.yml` or `Dockerfile`)  
- A smoke-test script (`TEST.sh`)  
- Documentation placeholders to explain your design and demo

## 📋 Submission Checklist

- [ ] All code in `src/` runs without errors  
- [ ] `bash TEST.sh` completes successfully  
- [ ] `ARCHITECTURE.md` contains a clear diagram sketch and explanation  
- [ ] `EXPLANATION.md` covers planning, tool use, memory, and limitations  
- [ ] `DEMO.md` links to a 3–5 min video with timestamped highlights  


## 🚀 Getting Started

1. **Clone / Fork** this template.  
2. **Install dependencies**  
   ```bash
   # Conda
   conda env create -f environment.yml
   conda activate agentic-hackathon

   #—or Docker—
   docker build -t agentic-agent .
   docker run --rm -it agentic-agent bash

## 📂 Folder Layout

![Folder Layout Diagram](images/folder-layout.png)


---

## 2. `ARCHITECTURE.md`

```markdown
# Architecture Overview

Below, sketch (ASCII, hand-drawn JPEG/PNG pasted in, or ASCII art) the high-level components of your agent.

## Components

1. **User Interface**  
   - E.g., Streamlit, CLI, Slack bot  

2. **Agent Core**  
   - **Planner**: how you break down tasks  
   - **Executor**: LLM prompt + tool-calling logic  
   - **Memory**: vector store, cache, or on-disk logs  

3. **Tools / APIs**  
   - E.g., Web search, calculator, database, custom endpoints  

4. **Observability**  
   - Logging of each reasoning step  
   - Error handling / retries  

