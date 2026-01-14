# 🔒 Security

## Reporting Security Vulnerabilities

**Please do NOT report security vulnerabilities through public GitHub issues.**

If you discover a security vulnerability, please send an email to:
**security@vulcanoconnects.ch**

Include:
- Description of the vulnerability
- Steps to reproduce
- Potential impact
- Suggested fix (if available)

We take all security reports seriously and will respond promptly.

## Security Best Practices

The Vulcano Community platform follows security best practices:

### Authentication & Authorization
- Email verification required for all accounts
- Secure password hashing (bcrypt)
- Session-based authentication via NextAuth.js
- CSRF protection enabled

### Data Protection
- SQL injection prevention via Prisma ORM
- XSS protection through React's built-in escaping
- Secure headers configuration
- HTTPS enforcement in production

### Infrastructure
- Rate limiting on API endpoints
- IP forwarding security for proxy environments
- Regular dependency updates
- Security audit logging

## Responsible Disclosure

We appreciate responsible disclosure and will:
- Acknowledge your report within 48 hours
- Provide regular updates on remediation progress
- Credit you in security advisories (if desired)
- Work with you to ensure proper fix before public disclosure

Thank you for helping keep Vulcano Community secure! 🛡️
