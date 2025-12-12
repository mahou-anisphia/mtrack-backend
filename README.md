_From the discovery & learning series "Magicodelogy"_

> **Note:** This project is **archived**. It is the backend component of the **first product I ever built at Viettel**, representing my first deep dive into Python and TCP socket programming.

## 📖 About
This is the backend server for the **Clairvoyance MTrack** platform. It acts as the bridge between physical MTrack hardware and the user dashboard.

Key features include:
* **TCP Server:** Listens on port `23304` for raw data packets from NB-IoT devices.
* **Data Processing:** Parses incoming hex/binary data from the trackers.
* **API:** Provides endpoints (via Flask) for the [Frontend](https://github.com/mahou-anisphia/clairvoyance-mtrack-fe) to retrieve device status and history.

## 🛠️ Tech Stack
* **Language:** Python 3
* **Framework:** Flask
* **Database:** PostgreSQL (via PL/pgSQL)
* **Protocols:** TCP, HTTP

## 🚀 Setup & Installation

### 1. Set up Virtual Environment
```bash
python3 -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
````

### 2\. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3\. Database Setup

Ensure you have a PostgreSQL instance running and apply the schema:

  * Run the scripts in `schema.sql`.

### 4\. Run the Server

```bash
python3 main.py
```

## 🔗 Related Repositories

  * **Frontend:** [clairvoyance-mtrack-fe](https://github.com/mahou-anisphia/clairvoyance-mtrack-fe)

## 📄 License

This project is open for educational and archival purposes.
