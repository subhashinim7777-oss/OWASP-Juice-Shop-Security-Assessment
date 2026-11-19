# OWASP Juice Shop – Web Application Security Assessment

## Project Overview

This project documents a hands-on web application security assessment performed using **OWASP Juice Shop**, an intentionally vulnerable web application designed for security training and learning.

The assessment was conducted in a local testing environment to understand common web security concepts, explore application vulnerabilities, inspect HTTP responses, and document practical observations.

## Objectives

- Set up and run OWASP Juice Shop in a local environment.
- Explore authentication and access control challenges.
- Understand common web application security vulnerabilities.
- Investigate Cross-Site Scripting (XSS).
- Inspect HTTP response headers using browser Developer Tools.
- Document testing observations, screenshots, and security recommendations.

## Tools and Technologies

| Tool | Purpose |
|---|---|
| OWASP Juice Shop | Vulnerable training application |
| Node.js | Application runtime |
| npm | Package management |
| Google Chrome | Application testing |
| Chrome Developer Tools | DOM and HTTP header inspection |
| Windows 11 | Testing environment |

## Testing Environment

- **Operating System:** Windows 11
- **Application:** OWASP Juice Shop
- **Version:** 20.4.0-SNAPSHOT
- **Node.js:** v24.11.0
- **npm:** v11.6.1
- **Local URL:** http://localhost:3000

## Practical Activities and Progress

### 1. Application Setup
- Downloaded and extracted the OWASP Juice Shop application.
- Started the application locally.
- Verified successful access through the browser.

### 2. Authentication Challenge
- Explored the Login Admin challenge.
- Successfully completed the built-in administrator login challenge.

### 3. Score Board Challenge
- Located the hidden Score Board page.
- Successfully completed the Score Board challenge.
- Observed the challenge progress through the application dashboard.

### 4. XSS Investigation
- Explored the application search functionality.
- Inspected the DOM using Chrome Developer Tools.
- Investigated search input behaviour.
- Further testing is required to confirm successful XSS execution.

### 5. HTTP Response Header Analysis
- Used the Network panel in Chrome Developer Tools.
- Inspected HTTP response headers.
- Observed headers such as:
  - Access-Control-Allow-Origin
  - Cache-Control
  - X-Content-Type-Options
  - X-Frame-Options
  - Content-Type

## Evidence and Screenshots

Screenshots collected during the practical assessment are maintained in the `screenshots/` directory.

They include:

1. OWASP Juice Shop application interface and Login Admin challenge completion.
2. Score Board challenge completion.
3. HTTP response header inspection.
4. Search functionality and DOM inspection.

## Key Learnings

- Understanding the fundamentals of web application security.
- Exploring authentication and access control challenges.
- Learning how to inspect HTML elements and the DOM.
- Understanding HTTP response headers.
- Using browser Developer Tools for security analysis.
- Documenting testing evidence and observations.
- Learning the importance of responsible security testing.

## Security Recommendations

- Implement proper authentication and authorization.
- Validate user inputs on the server side.
- Use parameterized queries to prevent SQL injection.
- Apply context-aware output encoding to prevent XSS.
- Configure appropriate HTTP security headers.
- Restrict cross-origin access to trusted origins.
- Follow the principle of least privilege.

## Project Documentation

The detailed technical report contains the testing procedures, observations, screenshots, results, and security recommendations.

**Report:** `OWASP-Juice-Shop-Security-Assessment.docx`

## Disclaimer

This assessment was conducted strictly within a local OWASP Juice Shop training environment for educational purposes.

No unauthorized third-party systems were targeted.

## References

- [OWASP Juice Shop](https://owasp.org/www-project-juice-shop/)
- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [OWASP Security Cheat Sheets](https://cheatsheetseries.owasp.org/)
- [OWASP Juice Shop GitHub Repository](https://github.com/juice-shop/juice-shop)

---

**Project Type:** Web Application Security Assessment  
**Prepared by:** Subhashini  
**Internship Organization:** SWYNEX Technology
