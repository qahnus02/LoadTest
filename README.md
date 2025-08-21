# K6 Load Testing Suite

This repository contains different types of load testing scripts built using [k6](https://k6.io).  
Each script is designed to simulate a specific kind of load on your system and measure performance under different conditions.  

---

## 📂 Test Types

- **Smoke Test (`smoke.js`)**  
  Ensures the system is working under minimal load. Quick and light test to validate the setup.

- **Load Test (`load.js`)**  
  Simulates expected production traffic to measure system performance.

- **Stress Test (`stress.js`)**  
  Pushes the system beyond normal load to find its breaking point and bottlenecks.

- **Spike Test (`spike.js`)**  
  Applies sudden large traffic spikes to check system stability and recovery.

- **Soak Test (`soak.js`)**  
  Runs for an extended period of time to check memory leaks, resource usage, and long-term stability.

- **Breakpoint Test (`breakpoint.js`)**  
  Gradually increases load until the system fails, helping determine maximum capacity.

---

## ⚙️ Prerequisites

- Install [k6](https://k6.io/docs/getting-started/installation/)  

```bash
# Ubuntu/Debian
sudo apt update
sudo apt install k6 -y
```

## 🚀 How to run tests

```bash
k6 run smoke.js
k6 run load.js
k6 run stress.js
k6 run spike.js
k6 run soak.js
k6 run breakpoint.js
```

## 📊 Sample Output

- k6 generates metrics like:

- HTTP requests per second (RPS)

- Response times (p95, p99)

- Error rate

- Throughput

- Resource usage


## 🛠️ Project Structure

```lua
.
├── smoke.js
├── load.js
├── stress.js
├── spike.js
├── soak.js
├── breakpoint.js
└── README.md
```

## 🙌 Contribution

Feel free to fork, suggest improvements, or add new test scenarios!


# macOS
brew install k6
