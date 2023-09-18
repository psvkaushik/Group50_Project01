# SE CSC510 Project01

**Group Number : 50**

Ayush Agarwal (aagarw36@ncsu.edu)

Kaushik Pillalamarri (spillal2@ncsu.edu)

Surya Upadyayula (supadya@ncsu.edu)

Vaishnavi Naik (vnaik@ncsu.edu)

> We have been assigned several projects, which we have now distributed among our team members. The projects are as follows:
> 
1. [Slash](https://github.com/NCSU-Group7-SE2021/slash/)
2. [Stock Guide and Analyst](https://github.com/lokesh45/StockPrediction)
3. [Tommas-Slash](https://github.com/TommasU/slash)
4. [Wolftrack 3.0](https://github.com/nehajaideep/WolfTrack3.0)
5. [GITS2.1-I.R.I.S](https://github.com/jayrshah98/GITS2.1-I.R.I.S)

> Below, we present our findings regarding these projects:
> 
1. **PROJECTS**
2. Slash:

> The slash application by NCSU-Group-7 aims at providing users a publicly accessible web API framework to scrape through popular e-commerce websites and provide the best deals possible.
> 
> 
> The interface through which users can interact with the application consists of both CLI and GUI. The repository provided a comprehensive guide to install the necessary tools to run the application. However, due to the code being more than two years old, there were multiple issues with the implementation on our mac.
> 
> The repo leverages the use of the npm module to install the requirements present in the ‘client/package.json’ file. For a person who hasn’t had any experience with using npm, I found it difficult to troubleshoot the issues I was facing while installing the requirements. After a tedious attempt to properly install the npm module, further complications came up when running the npm application. There were multiple errors that came up during the installation of the requirements listed in the package.json file which I was unable to troubleshoot.
> 
> As an application that was designed to be used by the general public for shopping, I felt that there was an extensive need for an updated guide/readme with exhaustive, easy-to-follow steps to install the required modules for the application to run properly. That would be a better suited repository intended for public use.
> 
1. Stock Guide and Analyst

> The stock exchange prediction application is a software that uses machine learning to analyze and compare the data collected from multiple companies on the stock market and provide a GUI to the user for analysis.
> 
> 
> The attempt to implement this code was extremely difficult as the code is almost three years old. The application uses two modes of implementation, one as a tester and the other as a developer. The tester way uses a Dockerfile that can be used to build an image that encompasses all the requirements, which can then be used to create a container that can run the application. Due to the code being old, there were packages in the Dockerfile that weren’t being used anymore. After correcting the Dockerfile, there were still issues with the installation of some of the requirements to create the image. With a heavy dependence on the Docker based implementation, I wasn't able to troubleshoot and successfully run the code as it was intended to.
> 
> The developer way of implementation used flask as the main utility to build the web application framework. This posed a great challenge as well due to outdated supporting modules that were required for the code to run correctly.
> 
> This repository had multiple issues according to me. The readme file just contained some screenshots of the WebUI they created, with a few commands on how to run it either as a tester or a developer. There was no proper documentation for troubleshooting issues that a user might face during installation. No steps were provided to install the main frameworks like Docker, Flask that are an essential part of their implementation. A general public user with no knowledge of what docker/flask is wouldn’t be able to use this application at all.
> 
1. Tommas-Slash

> Our evaluation of the "slash" project, designed to scrape major e-commerce websites and list top recommended products via a CLI or GUI, revealed a series of challenges. Initially, even after package installation, there were instances of missing packages, necessitating manual installations to fulfill dependencies.
> 
> 
> After resolving these package issues, we encountered difficulties with the import statements used in various Python modules within the codebase. It required extensive adjustments to ensure the proper functioning of the code.
> 
> Upon addressing the import statement issues, we were able to run the CLI version of the application. However, during CLI usage, we encountered further import statement problems that disrupted the user experience.
> 
> Subsequently, when attempting to run the Flask web application, we encountered yet more missing module issues. Surprisingly, individual examination of each Python file revealed no apparent issues, indicating a disconnect between the Flask setup and the codebase. These challenges collectively posed obstacles to achieving the desired functionality of the "slash" project.
> 
1. Wolftrack 3.0

> The WebGUI of the project ran well and they had clearly mentioned if any issue arises (which we think they might have encountered when trying test cases), what steps need to be taken. However, they also tried implementing the same using Docker to make it platform independent. When we tried that part of the project, we faced an issue. There were certain modules which needed to be installed while creating the Docker image of the application. This module installation was not mentioned anywhere in the repo. We learnt that when we encounter any issue during test cases, we need to make a note of the same so that we can summarize it in our report. This will help first time users to get better hold of the product. The only major issue while trying to run the project was some necessary modules were not told to be installed by the docker script, so once the packages were installed the application runs without any issues.
> 
1. GITS2.1-I.R.I.S

> We found this project very interesting because this project will help us students as well as in the industry.
> 
> 
> **Project Overview:**
> 
> GITS2.1 is an open-source project available on GitHub, which allows users to create and execute custom commands for GitHub operations. The repository for this project is well-maintained and thoughtfully documented, providing comprehensive details for users.
> 
> **Code Structure:**
> 
> The core code of GITS2.1, "gits.py," serves as the central module that imports functionality from other custom command scripts. Understanding this structure is crucial for those interested in extending or modifying GITS2.1.
> 
> **Custom Commands:**
> 
> One of the notable aspects of GITS2.1 is its collection of custom scripts for various GitHub commands, currently totaling 30 commands. These custom commands offer an array of functionalities, making GitHub operations more efficient and tailored to user needs.
> 
> **Platform Compatibility:**
> 
> GITS2.1 has been designed with platform compatibility in mind, offering separate setup instructions for Windows, Linux, and macOS environments. In this essay, we will delve into the experiences and challenges encountered when testing GITS2.1 on these different platforms.
> 
> Windows Compatibility:
> 
> When testing GITS2.1 on a Windows platform, we encountered no significant issues with code execution. However, one issue arose when executing the "gits push" command. This command called the "gits_push" function within the "gits_push.py" script, wherein we discovered that the repository name and authentication were hard-coded. This lack of documentation regarding the need to customize these parameters posed a challenge.
> 
> Linux Compatibility:
> 
> Testing on Ubuntu 20.04 LTS, we encountered an issue while running the "gits list" command. An error message, "code not found in the mentioned path," was displayed. Upon closer inspection, we identified that the code was missing the correct path for a variable. Once we corrected this issue, the command functioned as expected.
> 
> macOS Compatibility:
> 
> In our experience running software on macOS, we encountered several noteworthy issues. Firstly, there was a problem with a bash script that created directories in unintended locations, leading to file access issues. We had to modify the script to ensure it aligned with the correct folder structure, minimizing disruptions.
> 
> Secondly, despite the presence of a requirements.txt file in the repository, certain packages were missing upon installation, necessitating manual installation to meet dependencies.
> 
> Additionally, the code was designed to be cross-compatible with various operating systems, but the runtime OS detection for macOS was incorrect, causing unexpected behavior.
> 
> Furthermore, the lack of clear instructions for setting up GitHub repository authentication proved problematic. Instead of guidance, the previous team's credentials were present, raising concerns about data security. This issue was exacerbated by GitHub's policy change, which now requires login via ID and token rather than a passcode. We recommend establishing authentication as a system variable within a bash script for easier and more secure access management.
> 

II. **IMPROVEMENTS**

***We have decided to implement the [GITS2.1-I.R.I.S](https://github.com/jayrshah98/GITS2.1-I.R.I.S) project***. It applies the latest tech like python, Docker etc. We will improve upon the lessons learnt after executing the five projects mentioned above.

- Video Tutorials: Creating instructional video demonstrating the entire process of creating a repository and executing the operations mentioned in the code. This video could be provided as a separate link, offering first-time users a comprehensive guide on utilizing the application effectively.
- Error Handling and Documentation: In another project, 'Wolftrack,' we encountered a section that provided clear instructions on what to do when encountering a specific error. I found this information to be highly informative, especially for new users. I believe we can consider incorporating a similar approach into our current project.
- Streamlining Authentication Setup: To elevate user experience, we propose integrating authentication steps directly within the Bash script of GITS2.1. This approach will streamline the setup process across all platforms, making it more user-friendly and efficient.
- Issue Tracking: Mention/summarize issues observed when testing the project so that if any user encounters the issue they could refer to this document.