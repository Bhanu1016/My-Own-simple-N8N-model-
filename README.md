# n8n External Task Runner Setup

This project provides a **Docker-based environment for running n8n with external task runners**. It allows workflows to execute **JavaScript and Python code in isolated environments**, making automation workflows more scalable, secure, and flexible.

The setup uses Docker containers to run **n8n** along with dedicated **task runner services** that handle code execution separately from the main workflow engine.

---

## Features

* External task runners for secure code execution
* Support for **JavaScript and Python workflows**
* Preconfigured libraries for extended functionality
* Docker-based deployment for easy setup
* Scalable automation architecture
* Persistent data storage using Docker volumes

---

## Supported Libraries

### JavaScript

* crypto
* moment
* uuid

### Python

* numpy
* pandas

---

## Project Architecture

The system runs two main services:

1. **n8n Main Service**

   * Handles workflow automation
   * Communicates with task runners
   * Provides the workflow editor interface

2. **Task Runner Service**

   * Executes JavaScript and Python code
   * Runs in an isolated container environment
   * Uses controlled dependencies for security

---

## Project Structure

```
.
├── docker-compose.yml
├── Dockerfile
├── n8n-task-runners.json
```

**docker-compose.yml**
Defines and connects the n8n service with the task runner container.

**Dockerfile**
Builds the task runner environment.

**n8n-task-runners.json**
Configures available runners and allowed libraries.

---

## Installation

### 1. Clone the Repository

```
git clone https://github.com/yourusername/your-repository-name.git
cd your-repository-name
```

### 2. Start the Services

```
docker compose up -d
```

### 3. Open n8n in Browser

```
http://localhost:5678
```

---

## Example Use Cases

* AI workflow automation
* Data processing pipelines
* API integrations
* Python-based data analysis inside workflows
* Custom automation logic using JavaScript or Python

---

## Future Improvements

* AI workflow templates
* Distributed task runners
* Monitoring and logging tools
* Integration with AI services and APIs

---

## License

This project is licensed under the MIT License.

---

If you want, I can also give you **3 things that make a GitHub repo look professional instantly**:

* a **GitHub banner**
* an **architecture diagram**
* **example workflow files**

Those three things make your repo look **10× more serious** than a normal student project.
