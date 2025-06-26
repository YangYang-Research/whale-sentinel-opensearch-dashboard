# 🐋 Whale Sentinel OpenSearch Dashboard

This guide helps you set up the **Whale Sentinel** OpenSearch Dashboard for visualizing logs and monitoring system activity.

---

## ⚙️ Setup OpenSearch Stack

### 1. Prepare Docker Compose File

- Copy the example configuration to an active file:

```bash
  cp docker-compose.example.yml docker-compose.yml
```

- Open docker-compose.yml and update the environment variable: `OPENSEARCH_INITIAL_ADMIN_PASSWORD: your-strong-password`
Replace your-strong-password with a secure password of your choice.

### 2. Start OpenSearch Stack

Run the following command to start OpenSearch and its dashboard:

```bash
docker-compose up -d
```

This will launch all services in the background.


---

## 📊 Configure OpenSearch Dashboard

### 1. Create Index Pattern

- Navigate to:  
  **Sidebar → Dashboards Management → Index Patterns**
- Click **Create index pattern**
- Set the index name as: `whale-sentinel-*-logs`
- Complete the steps to save the index pattern.

---

### 2. Import Dashboards & Visualizations

- Navigate to:  
**Sidebar → Dashboards Management → Saved Objects**
- Click **Import**
- Upload the file: `templates/dashboard&visualization.ndjson`
- Confirm and overwrite if prompted.

---

## ✅ Result

You will now be able to access the prebuilt dashboards and visualizations tailored for Whale Sentinel log data.

---

## 🛠 Requirements

- OpenSearch Dashboard access
- `.ndjson` file provided in the repository

---

## 📁 Included File

- `templates/*` — contains all necessary dashboards and visualizations.

---

## 🤝 Contributing

We welcome contributions and feedback. Please fork the repository and open a pull request with your suggested changes.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🛡️ Security & Reporting

If you discover a vulnerability, please report it responsibly via GitHub Issues or contact the maintainers privately.




