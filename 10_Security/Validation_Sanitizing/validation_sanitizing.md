10.4. Data Validation 
Explanation: This section explains why data validation is important for security and where it should be applied. 

Data validation should occur at both the Nginx layer and the FastAPI gateway. When requests reach Nginx, it ensures HTTP headers are correctly formatted and sized, verifies that the request body does not exceed the maximum allowed size, and rejects malformed or oversized requests. After passing through Nginx, requests reach the FastAPI gateway, where authentication is verified, JSON body structure is validated, and token usage is checked against maximum allowed limits. 
Importance: Data validation is important because it reduces unnecessary token usage, enforces security standards, and prevents malicious or improperly formatted data from entering the system. 

10.5. Data Sanitization
Explanation: This section explains why data sanitization is important for security and where it should be applied. 

Data sanitization should occur at the FastAPI gateway. All incoming user input should have valid formatting, contain no null bytes, and include no unreadable characters before being processed. Database queries should be checked against a defined list of allowed parameters so common SQL injection methods cannot be used. Content filtering rules may also be applied to block prompt injection attempts, malicious payloads, or prohibited content before it reaches the LLM. 
Importance: Data sanitization helps protect backend services from malicious actors, mitigate attacks as well as prevent errors from occurring.
