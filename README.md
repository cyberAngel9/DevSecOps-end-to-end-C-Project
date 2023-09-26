# Assignment for Creating an End to End DevSecOps Pipeline for .NET/C# project Modified by Angel AKA I0n1c.

This DevSecOps project has helped me gain a comprehensive understanding of how to conduct scans using SAST, SCA, and DAST tools. Most importantly, it has taught me how to identify vulnerabilities, make improvements to the scans, and effectively communicate these findings to the deployment team. The entire process was facilitated using SonarCloud, Synk, and GitHub Actions, all configured with the necessary permissions and tokens. 

# Static Application Security Testing (SAST) Scan with SonarCloud
Static Application Security Testing (SAST) involves evaluating an application's source code or binary code to detect and assess potential security vulnerabilities and weaknesses. The SAST scan has been successfully completed, and the results indicate that everything is in good shape. Upon reviewing the results on SonarCloud, it confirms that everything is in order, and the scan has passed without detecting any issues or security hotspots.

### Screenshot of the SAST scan.

![image](https://github.com/cyberAngel9/DevSecOps-end-to-end-C-Project/assets/82012925/8967fe99-c99d-436f-8b9e-9b66a9e2a935)

### Screenshot of the summary on Sonarcloud.

![image-1](https://github.com/cyberAngel9/DevSecOps-end-to-end-C-Project/assets/82012925/43c27f0d-30c4-4083-ac13-070c4305f492)

# Software Composition Analysis (SCA) with Snyk
Software Composition Analysis (SCA) is a security and vulnerability scanning method that emphasizes the identification and assessment of components and libraries utilized in a software application. SCA scans also analyze third-party and open-source libraries, frameworks, and dependencies to detect known vulnerabilities and potential security risks. Upon reviewing the results in GitHub Actions, it becomes evident that certain vulnerabilities have been identified. During the SCA scan, a total of 14 dependencies were tested, revealing three issues and three vulnerable paths.

There are three vulnerable paths identified:

Newtonsoft.Json version 12.0.2 exhibits an Insecure Defaults issue, rated as high severity. To resolve this, it's recommended to upgrade to version 13.0.1.

jQuery version 3.4.1 is vulnerable to Cross-Site Scripting (XSS), with a medium severity rating. The fix for this XSS vulnerability is to upgrade to version 3.5.0.

jQuery.Validation version 1.17.0 is susceptible to Regular Expression Denial of Service (ReDoS), rated as a high severity issue. To address this, it's advised to upgrade to version 1.19.3."

### Screenshot of the SCA Scan

![image-2](https://github.com/cyberAngel9/DevSecOps-end-to-end-C-Project/assets/82012925/56f85e6d-8d58-41d2-bc0d-6082f6d91e99)

### Screenshot of the vulnerabilities found in the SCA scan

![image-3](https://github.com/cyberAngel9/DevSecOps-end-to-end-C-Project/assets/82012925/169df909-feb0-492e-a94f-a6dcb4c89bb5)

# Dynamic Application Security Testing (DAST) with ZAP
Dynamic Application Security Testing (DAST) is a security testing approach that assesses running web applications from an external perspective. It covers a range of evaluation criteria, including external testing, runtime analysis, vulnerability detection, scalability assessment, authentication handling, compliance testing, report generation, remediation strategies, and integration with CI/CD pipelines.

Once the DAST scan is complete, it generates an artifact containing the scan report, which is available for download in three formats: HTML, JSON, and MD. Reviewing the report provides in-depth insights, including the risk level, vulnerability names, and Alert Details, enabling a comprehensive understanding of the scan results.

### Screenshot of the DAST scan

![image-4](https://github.com/cyberAngel9/DevSecOps-end-to-end-C-Project/assets/82012925/cf4aea4b-3143-46c1-994b-fc2e148cec2c)

### Screenshot of the ZAP Scanning Report

![image-5](https://github.com/cyberAngel9/DevSecOps-end-to-end-C-Project/assets/82012925/46dcd563-14c9-4b08-9762-e4b1324e428a)

## All three reports will be available for viewing in the repository under 'ZAP Reports'.

