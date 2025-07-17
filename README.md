# Cybershield Technologies - Mock Cybersecurity Company (Student Project)

company_info = {
    "name": "Cybershield Technologies",
    "industry": "Cybersecurity",
    "founded": 2018,
    "location": "Austin, Texas, USA",
    "size": "About 100 employees",
    "website": "www.cybershieldtech.io (mock site)",
    "clients": ["Small Businesses", "Hospitals", "Banks"],
    "mission": "We help companies stay safe online by giving them simple, smart cybersecurity solutions that actually work."
}

services = {
    "Managed Security (MSSP)": [
        "24/7 monitoring",
        "Responding to attacks",
        "Our own Security Operations Center (SOC)"
    ],
    "Pen Testing (Ethical Hacking)": [
        "Checking if hackers can break in",
        "Testing websites and apps",
        "Social engineering (like phishing tests)"
    ],
    "Risk & Compliance Help": [
        "Making sure businesses follow rules (HIPAA, GDPR)",
        "Finding weak spots in their security"
    ],
    "Training People": [
        "Teaching employees how to avoid cyber scams",
        "Running fake phishing emails to test awareness"
    ],
    "Endpoint Protection": [
        "Making sure computers and devices are secure"
    ],
    "Cloud Security": [
        "Helping protect companies using AWS, Azure, or Google Cloud"
    ]
}

tech_stack = {
    "SIEM (Log Monitoring)": ["Splunk", "IBM QRadar"],
    "EDR (Device Security)": ["CrowdStrike", "SentinelOne"],
    "Cloud Security": ["Prisma Cloud", "Azure Security Center"],
    "Vulnerability Scanning": ["Nessus", "Qualys"],
    "Pen Testing Tools": ["Burp Suite", "Metasploit"]
}

team_members = [
    {"role": "CEO", "name": "Jessica Tran"},
    {"role": "CISO (Security Boss)", "name": "David Kim"},
    {"role": "SOC Manager", "name": "Priya Patel"},
    {"role": "Lead Hacker (Pen Tester)", "name": "Marcus Jones"},
    {"role": "Compliance Expert", "name": "Sarah Thompson"}
]

use_cases = [
    "Stopped a fake ransomware attack on a pretend fintech startup.",
    "Helped a fake hospital pass a HIPAA security check.",
    "Found and shut down an insider threat in a made-up company."
]

# Display Function
def display_company_profile():
    print("\n=== 🧑‍💻 Cybershield Technologies – Student Project ===")
    for key, value in company_info.items():
        if isinstance(value, list):
            print(f"{key.title()}: {', '.join(value)}")
        else:
            print(f"{key.title()}: {value}")

    print("\n=== 🛡️ Services Offered ===")
    for category, items in services.items():
        print(f"\n{category}:")
        for item in items:
            print(f"  - {item}")

    print("\n=== 🧰 Tech Stack / Tools Used ===")
    for area, tools in tech_stack.items():
        print(f"{area}: {', '.join(tools)}")

    print("\n=== 👥 Team Members ===")
    for member in team_members:
        print(f"{member['role']}: {member['name']}")

    print("\n=== 📝 Example Use Cases ===")
    for case in use_cases:
        print(f"- {case}")

# Run the display
if __name__ == "__main__":
    display_company_profile()

