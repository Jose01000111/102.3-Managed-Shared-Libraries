# 🔧 LPIC-1 Lab: 102.3 Manage Shared Libraries

## 📝 Introduction
In this lab, I explored the mechanics behind shared libraries in Linux. Shared libraries allow executables to reuse code, making systems more efficient. This lab helped me understand how to check dependencies, manage library paths, and ensure executables run properly.

I’ve included some helpful links to guide you through the lab and for studying afterward:

[LPIC Exam Objective 102.3](https://www.lpi.org/our-certifications/exam-101-102-objectives/#102.3_Manage_shared_libraries)


---

## ✅ What I Did in This Lab
I used tools like ldd, ldconfig, and LD_LIBRARY_PATH to investigate and manipulate how executables locate and load shared libraries on a Linux system. I experimented with default and custom library paths and practiced both temporary and permanent solutions.

## 1️⃣ Identify Shared Libraries
🔹 Use ldd to find out what shared libraries an executable depends on

🔹 View which .so files /bin/ls requires and where they reside.

## 2️⃣ Identify the Typical Locations of System Libraries

🔹 Explore common system directories that store shared libraries

🔹 I Looked for files ending in .so.

🔹 Used file to check file types:

## 3️⃣ Load Shared Libraries Temporarily Using LD_LIBRARY_PATH
🔹 Override the default library search path with a custom environment variable

🔹 Create a custom library directory:

🔹 Temporarily point to your custom directory

## 4️⃣ Load Shared Libraries Permanently Using ldconfig

🔹 Add and configure a permanent path for custom shared libraries

🔹 Update the shared library cache:

🔹 Update the shared library cache:

## 💡 What I Learned
In this lab, I learned how shared libraries support program execution and how to check and resolve their dependencies. I practiced using LD_LIBRARY_PATH for temporary library paths and used ldconfig to register permanent ones. 🛠️ This is an essential part of Linux system administration and package troubleshooting.

