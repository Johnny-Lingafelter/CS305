# CS305 - README.md

*Briefly summarize your client, Artemis Financial, and their software requirements. Who was the client? What issue did they want you to address?

Artemis Financial is a financial company offering retirement plans and savings accounts to their clients. The main issue they wanted to address was the security of their website and the security of the personal data regarding their clients that they stored on their servers.

*What did you do particularly well in identifying their software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall wellbeing?

I feel like I was able to identify what methods worked best for securing Artemis Financial's data rather well. This included manual inspecting their codebase and running dependency checks against it. It is extremely important to code securely in this day and age, because attackers are very prevalent and the landscape changes so frequently that if someone is not up to date with known vulnerabilities, it is only a matter of time before there is a security breach. Software security adds tremendous value to the company in the sense that they can be sure, and proud, that they are doing everything possible to protect their client's data from being compromised.

*What about the process of working through the vulnerability assessment did you find challenging or helpful?

For me, the most challenging part of working through the vulnerability assessment was correctly identifying which sections to apply to the specific codebase. This confused me at first, but after working through the modules in this course it made sense why each step of the assessment was necessary and helpful for the project.

*How did you approach the need to increase layers of security? What techniques or strategies would you use in the future to assess vulnerabilities and determine mitigation techniques?

Adding layers of security consists of things such as using HTTPS instead of HTTP and using cipher algorithms when data is particularly sensitive. I have learned many techniques for mitigation in this course, and in the future, I would start by immediately running a dependency check on the codebase. I believe this is one of the most important steps you can take to securing an application. Vulnerabilities are constantly being discovered, and if you let the codebase sit unchecked and do not upgrade the libraries you are asking for trouble. This needs to be a regular activity and should be integrated into the company’s business processes. Also, if using a CA and certificate on the server, care should be taken to ensure that the certificate is always valid, and that the server is configured correctly. Finally, manual inspection and testing of any and all new code added to the project needs to happen at multiple stages of development. Integrating a DevSecOps culture is strongly recommended for most companies.

*How did you ensure the code and software application were functional and secure? After refactoring code, how did you check to see whether you introduced new vulnerabilities?

To ensure functionality and security after refactoring, it is always advisable to run the code and try to "break" it or find ways to cause the program to behave unexpectedly. This allows you to be ahead of users and attackers and not be surprised when something unexpected happens with the application. Using the dependency check tool immediately after refactoring is also strongly recommended to avoid introducing new vulnerabilities into the codebase.

*What resources, tools, or coding practices did you employ that you might find helpful in future assignments or tasks?

The most helpful resource and tool that I will employ in the future is the OSWAP database and the Maven dependency check tool. I was unaware of this tool before this course, and I can see now how this tool is indispensable when dealing with codebases that rely on multiple third-party libraries. These codebases are much too large to facilitate manual inspection, and a tool such as dependency checking saves an enormous amount of time and effort. This is a must have tool in any developer’s toolbox.

*Employers sometimes ask for examples of work that you have successfully completed to demonstrate your skills, knowledge, and experience. What from this particular assignment might you want to showcase to a future employer?

Personally, I am most proud of the code in SslServerApplication.java that hashes a message using a MessageDigest object and the SHA-256 cipher algorithm. I believe I wrote this code cleanly and securely and would be happy to show any future employer my work. I would also demonstrate my ability to use and understand a tool like Maven's dependency check suite, which I believe is valuable to any employer that is concerned with the security of their application and the safety of their clients.
