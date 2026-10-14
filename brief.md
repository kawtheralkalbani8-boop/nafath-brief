Version:NAFATH-V4
Track:Networking
Overview
A national service provider must secure its software supply chain from development to deployment and operation. Software security protects configuration and secrets, while AI security addresses attacks on models and training data. Mobile security verification helps identify weaknesses before applications are released. Networking controls protect internet traffic from unauthorized redirection, and cybersecurity practices reduce exposure to critical vulnerabilities in software components. Data transparency, supported by a Software Bill of Materials (SBOM), helps teams identify affected dependencies and respond to incidents. These fields work together because a weakness in one component can threaten the entire service. The provider should combine secure development, application testing, route validation, dependency tracking, monitoring, and incident response rather than relying on a single control. This brief examines how these measures reduce supply-chain risks, with particular attention to BGP route hijacking and RPKI.
Software
The Twelve-Factor App methodology requires deployment-specific configuration to be stored in environment variables rather than hardcoded in source code. This includes database credentials, service tokens, and other settings that vary between deployments. Secrets should be provided through controlled, secure mechanisms and never committed to the repository. Separating configuration from code reduces accidental exposure and allows settings to change without modifying or rebuilding the application.
Resource: The Twelve-Factor App - III. Config - https://www.12factor.net/config
Ai
Adversarial machine learning attacks target different stages of an AI system. Evasion attacks manipulate inputs during use to cause incorrect predictions, while poisoning attacks corrupt training data or the learning process to influence the resulting model. Privacy attacks attempt to reveal information about training data, and model extraction attacks seek to reproduce a model through queries. These categories differ in their targets and objectives, so defenses must address both training and deployment.
Resource: Adversarial Machine Learning: A Taxonomy and Terminology of Attacks and Mitigations - https://csrc.nist.gov/pubs/ai/100/2/e2025/final
Mobail
The OWASP Mobile Application Security Verification Standard (MASVS) defines security and privacy controls for mobile applications. It covers areas such as data storage, cryptography, authentication, network communication, platform interaction, code quality, resilience, and privacy. Developers and security testers use these controls to assess an app systematically. The Mobile Application Security Testing Guide (MASTG) provides testing guidance to help verify whether the required controls are implemented effectively.
Resource: OWASP MASVS - https://mas.owasp.org/MASVS/
Networking
Border Gateway Protocol (BGP) is the postal service of the Internet. When someone drops a letter into a mailbox, the Postal Service processes that piece of mail and chooses a fast, efficient route to deliver that letter to its recipient. Similarly, when someone submits data via the Internet, BGP is responsible for looking at all of the available paths that data could travel and picking the best route, which usually means hopping between autonomous systems.
Resource: What is BGP? - https://www.cloudflare.com/learning/security/glossary/what-is-bgp/
Cybersecurity
Products designed with Secure by Design principles prioritize the security of customers as a core business requirement, rather than merely treating it as a technical feature. During the design phase of a product’s development lifecycle, companies should implement Secure by Design principles to significantly decrease the number of exploitable flaws before introducing them to the market for widespread use or consumption. Out-of-the-box, products should be secure with additional security features such as multi-factor authentication (MFA), logging, and single sign-on (SSO) available at no extra cost.
Resource: Secure by Design - https://www.cisa.gov/securebydesign
Data
A "Software Bill of Materials" (SBOM) acts as a detailed, nested inventory that lists the specific components making up a software product. The following documents, developed through an open and transparent collaborative process, were approved by consensus among stakeholders to enhance software component transparency. Further details regarding the NTIA multistakeholder process on this topic can be found in the available documentation.
Resource: Software Bill of Materials - https://www.ntia.gov/page/software-bill-materials
Misconception in My Track
Open Question
