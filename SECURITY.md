# Security Policy

## Reporting a Vulnerability

If you discover a security vulnerability, please report it responsibly:

1. **Do not** open a public issue
2. Email the maintainer at the address listed in the GitHub profile
3. Include a description of the vulnerability and steps to reproduce

You should receive a response within 48 hours. We will work with you to understand and address the issue before any public disclosure.

## Scope

This is a client-side only application with no server, no authentication, and no data storage. The primary security considerations are:

- XSS prevention in user inputs
- Safe handling of file uploads (PNG decoding)
- Secure use of `crypto.getRandomValues()` for UUID generation
