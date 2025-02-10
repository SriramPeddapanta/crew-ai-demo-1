# 🚀 Project Setup Guide

This guide provides step-by-step instructions to set up and run the project.

## 🛠️ Setup Instructions

1. **📥 Install Rye**  
   Run the following command to install Rye:
   ```bash
   curl -sSf https://rye.astral.sh/get | bash
   ```

2. **⚙️ Initialize the Project**  
   Initialize the project in the current directory:
   ```bash
   rye init .
   ```

3. **🔄 Sync Dependencies**  
   Synchronize the dependencies:
   ```bash
   rye sync
   ```

4. **🛠️ Add Required Tools**  
   Add the necessary tools for the project:
   ```bash
   rye add 'crewai[tools]'
   ```

5. **🤖 Create the AI Development Environment**  
   Use the `crewai` tool to create the development environment:
   ```bash
   rye run crewai create crew latest-ai-development
   ```

6. **📂 Navigate to the Development Directory**  
   Change into the newly created directory:
   ```bash
   cd latest_ai_development
   ```

7. **🔄 Resynchronize Dependencies**  
   Sync the dependencies again:
   ```bash
   rye sync
   ```

8. **🔧 Reinstall CrewAI**  
   Reinstall CrewAI to ensure all components are properly set up:
   ```bash
   rye run crewai install
   ```

9. **🏃‍♂️ Run the Project**  
   Start the project using the following command:
   ```bash
   rye run crewai run
   ```

## ✨ Customization

- **🔑 Add your `OPENAI_API_KEY`** into the `.env` file located in the `latest_ai_development` directory.
- Modify the following files to customize the project:
  - `📄 src/latest_ai_development/config/agents.yaml` to define your agents.
  - `📄 src/latest_ai_development/config/tasks.yaml` to define your tasks.
  - `📄 src/latest_ai_development/crew.py` to add your own logic, tools, and specific arguments.
  - `📄 src/latest_ai_development/main.py` to add custom inputs for your agents and tasks.

## 📝 Notes

- Ensure all commands are executed in the correct order to avoid setup issues.
- If you encounter any errors, refer to the documentation or check the logs for troubleshooting.
