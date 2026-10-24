
# SiteShield — Test Plan

## 1. Normal URLs
- https://google.com
- https://paypal.com
- https://example.com

Expected: No obvious warning signs for these examples under the current rules.
Note: This does not prove the websites are safe.

## 2. Look-alike domains
- https://paypa1.com
- https://pay-pal.com
- http://paypal.com.example.org

Expected: Brand impersonation warnings where applicable.

## 3. Connection and hostname warnings
- http://example.com
- https://192.0.2.1/login
- https://xn--e1afmkfd.example

Expected: HTTP, IP address, or punycode warnings.

## 4. Suspicious URL patterns
- https://bit.ly/example
- https://example.com/login/verify
- https://this-is-a-very-long-example-hostname-that-should-trigger-a-warning.com

Expected: Relevant warning indicators when the current rules detect them.

## 5. Invalid input
- Empty input
- ftp://example.com
- //example.com
- https://
- A URL containing spaces

Expected: A clear validation error; no broken results screen.

## 6. Safety checks
- A low score must never be described as proof of safety.
- The submitted URL must not be fetched by this prototype.
- User-provided text must not be interpreted as HTML.
