# Security-Headers
Response Security Headers

🏦 Scenario: Online Banking Site
Imagine you're using an online banking website:

https://secure.mybank.com/account?user=john&session=abc123
You click a link inside the banking portal that takes you to an external partner site:

https://partner-rewards.com
🔍 Without Referrer-Policy
The browser sends this HTTP header to partner-rewards.com:

Referer: https://secure.mybank.com/account?user=john&session=abc123
✅ What just happened?

You unknowingly leaked:

Your username (john)

Your session token (abc123)

That you're viewing your bank account page

🔓 A malicious external site could now:

Steal your session token

Track your behavior on sensitive pages

Mount phishing attacks
