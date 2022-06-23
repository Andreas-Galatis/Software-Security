# Software-Security
Projects done for CS-305 Software Security

*Briefly summarize your client, Artemis Financial, and their software requirements. Who was the client? What issue did they want you to address?*

•	The client for this project was Artemis Financial, a financial consulting company that develops individualized financial plans for savings, retirement, investments, and insurance for their patrons. 
•	Artemis Financial wanted to address the issue of software security for their organization, because they have a RESTful web application programming interface, and they wanted to ensure that they were protected from external threats. They needed our team to identify any security vulnerabilities in their current software and assist in determining a mitigation plan.

*What did you do particularly well in identifying their software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall wellbeing?*

•	What our team did well in identifying Artemis Financial’s software security vulnerabilities was in performing a manual code review according to a vulnerability assessment process flow used for conducting an architecture review and code review to identify vulnerabilities in code. This process flow helped identify any weakness in input validation, API interactions, cryptographic vulnerabilities, client/server communications, secure code handling, secure data structures, and overall secure coding practices. 
•	The first step in security is to code securely. The importance of this step cannot be understated. It is much more difficult and often costly to remediate security issues in coding post-production than it is during the after. Adhering to secure coding practices is also important for a software engineer as a matter of integrity and ethical values.
•	Companies benefit greatly from implementing software security into their organizational structure as it protects them, as well as their clients, from financial damage. It also helps the company uphold a sound reputation and trust with their customers. Additionally, it ensures all their data remains confidential.

*What about the process of working through the vulnerability assessment did you find challenging or helpful?*

•	The main challenge in working through the vulnerability assessment was determining was trying to understand what caused them and how to mitigate them. This called for much research and thorough analysis. Also determining which vulnerability was a false positive and whether or not it had to be suppressed presented some challenges, however, looking up an OSS Index data to see which ones were valid vulnerabilities was helpful and proved to be effective in sorting through the false positives.  With the false positives out of the way, the team could then focus their attention on mitigating the critical vulnerabilities associated with Artemis Financial’s web application.

*How did you approach the need to increase layers of security? What techniques or strategies would you use in the future to assess vulnerabilities and determine mitigation techniques?*

•	We approached the need to increase layers of security by adding an SHA-256 encryption algorithm cipher with a checksum. We also generated appropriately signed certificates to reassure those visiting the website that they were not on a site that may have been impersonating Artemis Financial. And lastly, we made sure to verify secure communications by implementing HTTPS protocols to the API.
•	To assess vulnerabilities and determine mitigation techniques in the future, we plan on continuously practicing effective code reviews and following the vulnerability assessment process flow to weed out any weak areas in the code. We also plan on relying on tools such as the Maven dependency check and OWASP’s reliable reports that detail each found vulnerability and ways to mitigate them.

*How did you ensure the code and software application were functional and secure? After refactoring code, how did you check to see whether you introduced new vulnerabilities?*

•	We ensured that the code and software application were functional and secure by first practicing secure coding practices, and then testing it repeatedly. We verified the output on the web browser and made sure that the secure connection icon was displayed in the tab. We also verified the output on the IDE console to make sure that the ssl server application had deployed effectively. And lastly, we verified that the proper certificate was generated and was being used through the keystore mechanism.
•	To ensure we didn’t introduce any new vulnerabilities to the application, we first ran a Maven dependency check prior to making any changes to the code. Then after refactoring the code, we ran another dependency check and cross referenced the two dependency check reports to make sure no new vulnerabilities we introduced.

*What resources, tools, or coding practices did you employ that you might find helpful in future assignments or tasks?*

•	One resource that will be useful in future assignments is the OWASP top ten list of web application security risks (OWASP Top Ten Web Application Security Risks | OWASP, n.d.). This report details the most common security risks involved when developing web applications. This will also be helpful in developing solid coding practices. By being thorough and detail oriented, as well as well-versed in all the vulnerability risks, we can ensure that our coding is secure and effectively guarded from hackers. And along with the available resources and good practices, we plan on using dependency checks and performing routine tests to make sure we are not introducing vulnerabilities in our applications, as well as being made aware of new ones.

*Employers sometimes ask for examples of work that you have successfully completed to demonstrate your skills, knowledge, and experience. What from this particular assignment might you want to showcase to a future employer?*

•	Some elements of this project that we would like to showcase to future employers is our ability to create a self-signed certificate by using the Java Keytool from the command line. Also, our ability to implement a SHA-256 algorithm cypher by means of a checksum verification, as well as code a RESTful application to have secure HTTPS protocol. And lastly, our ability to perform a manual code review, run a dependency check, identify false positives, and effectively recommend mitigations for the valid vulnerabilities.


*References*
OWASP Top Ten Web Application Security Risks | OWASP. (n.d.). Owasp.Org. https://owasp.org/www-project-top-ten/

