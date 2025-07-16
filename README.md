# 🚀 JMeter Performance Testing Project

This project uses **Apache JMeter** to simulate HTTP performance tests against a sample API (`https://jsonplaceholder.typicode.com`). It's designed to demonstrate basic load testing, assertions, and report generation.

---

## 📦 What's Included

- ✅ Basic HTTP GET request
- ✅ Response Assertion (expects HTTP 200)
- ✅ Constant Timer (500ms delay to simulate user think time)
- ✅ HTML report generation
- ✅ CLI run support for automation
- ✅ GitHub-compatible structure for cross-platform usage

---

## 🧰 Requirements

- Java 8+ (JDK 17 or later recommended)
- [Apache JMeter](https://jmeter.apache.org/download_jmeter.cgi)
- Git (to clone and push changes)

---

## 🛠 Setup Instructions

### 1. Clone this Repository

bash
git clone https://github.com/bmensh821/jmeter-http-test.git
cd jmeter-http-test


### 2. Open the Test Plan
Open `basic_http_test.jmx` in the JMeter GUI.


🧪 Run the Test in Headless Mode (CLI)
`jmeter -n -t basic_http_test.jmx -l results.jtl -e -o html_report`


🔍 What These Flags Do
| Flag    | Purpose                                |
| ------- | -------------------------------------- |
| `-n`    | Run in non-GUI (headless) mode         |
| `-t`    | Path to test plan `.jmx` file          |
| `-l`    | Log file for results `.jtl`            |
| `-e -o` | Generate HTML report in `html_report/` |



📊 View the Report
`html_report/index.html`

You'll see:

🟢 Response Times
🧵 Thread Counts
💥 Errors and Failures
📈 Request Throughput
🔁 Summary Stats


📁 Project Structure
```grapthql
jmeter-http-test/
│
├── basic_http_test.jmx        # JMeter test plan
├── results.jtl                # Raw test results (auto-generated)
├── html_report/               # HTML report folder (auto-generated)
├── README.md                  # Project documentation


🤝 Contributing
This project is a personal performance testing sandbox. Contributions, pull requests, or suggestions are welcome!

🧑‍💻 Author
Benyapak Mensh
GitHub: @bmensh821
