Artemis Financial is a consulting company that creates client financial plans that cover investments, savings, retirement, and insurance plans. The company needed help modernizing their software, so that it could securely transmit sensitive data, like client and financial information. 

During this project, I found vulnerabilities in the app, like missing data verification and HTTPS security. Coding securely is extremely important to protect against fraud, data breaches, and cyberattacks. By strengthening software security, the company ultimately strengthens its trust with their clients and maintains a good reputation.

A challenging part of the vulnerability assessment was understanding how to run static code analysis tools like OWASP Dependency-Check. There are new NVD API restrictions that prevented me from doing so. However, it was helpful to learn how to work around real-world limitations and submit work that I felt was a good indication of proof. 

I set up HTTPS using a self-signed SSL certificate and added a SHA-256 checksum endpoint to verify data integrity - this added layers of security. In the future, I would use updated tools like Dependency-Check or Snyk to review vulnerabilities.

I manually tested the server startup, verified HTTPS was working, accessed the /hash endpoint, and reviewed console output for errors. I also performed static testing to make sure no new vulnerabilities were introduced.

Resources that helped included the OWASP Dependency-Check Maven tool, the Java Keytool utility for SSL certificates, and official Java documentation about cryptographic algorithms. I will keep using these in future projects.

For future employers, I would show this assignment to demonstrate my ability to refactor code securely, implement HTTPS, integrate encryption features, and apply secure development practices in a real-world project, even when issues arise, like the NVD API restrictions. 
