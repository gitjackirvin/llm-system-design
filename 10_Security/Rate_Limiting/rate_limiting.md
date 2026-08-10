Explanation: This section explains how rate limiting will take place and why it is necessary to ensure LLM system functionality.

In order to follow industry best‑practice rate‑limiting methods, rate limiting needs to take place at both Nginx and the FastAPI gateway. When requests reach Nginx, they should be rate limited based on IP address to prevent DoS attacks and bandwidth exhaustion. At the FastAPI gateway, rate limiting could be enforced based on authentication, ensuring users only receive a certain number of requests within a defined time frame. 
Importance: Rate Limiting is important because it prevents tokens from being exhausted by spam requests and mitigates loss of service from DoS attacks.
