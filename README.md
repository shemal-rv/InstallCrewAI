# Setting Up CrewAI with Python

Follow these steps to set up CrewAI on your system.

## Prerequisites

- Ensure you have Python version **>=3.10** and **<=3.13** installed on your system.
- If Python is not installed or is not within the required version range, download the appropriate version from [Python's official website](https://www.python.org/downloads/).

## Installation Steps

### 1. Install CrewAI and CrewAI Tools

Open your terminal and run the following command to install CrewAI:

```bash
pip install crewai crewai-tools
```
2. Verify Installation
To confirm that CrewAI was installed correctly, execute the following command in your terminal:

pip freeze | grep crewai
You should see output similar to the following, which confirms the versions installed:

crewai==X.X.X
crewai-tools==X.X.X
3. Create a New CrewAI Project
Run this command to create a new CrewAI project. Replace <project_name> with your desired project name.

crewai create crew <project_name>
4. Set Environment Variables
Navigate to your project directory and set up your environment variables:

Change into your project directory:

cd <project_name>
Create a .env file and add your OpenAI API key (ensure it starts with sk-).

echo "OPENAI_API_KEY=sk-..." > .env
5. Install Project Dependencies
Finally, install the necessary dependencies for your CrewAI project:

crewai install
Your CrewAI project is now set up and ready for development!

