YARA-RULE collection

# Custom Threat Detection & YARA Rules

a collection of custom YARA rules, Querries & detection logic. All rules/querries are actively developed based on 
real-world SOC incident response cases, threat hunting operations and malware reverse engineering.

## 📂 Structure
```
├── yara-rules/
│   ├── APT/            # Rules targeting specific Advanced Persistent Threats
│   ├── Ransomware/     # Rules for ransomware families and decryptors
│   ├── Tools/          # Rules detecting offensive tooling (Cobalt Strike etc.)
│   └── Phishing/       # Rules for malicious attachments and droppers
├── Querries/
│   ├── Splunk/         # SPL queries for detection
│   └── ELK/            # Elastic Security queries and KQL
|   └── Cortex XQL      # XQL queries for detection
└── README.md
```

🚀 Usage
To scan a directory or file with a specific rule using the YARA command-line tool:

Bash
```yara -w YARA_Rules/Ransomware/rule_name.yar /path/to/target/directory```


⚠️ Disclaimer
These rules are provided "as is" for defensive and research purposes only. 
I am not responsible for incorrect querries, blocked legitimate traffic or missed detections in your environment. 
Test before deployment.
