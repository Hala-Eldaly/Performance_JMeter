# 🧪 JMeter Performance Testing Project: UI & API Workload Simulation

## 📌 Project Overview
This project demonstrates comprehensive performance testing using **Apache JMeter**, covering:

- End-to-end UI workflows (PetStore e-commerce)
- REST API flows (Restful Booker service)
- Real-world load simulations with SLA validation

---

## 🛠️ Key Components

### 1️⃣ Test Plan Design

#### A. UI Scenario – PetStore Workflow
- Homepage navigation → User registration → Product browsing  
- Cart operations → Checkout process → Order confirmation validation  

**Techniques Used:**
- CSV data parameterization (`Test_Data.csv`)
- Response assertions (content validation)
- Realistic pacing (timers for think time)

#### B. API Scenario – Restful Booker Flow
- Authentication → Booking CRUD operations (Create/Read/Update/Delete)

**Techniques Used:**
- Environment-agnostic requests (HTTP Request Defaults)
- Session consistency (Cookie & Cache managers)
- JSON extraction for dynamic data handling

---

### 2️⃣ Execution & Analysis

- **Test Configuration:**
  - 2 concurrent users
  - 10-minute duration
  - Monitoring via Aggregate Report + SLA benchmarks

- **SLA Validation:**
  - ✅ Error rate ≤ 10%
  - ✅ 90% of responses ≤ 3 seconds
  - ✅ 99% of responses ≤ 5 seconds

- **Deliverables:**
  - Screenshots of test results
  - Formal report with metrics analysis (`Aggregate Report_HalaEldaly.docx`)

---

### 3️⃣ Advanced Load Simulation

- **Stepping Thread Group Plugin:**
  - Gradual ramp-up: +100 users (1/sec)
  - Controlled ramp-down: -100 users (1/sec)

**Purpose:** Identify performance thresholds and system stability under progressive load.

---

## 📂 Project Structure

| Path                                         | Description                            |
|----------------------------------------------|----------------------------------------|
| `jmeter/Performance_Testing_Jmeter_Project.jmx` | JMeter test plan                        |
| `jmeter/Test_Data.csv`                        | Parameterization input data             |
| `jmeter/Aggregate Report_HalaEldaly.docx`     | Results with SLA analysis               |
| `Attachments/`                                | Visual evidence (graphs/screenshots)    |

---

## 🧰 Tools & Techniques

- **Core JMeter:** Thread Groups, Timers, Assertions
- **Data Management:** CSV Config, JSON Extractor
- **Plugins:** Stepping Thread Group for load profiling
- **Analysis:** Aggregate Report, Response Time vs. Load correlation

---

## 🚀 How to Run

1. Open `Performance_Testing_Jmeter_Project.jmx` in Apache JMeter.
2. Place `Test_Data.csv` in the same directory.
3. Execute the test (UI/API/load profile as needed).
4. Analyze results via **Aggregate Report** or switch to **Stepping Thread Group** for load testing.

---

## 🔍 Why This Matters

- Validates real-user behavior under controlled load.
- Ensures API reliability through CRUD operation testing.
- Provides actionable insights via SLA-driven metrics.
