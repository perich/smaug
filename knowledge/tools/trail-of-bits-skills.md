# Trail of Bits Security Skills

**Repository:** https://github.com/trailofbits/skills
**Stars:** 2,401
**Language:** Python

## Overview
Trail of Bits Security Skills is a Claude Code plugin marketplace providing skills to enhance AI-assisted security analysis, testing, and development workflows. It offers a comprehensive suite of security tools integrated as Claude Code plugins.

## Installation
```
/plugin marketplace add trailofbits/skills
```

## Available Plugin Categories

### Smart Contract Security
- **building-secure-contracts**: Smart contract security toolkit with vulnerability scanners for 6 blockchains
- **entry-point-analyzer**: Identify state-changing entry points in smart contracts for security auditing

### Code Auditing
- **audit-context-building**: Build deep architectural context through ultra-granular code analysis
- **burpsuite-project-parser**: Search and extract data from Burp Suite project files
- **differential-review**: Security-focused differential review of code changes with git history analysis
- **insecure-defaults**: Detect insecure default configurations, hardcoded credentials, and fail-open security patterns
- **semgrep-rule-creator**: Create and refine Semgrep rules for custom vulnerability detection
- **semgrep-rule-variant-creator**: Port existing Semgrep rules to new target languages with test-driven validation
- **sharp-edges**: Identify error-prone APIs, dangerous configurations, and footgun designs
- **static-analysis**: Static analysis toolkit with CodeQL, Semgrep, and SARIF parsing
- **testing-handbook-skills**: Skills from the Testing Handbook: fuzzers, static analysis, sanitizers, coverage
- **variant-analysis**: Find similar vulnerabilities across codebases using pattern-based analysis

### Malware Analysis
- **yara-authoring**: YARA detection rule authoring with linting, atom analysis, and best practices

### Verification
- **constant-time-analysis**: Detect compiler-induced timing side-channels in cryptographic code
- **property-based-testing**: Property-based testing guidance for multiple languages and smart contracts
- **spec-to-code-compliance**: Specification-to-code compliance checker for blockchain audits

### Audit Lifecycle
- **fix-review**: Verify fix commits address audit findings without introducing bugs

### Reverse Engineering
- **dwarf-expert**: Interact with and understand the DWARF debugging format

### Mobile Security
- **firebase-apk-scanner**: Scan Android APKs for Firebase security misconfigurations

### Development Tools
- **ask-questions-if-underspecified**: Clarify requirements before implementing
- **modern-python**: Modern Python tooling and best practices with uv, ruff, and pytest

## Use Cases
- Real, top-tier security audits
- Smart contract vulnerability scanning
- Code security analysis and pattern detection
- Malware detection and reverse engineering
- Compliance verification for blockchain applications
- Testing and verification workflows
