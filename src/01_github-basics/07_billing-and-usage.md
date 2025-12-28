# GitHub Billing and Usage

**Session**: 03 - Introduction to GitHub Products, Plans & Billing  
**Domain**: GitHub Fundamentals (20%)  
**Duration**: ~10 minutes

---

## How GitHub Billing Works

### Billing Owner

* **Organization Level**: Billing is managed at the organization level
* **Billing Owner**: Person responsible for payment
* **Centralized**: One billing account per organization
* **Not Per Repository**: Billing is not tied to individual repositories

### Billing Structure

```
Organization
├── Subscription (plan cost)
│   ├── Team plan: $X/user/month
│   └── Enterprise plan: Custom pricing
│
└── Usage-Based (metered)
    ├── Actions minutes
    ├── Storage
    └── Advanced security features
```

---

## Subscription vs Usage-Based Billing

### Subscription Features

* Fixed monthly/annual cost
* Included in plan
* Examples:
  * Private repositories
  * Team collaboration tools
  * Basic Actions minutes (included)
  * Basic storage (included)

### Usage-Based Billing

* Charged based on consumption
* Additional cost beyond subscription
* Examples:
  * GitHub Actions minutes (beyond included)
  * Storage (beyond included)
  * Advanced security scanning
  * GitHub Packages storage

---

## License Usage Stats

### What is License Usage?

* Tracks consumption of paid seats/licenses
* Shows who is using licenses
* Helps with cost optimization
* Visibility for administrators

### Why It Matters

* **Cost Control**: Identify unused licenses
* **Compliance**: Ensure proper license allocation
* **Forecasting**: Plan for future needs
* **Optimization**: Right-size license count

### Viewing License Usage

* Organization settings → Billing
* See active users
* See license consumption
* Export usage reports

---

## Non-Human License Usage

### Machines and Peripherals

* **Bots**: Automated accounts can consume licenses
* **CI/CD Systems**: Build servers may need licenses
* **Integrations**: Third-party tools may require licenses
* **Service Accounts**: Automated service accounts

### Understanding Usage

* Not always "one developer = one license"
* Machines and tools can consume entitlements
* Important for accurate license planning
* Affects billing calculations

---

## Metered Usage Reports

### What is Metered Usage?

* Features charged based on consumption
* Tracked separately from subscription
* Reported in usage dashboards
* Helps with cost forecasting

### Examples of Metered Features

#### GitHub Actions Minutes

* Compute time for workflows
* Charged per minute used
* Different rates for different runners
* Free tier includes limited minutes

#### Storage

* Repository storage
* GitHub Packages storage
* Charged per GB used
* Free tier includes limited storage

#### Advanced Security

* Code scanning
* Secret scanning
* Dependency review
* Charged per repository or per scan

---

## Usage Reporting

### What Reports Show

* **License Usage**: Who is using licenses
* **Actions Minutes**: Compute consumption
* **Storage**: Storage usage across repos
* **Security Scans**: Number of scans performed

### Benefits

* **Cost Visibility**: Understand spending
* **Forecasting**: Plan for future costs
* **Optimization**: Identify cost-saving opportunities
* **Compliance**: Track usage for reporting

---

## Billing Best Practices

### Monitor Usage Regularly

* Review usage reports monthly
* Identify trends and spikes
* Plan for seasonal variations
* Optimize based on data

### Right-Size Licenses

* Remove inactive users
* Consolidate service accounts
* Review license allocation quarterly
* Adjust based on actual usage

### Optimize Metered Usage

* Monitor Actions minutes
* Clean up unused repositories
* Archive old repositories
* Optimize workflow efficiency

### Set Up Alerts

* Configure spending limits
* Set up usage alerts
* Get notified of unusual activity
* Prevent unexpected charges

---

## Key Takeaways

### Mental Model

```
Subscription = Access
├── Plan gives you access to features
└── Fixed monthly/annual cost

Metered Usage = Consumption
├── Pay for what you use
└── Variable cost based on usage
```

### Important Points

* Billing is **per organization**, not per repository
* Some features are **subscription-based** (fixed cost)
* Some features are **usage-based** (variable cost)
* License usage includes **human and non-human** consumers
* Usage reports help with **cost optimization**

---

## Next Steps

* Learn about access methods: `08_github-desktop-mobile.md`
* Review resources: `src/resources/official-links.md`
* Check exam prep: `src/exam-prep/01_key-definitions.md`

---

**Related Content**:
* Notes: `src/notes/exam-tips.md`
* Resources: `src/resources/official-links.md`

