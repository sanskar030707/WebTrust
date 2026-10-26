# SiteShield 🛡️

### Look-Alike Website Detector

SiteShield is a beginner-friendly web application that analyzes website URLs for common warning signs associated with phishing and domain impersonation.

## Problem

Fake websites can imitate banks, government portals, and popular online services. Users may struggle to identify suspicious URLs before entering sensitive information.

## Solution

SiteShield examines visible URL characteristics and explains potential warning signs in simple language, helping users make more informed decisions before trusting a link.

## Features

- URL validation for HTTP and HTTPS addresses
- Detection of possible brand impersonation
- Warnings for IP-address hosts and punycode domains
- Detection of known URL shorteners
- Checks for unusual hostname patterns and account-related keywords
- Risk indicator score with explanations
- Input validation and clear error messages
- Responsive interface for desktop and mobile
- Browser-based analysis without sending submitted URLs to a server

## Technology Stack

- HTML5
- CSS3
- JavaScript
- Browser URL API

## Getting Started

1. Clone or download this repository.
2. Open the project folder in VS Code.
3. Open `index.html` using Live Server, or open it in a modern browser.
4. Enter a URL and select **Check URL**.

## Testing

Open `test.html` using Live Server and click **Run tests** to check representative URL inputs and expected behavior.

## Limitations

- This is a heuristic prototype, not a complete phishing-detection service.
- It does not query live threat-intelligence databases.
- Its list of known brand domains is limited.
- It may produce false positives or miss malicious websites.
- The score is not a probability of fraud.
- A low score does not guarantee that a website is safe.

## Future Scope

- Integrate a trusted threat-intelligence API.
- Expand and maintain official-domain references.
- Add more automated tests for URL edge cases.
- Improve detection accuracy using validated security data.

## Disclaimer

SiteShield is an educational project. Always independently verify a website before entering passwords, one-time codes, or payment details.
