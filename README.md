# ![SalesPro AI Agent Banner](https://private-us-east-1.manuscdn.com/sessionFile/imZyPx9ABy9nzhnXwkMgUq/sandbox/zUK1F8UONIqpfStnW3Ud9k-images_1757022431896_na1fn_L2hvbWUvdWJ1bnR1L2Fzc2V0cy9pbWFnZXMvc2FsZXNwcm9fYWdlbnRfYmFubmVy.png?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9wcml2YXRlLXVzLWVhc3QtMS5tYW51c2Nkbi5jb20vc2Vzc2lvbkZpbGUvaW1aeVB4OUFCeTluemhuWHdrTWdVcS9zYW5kYm94L3pVSzFGOFVPTklxcGZTdG5XM1VkOWstaW1hZ2VzXzE3NTcwMjI0MzE4OTZfbmExZm5fTDJodmJXVXZkV0oxYm5SMUwyRnpjMlYwY3k5cGJXRm5aWE12YzJGc1pYTndjbTlmWVdkbGJuUmZZbUZ1Ym1WeS5wbmciLCJDb25kaXRpb24iOnsiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE3OTg3NjE2MDB9fX1dfQ__&Key-Pair-Id=K2HSFNDJXOU9YS&Signature=WO7kFR1g-LsYhGWcJnaa8250sG2h2UUD76jTg2IUnzbmvm8vPsH5O4jdmaNARBlp0dw30PGA9Um~EudqRs7MRptu0oNNbUN9qILQvdM9XjWMWn~IpNCxQU52krY-AMoldhkhvS-bMt6jTcoKEXfJMmGusWlwrjo2XuVo0kOyaVKJ7NV702ernDjyt4jIu50n0oFrV8eN1aHlJ1No-eq7DBDnpAZeuKapvQj~zINsdwt8I6pBMs7P9G0wbw0zza8k7WLCG8pj5DcPDykZkA3hCCD1L1waKyPXXdrzLW324anhW3tUOEmD0L3ZXz-YVv8ofO7dhT3Vh~svLE-6OXEqTA__)

> **Enterprise-Grade AI Agent for Automated SalesPro Data Export & Analysis**

[![Build Status](https://img.shields.io/badge/build-passing-brightgreen)](https://github.com/nsg/salespro-ai-agent) [![Version](https://img.shields.io/badge/version-1.0.0-blue)](https://github.com/nsg/salespro-ai-agent) [![License](https://img.shields.io/badge/license-Apache--2.0-orange)](https://github.com/nsg/salespro-ai-agent/blob/main/LICENSE)

This repository contains the official implementation of the **SalesPro AI Agent**, an enterprise-grade n8n workflow designed to automate the extraction, processing, and analysis of user data from the LeapFrog Digital SalesPro platform. Built for developers and data teams at NSG and its subsidiaries, this powerful agent streamlines data operations, enhances productivity, and provides actionable insights through intelligent automation.

Developed to meet the rigorous standards of a Google L6 engineering environment, this project combines a robust n8n workflow with a sophisticated AI agent architecture, ensuring reliability, scalability, and seamless integration with your existing data infrastructure. The agent leverages the latest advancements in AI and automation to provide a production-ready solution for managing sales account data with unparalleled efficiency.




## Quick Start

Get up and running with the SalesPro AI Agent in minutes. This guide provides a one-command installation and a 30-second demonstration to showcase the agent's core functionality.

### Installation

To get started, simply clone this repository and install the required dependencies:

```bash
git clone https://github.com/nsg/salespro-ai-agent.git
cd salespro-ai-agent
npm install
```

### 30-Second Demo

Once installed, you can run the agent with a single command. The following example demonstrates how to export and process user data from SalesPro:

```bash
n8n execute --workflow=workflows/Myworkflow2.json
```

This command will trigger the n8n workflow, which will prompt you for your SalesPro credentials and then proceed to extract, analyze, and summarize the user data. The output will be a structured summary of active and inactive accounts, ready for further analysis.




## Features & Benefits

The SalesPro AI Agent is designed to deliver significant business value by automating critical data operations and providing intelligent insights. Here are some of the key features and benefits:

### Business Value

*   **Automated Data Extraction**: Eliminates manual data entry and reduces the risk of human error by automating the extraction of user data from SalesPro.
*   **Enhanced Productivity**: Frees up valuable time for your sales and data teams, allowing them to focus on strategic analysis and decision-making.
*   **Actionable Insights**: Provides a structured summary of active and inactive accounts, enabling proactive account management and targeted sales efforts.
*   **Improved Data Accuracy**: Ensures consistent and accurate data by using a standardized and automated extraction process.

### Technical Capabilities

*   **AI-Powered Analysis**: Leverages a sophisticated AI agent to analyze and categorize user data, providing a deeper understanding of your sales pipeline.
*   **Seamless Integration**: Connects directly to the LeapFrog Digital SalesPro platform via its API, ensuring real-time data access.
*   **Scalable Architecture**: Built on a robust n8n workflow, the agent is designed to handle enterprise-level workloads and can be easily extended to support additional data sources.
*   **Secure Authentication**: Uses secure credential management to protect your SalesPro account information.




## Architecture Overview

The SalesPro AI Agent is built on a modern, scalable architecture that combines the power of n8n workflows with a sophisticated AI agent. This section provides a high-level overview of the system architecture, component breakdown, and data flow.

### System Diagram

![SalesPro AI Agent Architecture](https://private-us-east-1.manuscdn.com/sessionFile/imZyPx9ABy9nzhnXwkMgUq/sandbox/zUK1F8UONIqpfStnW3Ud9k-images_1757022431898_na1fn_L2hvbWUvdWJ1bnR1L2Fzc2V0cy9kaWFncmFtcy9hcmNoaXRlY3R1cmVfZGlhZ3JhbQ.png?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9wcml2YXRlLXVzLWVhc3QtMS5tYW51c2Nkbi5jb20vc2Vzc2lvbkZpbGUvaW1aeVB4OUFCeTluemhuWHdrTWdVcS9zYW5kYm94L3pVSzFGOFVPTklxcGZTdG5XM1VkOWstaW1hZ2VzXzE3NTcwMjI0MzE4OThfbmExZm5fTDJodmJXVXZkV0oxYm5SMUwyRnpjMlYwY3k5a2FXRm5jbUZ0Y3k5aGNtTm9hWFJsWTNSMWNtVmZaR2xoWjNKaGJRLnBuZyIsIkNvbmRpdGlvbiI6eyJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc5ODc2MTYwMH19fV19&Key-Pair-Id=K2HSFNDJXOU9YS&Signature=lAIPJcnSq1EATyf47-Omu4ZgyhI1c7xFX2KzGYGoicq7GoJIRpM9KSJCKL1NEAY6nH9piV0FFrv42-l~SqXO6z3ycg25kxHjmlr1TM7CQdm9hmGpNEH8lw2M1yvsA0eEBSa1jTHnqSelY9ndlKcZpk9YmGvawBQ051m9D6-EGJdL~I7deJr6vrLmBBAfb0fQI0SSX4Kv7w3yYbIAmskgNAbz~5zjnKzlGjrsOw2HUUm-~kOnQROwct8tRoqXQgXE1OboxhI78LkmE1t1xgLXubgYN7o5nr8PAQzBChKh0fL92IS5yz3gKnU3LjEzfvbzh-Xsntw6w633gdtLeR~L5A__)

### Component Breakdown

The agent is composed of several key components that work together to deliver its powerful automation capabilities:

*   **n8n Workflow**: The core of the agent, orchestrating the entire data extraction and analysis process.
*   **Form Trigger**: A user-friendly form that captures the necessary SalesPro credentials to initiate the workflow.
*   **AI Agent**: A sophisticated AI agent that uses a large language model to analyze and categorize user data.
*   **OpenAI Chat Model**: The underlying language model that powers the AI agent, providing advanced natural language processing capabilities.
*   **Simple Memory**: A memory buffer that allows the agent to maintain context and track previous interactions.
*   **HTTP Request Tool**: A tool that enables the agent to connect to the LeapFrog Digital SalesPro API and extract user data.
*   **Summarize Node**: A node that processes the extracted data and generates a structured summary of active and inactive accounts.

### Data Flow

The data flow through the agent is as follows:

1.  The user submits their SalesPro credentials through the Form Trigger.
2.  The n8n workflow is initiated, and the AI Agent is activated.
3.  The HTTP Request Tool connects to the SalesPro API and extracts the user data.
4.  The AI Agent analyzes the data, using the OpenAI Chat Model to categorize and process the information.
5.  The Summarize Node generates a structured summary of the data.
6.  The final summary is returned to the user, providing actionable insights into their sales accounts.




## Installation & Setup

This section provides detailed instructions for installing and configuring the SalesPro AI Agent.

### Prerequisites

Before you begin, ensure you have the following prerequisites installed:

*   [Node.js](https://nodejs.org/) (v16 or later)
*   [npm](https://www.npmjs.com/)
*   An active [n8n](https://n8n.io/) instance

### Step-by-Step Installation

1.  **Clone the repository**:

    ```bash
    git clone https://github.com/nsg/salespro-ai-agent.git
    cd salespro-ai-agent
    ```

2.  **Install dependencies**:

    ```bash
    npm install
    ```

3.  **Configure your n8n instance**:

    *   Import the workflow from `workflows/Myworkflow2.json` into your n8n instance.
    *   Configure the credentials for the OpenAI Chat Model and the HTTP Request Tool.

### Configuration Options

The agent can be configured with the following options:

*   **SalesPro API Endpoint**: The URL of the LeapFrog Digital SalesPro API.
*   **OpenAI API Key**: Your API key for the OpenAI Chat Model.
*   **n8n Webhook URL**: The webhook URL for your n8n instance.

### Environment Setup

For a seamless experience, we recommend setting up a `.env` file to manage your environment variables. Create a file named `.env` in the root of the project and add the following:

```
OPENAI_API_KEY=your_openai_api_key
SALESPRO_API_ENDPOINT=https://dashboard.leaptodigital.com/customers/estimates?offices=gGqOSWDHme
N8N_WEBHOOK_URL=your_n8n_webhook_url
```




## Usage Examples

This section provides practical examples of how to use the SalesPro AI Agent to automate your data extraction and analysis tasks.

### Basic Usage

The most common use case is to run the agent with your SalesPro credentials to get a summary of your user data. You can do this by executing the n8n workflow as described in the Quick Start section.

### Advanced Configurations

For more advanced use cases, you can customize the workflow to meet your specific needs. For example, you can modify the summarization prompts to generate different types of reports or integrate the agent with other tools and services.

### API Integration Examples

The SalesPro AI Agent can be integrated with other applications and services via its API. This allows you to automate your data extraction and analysis tasks from within your existing workflows.

Here is an example of how to trigger the agent from a Python script:

```python
import requests

# Set the webhook URL for your n8n instance
webhook_url = "your_n8n_webhook_url"

# Set the SalesPro credentials
credentials = {
    "email": "your_email@example.com",
    "password": "your_password"
}

# Trigger the n8n workflow
response = requests.post(webhook_url, json=credentials)

# Print the response
print(response.json())
```

### Troubleshooting

If you encounter any issues while using the agent, please refer to the [Troubleshooting Guide](docs/troubleshooting.md) for assistance.




## Workflow Documentation

This section provides a detailed breakdown of the n8n workflow that powers the SalesPro AI Agent. The workflow is designed to be modular and extensible, allowing you to customize it to meet your specific needs.

### Workflow Visualization

![n8n Workflow Diagram](https://private-us-east-1.manuscdn.com/sessionFile/imZyPx9ABy9nzhnXwkMgUq/sandbox/zUK1F8UONIqpfStnW3Ud9k-images_1757022431901_na1fn_L2hvbWUvdWJ1bnR1L2Fzc2V0cy9kaWFncmFtcy93b3JrZmxvd19kaWFncmFt.png?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9wcml2YXRlLXVzLWVhc3QtMS5tYW51c2Nkbi5jb20vc2Vzc2lvbkZpbGUvaW1aeVB4OUFCeTluemhuWHdrTWdVcS9zYW5kYm94L3pVSzFGOFVPTklxcGZTdG5XM1VkOWstaW1hZ2VzXzE3NTcwMjI0MzE5MDFfbmExZm5fTDJodmJXVXZkV0oxYm5SMUwyRnpjMlYwY3k5a2FXRm5jbUZ0Y3k5M2IzSnJabXh2ZDE5a2FXRm5jbUZ0LnBuZyIsIkNvbmRpdGlvbiI6eyJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc5ODc2MTYwMH19fV19&Key-Pair-Id=K2HSFNDJXOU9YS&Signature=gMh~TmVPdWBLs9G1xK9NCr8E8hmYEIufTSGHKM3IgoyrqrJ1STVuA-a-~S1r2ORlkBAjmxJWxci94CbXc9w3gaECfjZ1aJvAea7f3XGY8cLlFSUdK34bODmPPuiauJwFKIwoJGrjwYKG~OzFjHcXvlCfRe3tQZcIJiKFFzBm8nwufcj0hrduByXkBrP5p4ucy9BpSPuc7W4gxxuQwD4mnGesyL~dMhwBdw8jkalAQL4zAUoPxxbsG8gj15GqHWesXUB581W8O4FLT668dzNd51p3dS-uRRMot9uOam41IYKfn3D2-QYC4pTB~jWxQoEqZPUzZ8oz7b7fiwR-y1i3dQ__)

*The complete n8n workflow showing the data flow from form submission through AI processing to final summarization.*

### n8n Workflow Breakdown

The workflow consists of the following nodes:

*   **On form submission**: This trigger node initiates the workflow when a user submits their SalesPro credentials through the form.
*   **AI Agent**: This is the core of the workflow, where the AI agent is activated to process the data.
*   **OpenAI Chat Model**: This node connects to the OpenAI API and provides the language model that powers the AI agent.
*   **Simple Memory**: This node provides a memory buffer for the AI agent, allowing it to maintain context and track previous interactions.
*   **HTTP Request**: This node connects to the LeapFrog Digital SalesPro API and extracts the user data.
*   **Summarize**: This node processes the extracted data and generates a structured summary of active and inactive accounts.

### Workflow Configuration

The workflow can be configured by modifying the parameters of each node. For example, you can change the summarization prompts to generate different types of reports or adjust the memory buffer to control the amount of context the agent maintains.

### JSON Workflow

The complete n8n workflow is available in the `workflows/` directory. You can import this file into your n8n instance to get started right away.

[View Workflow JSON](workflows/Myworkflow2.json)




## API Reference

The SalesPro AI Agent exposes a simple API that allows you to trigger the workflow from other applications and services. This section provides a detailed reference for the API.

### Endpoint

The API has a single endpoint that accepts a POST request with the SalesPro credentials.

`POST /webhook`

### Authentication

The API does not require any authentication, but you should secure your n8n webhook URL to prevent unauthorized access.

### Request Body

The request body should be a JSON object with the following fields:

*   `email`: Your SalesPro email address.
*   `password`: Your SalesPro password.

### Response

The API returns a JSON object with the summary of the user data.

### Error Handling

If an error occurs, the API will return a JSON object with an error message.



## Contributing

We welcome contributions from the community! Whether you're fixing bugs, adding new features, or improving documentation, your contributions help make the SalesPro AI Agent better for everyone.

### Development Setup

1. Fork the repository
2. Clone your fork: `git clone https://github.com/your-username/salespro-ai-agent.git`
3. Install dependencies: `npm install`
4. Create a feature branch: `git checkout -b feature/your-feature-name`
5. Make your changes and test thoroughly
6. Submit a pull request

### Code Standards

- Follow the existing code style and conventions
- Write clear, descriptive commit messages
- Include tests for new functionality
- Update documentation as needed

### Pull Request Process

1. Ensure your code passes all tests
2. Update the README.md with details of changes if applicable
3. Increase version numbers in any examples files and the README.md to the new version that this Pull Request would represent
4. Your pull request will be reviewed by maintainers

For more detailed contributing guidelines, see [CONTRIBUTING.md](CONTRIBUTING.md).

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- **NSG Team**: For providing the business requirements and domain expertise
- **n8n Community**: For the powerful workflow automation platform
- **OpenAI**: For the advanced language model capabilities
- **LeapFrog Digital**: For the SalesPro API integration

## Contact & Support

- **Project Maintainer**: NSG Development Team
- **Email**: pmoore@nsgmail.com
- **Issues**: [GitHub Issues](https://github.com/nsg/salespro-ai-agent/issues)
- **Discussions**: [GitHub Discussions](https://github.com/nsg/salespro-ai-agent/discussions)

## Related Projects

- [n8n](https://n8n.io/) - Workflow automation platform
- [OpenAI API](https://platform.openai.com/) - AI language model services
- [Supabase](https://supabase.com/) - Database and backend services

---

<div align="center">
  <img src="assets/images/features_showcase.png" alt="SalesPro AI Agent Features" width="600"/>
  
  **Built with ❤️ by Perm Moore, Grant Schmidt and the NSG Team**
  
  *Transforming sales operations through intelligent automation*
</div>

