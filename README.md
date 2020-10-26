# software-security-snhu
Coursework for CS-305 Software Security at SNHU

**Briefly summarize your client, Artemis Financial, and their software requirements. Who was the client? What issue did they want you to address?**

This was a scenario-driven project. The client, Artemis Financial, is a fictional financial consulting company that develops individual savings, retirement, investment, and insurance plans for their patrons. Artemis Financial wants to modernize their operations by improving their security. They have hired my software company to examine their web-based software application, and identify and mitigate security vulnerabilities.

**What did you do particularly well in identifying their software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall wellbeing?**

The aspect of my work on this project about which I am proudest is my thoroughness. Throughout this course we generated multiple vulnerability reports, identifying known vulnerabilities in a software application. The largest of these reports showed 26 vulnerabilities. I took the time to individually research each vulnerability as part of a defense-in-depth strategy. It is important to code securely, especially when utilizing multiple third-party dependencies (many of which are open source), as security incidents in software can have significant consequences. Even in a low-stakes context, when the risk posed by a breach is negligible, secure code is still more desirable for its reuseability and applicability to evolving security concerns.

**What about the process of working through the vulnerability assessment did you find challenging or helpful?**

For me, the most challenging aspect of vulnerability assessments was identifying the circumstances in which a piece of code or design pattern represents a vulnerability. The OWASP vulnerability report tool describes itself as a "best effort" and emphasizes the presence of both false positives and false negatives. Still, their reports are exceptionally helpful as they contain not only vulnerability information, but also thorough documentation of the vulnerability's identification and mitigation. Still, I think the most helpful thing while working through the vulnerability assessment was the advice found in Iron Clad Java, to treat all user-submitted data as unsafe and malicious. It helped me to be vigilant and critical in my assessments.

**How did you approach the need to increase layers of security? What techniques or strategies would you use in the future to assess vulnerabilities and determine mitigation techniques?**

I implemented various forms of security improvements, including SHA-256 checksum implementation using a self-signed certificate and keystore. In the future this plus appropriate key-exchange algorithms (such as RSA or Elliptic Curve Diffie-Hellmann) could form the basis of a modern and robust Internet security solution. I would also look to implement an SQL or similar database with automatic or forced parameterization, to prevent the risk of injection attacks or cross-site scripting.

**How did you ensure the code and software application were functional and secure? After refactoring code, how did you check to see whether you introduced new vulnerabilities?**

I tested the application in three separate web browsers (Firefox, Chrome, and Internet Explorer), and ran OWASP vulnerability assessment reports at multiple stages of the security assessment process to ensure I had not introduced any new vulnerabilities. If this had been a longer-term project, I would have sought to implement automated unit testing and regression testing via the JUnit test framework.

**What resources, tools, or coding practices did you employ that you might find helpful in future assignments or tasks?**

I have already used Java's MessageDigest library, which I learned in this course, to add password hashing to a mobile app created for another course. I also learned more about RESTful implementations, specifically Spring, which seem to represent an effective and common way to implement a web-application-server. I have no doubt that I will be learning about and using these much more in the future. I also plan to make use of the OWASP vulnerability assessment report tool on any and all future projects, to ensure I am not developing software with known vulnerabilities.

**Employers sometimes ask for examples of work that you have successfully completed to demonstrate your skills, knowledge, and experience. What from this particular assignment might you want to showcase to a future employer?**

I would want to emphasize the thoroughness and presentation of my vulnerability assessment reports. I would also highlight the components of my coursework that utilized SHA-256 cryptography, to demonstrate that I have an awareness of relevant industry-tested cryptographic standards.

----------
References
----------

Manico, J., &amp; Detlefsen, A. (2015). Iron-clad Java: Building secure web applications. New York: McGraw-Hill Education. Retrieved October 25, 2020, from https://learning.oreilly.com/library/view/iron-clad-java/9780071835886/
