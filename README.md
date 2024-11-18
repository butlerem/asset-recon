# AssetRecon

A project for automating asset discovery and mapping external attack surfaces. Consolidates various reconnaissance techniques into a modular, extensible platform.

## Key Features (Planned)

- **Subdomain Enumeration**:
  - Discover public-facing and hidden subdomains using both passive and active methods.
- **Port Scanning**:
  - Identify open ports and services running on discovered assets.
- **Fingerprinting**:
  - Recognize technologies and frameworks (e.g., CMS, server types) on scanned endpoints.
- **Automation**:
  - Chain reconnaissance steps into a unified pipeline.
- **Exportable Reports**:
  - Output findings in structured formats (e.g., JSON, CSV) for integration into other tools.

## Goals

The project aims to:

1. Streamline the reconnaissance process for penetration testing and attack surface analysis.
2. Provide a modular architecture for extending features or customizing workflows.
3. Offer a middle ground between command-line tools and enterprise solutions.

## Repository Structure

The repository is structured as follows:

```plaintext
AssetRecon/
│
├── backend/              # Core backend functionality
│   ├── __init__.py       # Backend package initializer
│   ├── scan.py           # Main orchestration for scanning
│   ├── subdomain.py      # Subdomain enumeration logic
│   ├── port_scan.py      # Port scanning logic
│   └── tech_fingerprint.py # Technology fingerprinting logic
│
├── docs/                 # Documentation
│   ├── README.md         # Project overview
│   ├── CONTRIBUTING.md   # Contribution guidelines
│   └── API_DOCS.md       # Planned API documentation
│
├── frontend/            # Frontend-related files
│   ├── public/          # Static files (e.g., index.html)
│   ├── src/             # Source code (React or other framework)
│   └── package.json     # Frontend dependencies
│
├── tests/                # Unit and integration tests
│   ├── test_scan.py      # Tests for scan orchestration
│   ├── test_port_scan.py # Tests for port scanning
│   └── test_subdomain.py # Tests for subdomain enumeration
│
├── .gitignore            # Git ignore file
├── LICENSE               # Project license
├── requirements.txt      # Dependencies
└── setup.py              # Python package setup
```
