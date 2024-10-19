# AppSec best practices checklist

[ ] Encrypt sensitive data related to LLM models and datasets at rest and in transit.


[ ] Secrets management
- Encrypted secrets at rest.
- Use secure storage such as a vault to store LLM API keys.


[ ] Access control
- Least privilege on access to the LLM, as well as the LLM’s access to backend systems.
- Bounds between security and usability need clear definitions as elevated privilege may be needed in some cases.
- Least privilege for all LLM-based intellectual property ensuring only authorized personnel have access to these artifacts .


[ ] Source code management
- Store source code, executable code, infrastructure as code, and artifacts, for example: models, parameters, configurations, data, and tests in a version control system with proper access controls to ensure only validated code is used, and any changes are tracked.


[ ] Network segmentation and controls
- Isolate LLMs from public networks.
- Prevent scraping data from unintended data sources via restricted network access. 
- Sandbox the environment running LLM models within hardened containers or virtual machines.
- Rate limiting to prevent abuse of the LLM API. 


[ ] Input and output validation
- Ensure that the LLM model only processes acceptable and safe input formats. 
- Contextual output encoding wherever data is presented to the end user.


[ ] Use secure third-party libraries and frameworks.
 
[ ] Adversarial testing
- Evaluate the robustness, security, and overall performance of LLM models against malicious inputs.


[ ] Monitoring
- Intermediate service to enforce guardrails around LLM use.
- Real time detection and response capability to alert on anomalous behavior.
