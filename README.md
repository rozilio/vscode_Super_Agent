# VSCode Super Agent

A framework for managing and utilizing a "memory bank" to provide context to an AI agent within a project. This allows the agent to maintain a deep understanding of the project's goals, technical stack, and ongoing progress.

## Getting Started

There are two options to set up the project environment.

### Option A: Automatic Initialization

This option uses the agent to create and initialize all the necessary files.

1.  **Open a new or existing project** in your IDE.
2.  **Copy the `main.instructions.md` file** to the following directory (create the path if it does not exist):
    ```
    C:\<YOUR_PROJECT_DIRECTORY>\.github\instructions\
    ```
3.  **In PLAN MODE, issue the following command:**
    ```
    initialize memory bank and create all the core and optional files
    ```
4.  **Switch to ACT MODE** and approve the agent's actions.

### Option B: Manual Setup

This option involves manually setting up the file structure.

1.  **Copy the `main.instructions.md` file** to the following directory (create the path if it does not exist):
    ```
    C:\<YOUR_PROJECT_DIRECTORY>\.github\instructions\
    ```
2.  **Copy the `memory-bank` directory** to the root of your project:
    ```
    C:\<YOUR_PROJECT_DIRECTORY>\
    ```

## Project Structure

The `memory-bank` directory is the core of this framework. It is structured as follows:

```
<YOUR_PROJECT_DIRECTORY>
├── memory-bank/
     ├── projectbrief.md          (Foundation - created first)
     ├── productContext.md        (Built from projectbrief)
     ├── systemPatterns.md        (Built from projectbrief)
     ├── techContext.md           (Built from projectbrief)
     ├── activeContext.md         (Built from the three files above)
     ├── progress.md              (Built from activeContext)
     └── tasks/
         └── _index.md            (Task management system)
```
flowchart TD
    PB[projectbrief.md] --> PC[productContext.md]
    PB --> SP[systemPatterns.md]
    PB --> TC[techContext.md]
    
    PC --> AC[activeContext.md]
    SP --> AC
    TC --> AC
    
    AC --> P[progress.md]
    AC --> TF[tasks/ folder]

This hierarchical structure ensures that the agent has a layered and comprehensive understanding of the project at all times.
