# Code Scanning Overview

**Session**: 04 - Configuring Code Scanning on GitHub  
**Domain**: Security and Compliance (20%)  
**Duration**: ~33 minutes

---

## Why Code Scanning Matters

Security is most effective when it runs alongside everyday development work, not as a last-minute gate.
Code scanning helps teams spot potential vulnerabilities and risky coding patterns early, when fixes are cheaper and easier.

### The Shift-Left Approach

**Traditional Approach**:
* Develop code
* Test functionality
* Security review at the end
* Fix issues late (expensive)

**Shift-Left Approach**:
* Security checks during development
* Catch issues early
* Fix before production
* Lower cost and risk

---

## What Is Code Scanning?

Code scanning is the automated analysis of source code to identify security vulnerabilities, coding errors, and unsafe patterns before code reaches production.

### How It Works

* **Static Analysis**: Examines code without running it
* **Pattern Detection**: Looks for known risky patterns
* **Automated**: Runs as part of CI/CD pipeline
* **Continuous**: Scans on every change

### What Code Scanning Detects

* **Security Vulnerabilities**: SQL injection, XSS, authentication flaws
* **Code Quality Issues**: Unused variables, dead code, complexity
* **Unsafe Patterns**: Hardcoded secrets, weak encryption, insecure APIs

---

## Code Scanning vs Other Scanning Types

### Code Scanning

* Analyzes **your source code**
* Looks for risky patterns in your code
* Detects vulnerabilities you introduce
* Scans the code you write

### Dependency Scanning

* Analyzes **libraries you use**
* Checks for known vulnerabilities in dependencies
* Detects issues in third-party packages
* Scans packages from package managers

### Secret Scanning

* Detects **exposed credentials**
* Looks for API keys, passwords, tokens
* Scans for secrets in code and history
* Prevents credential exposure

### Key Mental Model

```
Code Scanning = Analyze YOUR code for risky patterns
Dependency Scanning = Analyze LIBRARIES you use
Secret Scanning = Detect EXPOSED CREDENTIALS
```

---

## GitHub Advanced Security

### What Is Advanced Security?

GitHub Advanced Security is a set of security features available on GitHub Enterprise plans. It includes:

* **Code Scanning**: Automated security analysis
* **Secret Scanning**: Credential detection
* **Dependency Review**: Dependency vulnerability checking
* **Security Advisories**: Coordinated vulnerability disclosure

### Plan Requirements

* **Free/Team**: Limited security features
* **Enterprise**: Full Advanced Security features
* **Public Repos**: Some features available for free

---

## Enabling Code Scanning

### Repository-Level Configuration

Code scanning is enabled at the repository level. You can enable it through:

* **GitHub Actions**: Automated workflows
* **Third-Party Tools**: External security scanners
* **Native GitHub**: Built-in scanning (Enterprise)

### Using GitHub Actions

GitHub Actions workflows can run code scanning tools automatically:

* **On Push**: Scan when code is pushed
* **On Pull Request**: Scan before merging
* **On Schedule**: Regular scheduled scans
* **Manual**: Trigger on demand

---

## Code Scanning Workflow

### Typical Workflow

1. **Developer Pushes Code**: Makes changes and pushes
2. **Workflow Triggers**: GitHub Actions runs automatically
3. **Scan Executes**: Code scanning tool analyzes code
4. **Results Generated**: Issues and alerts created
5. **Developer Reviews**: Checks Security tab
6. **Issues Addressed**: Fixes vulnerabilities
7. **Re-scan**: Verifies fixes

### Scan Triggers

**On Push**:
* Scans every commit
* Immediate feedback
* Catches issues quickly

**On Pull Request**:
* Scans before merge
* Prevents bad code from merging
* Review as part of PR process

**On Schedule**:
* Regular scans (daily, weekly)
* Catches new vulnerabilities
* Comprehensive coverage

---

## Viewing Scan Results

### Security Tab

* Central location for security findings
* Shows all security alerts
* Organized by type and severity
* Links to detailed information

### Code Scanning Alerts

* List of detected issues
* Severity levels (critical, high, medium, low)
* File and line number
* Description and remediation guidance

### Alert Details

Each alert includes:
* **Severity**: How serious is it?
* **Location**: Where in the code?
* **Description**: What's the issue?
* **Remediation**: How to fix it?
* **References**: Additional resources

---

## Third-Party Code Scanning Tools

### Why Use Third-Party Tools?

* **Specialized Coverage**: Tools focused on specific languages or frameworks
* **Customization**: More configuration options
* **Integration**: Already using specific tools
* **Compliance**: Meet specific requirements

### Popular Tools

* **CodeQL**: GitHub's own analysis engine
* **SonarQube**: Code quality and security
* **Snyk**: Security scanning
* **Checkmarx**: Application security testing
* **Veracode**: Static analysis

### Integration via GitHub Actions

Third-party tools integrate through GitHub Actions:

* Tool runs as workflow step
* Results uploaded to GitHub
* Alerts appear in Security tab
* Unified view of security issues

---

## Understanding Alerts

### Alert States

* **Open**: Active issue, needs attention
* **Dismissed**: Marked as not relevant
* **Fixed**: Issue resolved in code

### Severity Levels

* **Critical**: Immediate security risk
* **High**: Significant security concern
* **Medium**: Moderate security issue
* **Low**: Minor security concern
* **Note**: Informational finding

### Alert Lifecycle

1. **Detected**: Scan finds issue
2. **Alert Created**: Appears in Security tab
3. **Reviewed**: Developer examines
4. **Fixed**: Code updated
5. **Verified**: Re-scan confirms fix
6. **Closed**: Alert resolved

---

## Best Practices

### For Developers

* **Review Alerts Promptly**: Don't ignore security findings
* **Fix Critical Issues First**: Prioritize by severity
* **Understand the Issue**: Read descriptions carefully
* **Test Fixes**: Verify solutions work
* **Learn from Findings**: Improve coding practices

### For Teams

* **Enable Scanning Early**: Set up from project start
* **Automate Everything**: Use GitHub Actions
* **Review Regularly**: Check Security tab often
* **Set Policies**: Define severity thresholds
* **Track Metrics**: Monitor security trends

### For Organizations

* **Standardize Tools**: Use consistent scanning tools
* **Enforce Policies**: Require scanning on all repos
* **Provide Training**: Educate developers
* **Monitor Compliance**: Track security posture
* **Invest in Security**: Allocate resources

---

## Common Misconceptions

### Misconception 1: "Code scanning finds all vulnerabilities"

**Reality**: Code scanning finds many issues but not all. It's a tool, not a guarantee.

### Misconception 2: "Only security teams need code scanning"

**Reality**: All developers benefit from code scanning. Security is everyone's responsibility.

### Misconception 3: "Code scanning slows down development"

**Reality**: Modern tools are fast. The time saved by catching issues early outweighs scan time.

### Misconception 4: "Code scanning is too complex"

**Reality**: GitHub makes it easy with starter workflows and automation.

---

## Guided Exercise: Enable Code Scanning

### Step 1: Choose a Repository

* Select a repository to scan
* Ensure you have admin access
* Consider starting with a test repo

### Step 2: Enable Code Scanning

* Go to repository Settings
* Navigate to Security & analysis
* Enable code scanning
* Choose scanning method

### Step 3: Configure Workflow

* Use starter workflow if available
* Or create custom workflow
* Configure scan triggers
* Set up notifications

### Step 4: Trigger Scan

* Make a commit
* Or create pull request
* Workflow runs automatically
* Wait for results

### Step 5: Review Results

* Go to Security tab
* View code scanning alerts
* Examine findings
* Understand severity

### Step 6: Address Issues

* Fix critical issues first
* Update code
* Commit changes
* Verify fixes

---

## Next Steps

* Learn about dependency scanning: `dependency-secret-scanning.md`
* Explore branch protection: `branch-protection.md`
* Study permissions: `permissions-roles.md`
* Practice with labs: `../labs/`

---

**Related Content**:
* Dependency Scanning: `dependency-secret-scanning.md`
* Branch Protection: `branch-protection.md`
* Permissions: `permissions-roles.md`
* Labs: `../labs/`

