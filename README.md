# 🔧 LPIC-1 Lab: 102.3 Manage Shared Libraries

## 📝 Introduction
In this lab, I explored the mechanics behind shared libraries in Linux. Shared libraries allow executables to reuse code, making systems more efficient. This lab helped me understand how to check dependencies, manage library paths, and ensure executables run properly.

I’ve included some helpful links to guide you through the lab and for studying afterward:

[LPIC Exam Objective 102.3](https://www.lpi.org/our-certifications/exam-101-102-objectives/#102.3_Manage_shared_libraries)

[102.3 NOTES](https://1drv.ms/w/c/354f1c8d534fbced/EceKeVlQJHJKvXPW91sCbxYBuwgB9ERJETpLuEY-A76niQ?e=YgEAVs)

[102.3 LAB](https://1drv.ms/w/c/354f1c8d534fbced/Ef38O2_Zoh5GrWdO7x_Dv98Bh_zca6oodNMDxJ1nXxBVvQ?e=Bacp7y)

---

## ✅ What I Did in This Lab
I used tools like ldd, ldconfig, and LD_LIBRARY_PATH to investigate and manipulate how executables locate and load shared libraries on a Linux system. I experimented with default and custom library paths and practiced both temporary and permanent solutions.

## 1️⃣ Identify Shared Libraries
🔹 Use ldd to find out what shared libraries an executable depends on

![8YOPEKg](https://github.com/user-attachments/assets/cece8b61-069a-43db-a555-e848e2e2367b)

🔹 View which .so files /bin/ls requires and where they reside.

![wfh9VqR](https://github.com/user-attachments/assets/b99422c8-d87e-4949-9563-6b2e05a9a62d)

## 2️⃣ Identify the Typical Locations of System Libraries

🔹 Explore common system directories that store shared libraries

![QG1AO0B](https://github.com/user-attachments/assets/f47e8391-8a33-44ed-be07-37f1728e2d09)

🔹 I Looked for files ending in .so.

![Q5cZoFy](https://github.com/user-attachments/assets/74a96eda-24e5-41f6-ad84-4f54d456e570)

## 3️⃣ Load Shared Libraries Temporarily Using LD_LIBRARY_PATH

🔹 Override the default library search path with a custom environment variable

🔹 Create a custom library directory:

![v6zpP2m](https://github.com/user-attachments/assets/4a54f928-fa93-4c21-9bf8-d93a7c77b276)

🔹 Temporarily point to your custom directory

![3w8KkrK](https://github.com/user-attachments/assets/f6e953f4-af63-4616-a92f-6bce3981a3ff)

![zG4wdWw](https://github.com/user-attachments/assets/3a67f49d-9ecc-4a28-9fba-88239665c453)

## 4️⃣ Load Shared Libraries Permanently Using ldconfig

🔹 Add and configure a permanent path for custom shared libraries

![ZIzZ7LB](https://github.com/user-attachments/assets/02902927-4ee0-4382-8fc4-a9de24e17183)

🔹 Update the shared library cache:

🔹 Update the shared library cache:

![MmCJApv](https://github.com/user-attachments/assets/5434cf40-f6b3-44bb-9a07-dcadc6bfaf9b)

## 💡 What I Learned
In this lab, I learned how shared libraries support program execution and how to check and resolve their dependencies. I practiced using LD_LIBRARY_PATH for temporary library paths and used ldconfig to register permanent ones. 🛠️ This is an essential part of Linux system administration and package troubleshooting.

