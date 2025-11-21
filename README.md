# GitHub Crypto Repositories Commits


A professional and modular tool designed to verify and analyze commit activity across a curated list of cryptocurrency-related GitHub repositories. This project aims to help researchers, developers, and ecosystem analysts track development activity as an indicator of project health and transparency.


## 🔍 Overview
Development activity is a critical metric in understanding the long‑term sustainability of open‑source blockchain projects. This tool retrieves commit counts from selected repositories and provides structured output for analysis or automation workflows.


## ✨ Features
- Fetches commit data from a curated list of crypto-related open-source repos
- Lightweight and easy to integrate into analytics pipelines
- Outputs results in JSON format
- Supports GitHub API tokens for extended rate limits
- Clean and extensible code structure


## 📁 Repository Structure
```
crypto-commit-repo/
├── fetch_commits.py # Main script for collecting commit data
├── requirements.txt # Python dependencies
├── README.md # Project documentation
└── LICENSE # MIT license
```


## 🚀 Installation
Clone the repository:
```bash
git clone https://github.com/username/crypto-commit-repo.git
cd crypto-commit-repo
```
Install dependencies:
```bash
pip install -r requirements.txt
```


## ▶️ Usage
Run the commit scanner:
```bash
python fetch_commits.py
```
Optional (recommended): Set a GitHub API token to avoid rate limits
```bash
export GITHUB_TOKEN=your_token_here
```


## ⚙️ Configuration
Edit the `REPOS` array inside `fetch_commits.py` to customize which repositories are scanned:
```python
REPOS = [
"bitcoin/bitcoin",
"ethereum/go-ethereum",
"solana-labs/solana"
]
```


## 📜 Output Example
```json
{
"bitcoin/bitcoin": 30,
"ethereum/go-ethereum": 45,
"solana-labs/solana": 52
}
```


## 🧩 Roadmap
- Add async request support
- Add trend analysis and commit history graphs
- Export results to CSV
- Add repository metadata insights (stars, forks, contributors)


## 🤝 Contributing
Contributions are welcome! Feel free to open issues or submit pull requests.
