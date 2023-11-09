```mermaid
---
title: Goose Framework
---
flowchart TB
    Agent
    Threads
    Message
    User
    Planner
    Step
    Executor
    Action
    Tool
    decisionLoop(Decision Loop)

    User --> Threads
    Agent --> Threads
    Threads --> Message
    Agent --> Planner
    Planner --> Step
    Agent --> decisionLoop
    Agent --> Executor
    Executor --> Action
    Action --> Tool
```
