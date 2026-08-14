# 🤖 Autonomous BigQuery Data Agent

An autonomous Data Agent powered by **Gemini**, built using the **Google Agent Development Kit (ADK)**, and integrated with **BigQuery via the Model Context Protocol (MCP)**, deployed serverless on **Google Cloud Run**.

---

## 📌 Overview

This project demonstrates an agentic analytical workflow that replaces manual SQL query writing. Given a natural language business objective—such as optimizing the placement of commercial coffee trucks in New York City—the agent autonomously:

1. **Explores Schemas:** Inspects BigQuery dataset tables and column metadata.
2. **Executes Dynamic Queries:** Formulates and runs secure, read-only SQL queries over **58.9M+ records** in the NYC Citi Bike public dataset via MCP.
3. **Applies Multi-Factor Reasoning:** Filters by morning rush hour windows (6 AM – 10 AM), station departure/arrival flows, and dock capacities.
4. **Delivers Actionable Insights:** Recommends optimal physical locations backed by foot-traffic metrics.

---

## 🛠️ Architecture & Tech Stack

* **LLM Engine:** Gemini
* **Agent Framework:** Google Agent Development Kit (ADK)
* **Data Integration:** Model Context Protocol (MCP) Toolset (`execute_sql_readonly`, `list_tables`, `get_table_info`)
* **Data Warehouse:** Google Cloud BigQuery (`bigquery-public-data.new_york_citibike`)
* **Compute & Hosting:** Google Cloud Run

---

## 🚀 Getting Started

### Prerequisites
* Google Cloud Platform account with BigQuery & Cloud Run enabled
* Python 3.10+
* Google Cloud SDK (`gcloud`) installed and authenticated

### Local Setup
1. Clone the repository:
   ```bash
   git clone [https://github.com/](https://github.com/)<YOUR_USERNAME>/<REPO_NAME>.git
   cd <REPO_NAME>
