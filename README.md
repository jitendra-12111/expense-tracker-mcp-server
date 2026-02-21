# Expense Tracker MCP Server

An **Expense Tracker MCP (Model Context Protocol) server** that enables expense tracking tools to integrate with MCP-compatible clients such as Claude Desktop. This server provides a structured interface for managing and testing expense-related operations.

---

## 📌 Overview

The **Expense Tracker MCP Server** allows you to:

* Run an MCP-compatible expense tracking service
* Integrate with Claude Desktop
* Test tools locally using an inspector
* Host the MCP server on a local port
* Enable structured tool execution through MCP

This project is useful for building, testing, and deploying MCP-based expense tracking workflows.

---

## ⚙️ Prerequisites

Before setting up the project, ensure you have:

* **Python 3.9+**
* **uv package manager** installed
  Install from: https://docs.astral.sh/uv/
* Basic knowledge of MCP tools (optional)

---

## 🚀 Installation

### 1. Initialize the Project

```bash
uv init
```

### 2. Install Dependencies

```bash
pip install fastmcp
```

Or using `uv`:

```bash
uv pip install fastmcp
```

---

## 🔌 Install Tool in Claude Desktop (First-Time Setup)

To register and install the MCP tool in **Claude Desktop**, run:

```bash
uv run fastmcp install claude-desktop main.py
```

This command connects your MCP server with Claude Desktop so it can access and execute the tool.

---

## 🧪 Development & Testing

### Run Local Inspector (Recommended for Testing)

Use the MCP inspector to test your tool locally:

```bash
uv run fastmcp dev inspector main.py
```

This starts a local development interface where you can:

* Test tool behavior
* Debug requests/responses
* Verify MCP integration

---

## ▶️ Running the MCP Server

### Start the Server (Host on a Local Port)

```bash
uv run fastmcp run main.py
```

This command:

* Starts the MCP server
* Hosts the tool on a local port
* Makes the tool accessible to MCP clients

---

## 📁 Project Structure (Example)

```
expense-tracker-mcp-server/
│
├── main.py              # MCP server entry point
├── README.md            # Project documentation
└── requirements.txt     # Dependencies (optional)
```

---

## 🛠 Common Commands Summary

| Purpose                        | Command                                         |
| ------------------------------ | ----------------------------------------------- |
| Initialize project             | `uv init`                                       |
| Install dependency             | `pip install fastmcp`                           |
| Install tool in Claude Desktop | `uv run fastmcp install claude-desktop main.py` |
| Run local inspector            | `uv run fastmcp dev inspector main.py`          |
| Run MCP server                 | `uv run fastmcp run main.py`                    |

---

## ❗ Troubleshooting

### Tool not visible in Claude Desktop

* Restart Claude Desktop after installation.
* Verify the install command completed successfully.

### Dependency issues

* Ensure Python version is compatible.
* Reinstall dependencies using `uv pip install fastmcp`.

### Port already in use

* Stop other running services or restart your system.

---

## 📜 License

Specify your project license here (MIT, Apache 2.0, etc.).

---

## 🤝 Contributing

Contributions, improvements, and suggestions are welcome.
Feel free to fork the repository and submit a pull request.

---
