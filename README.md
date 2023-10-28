# Changing Environment Variables on Windows 10 / 11

Welcome to the guide on how to change environment variables on Windows 10 and 11. This step-by-step tutorial will show you how to modify these variables for any application or system-wide use. Environment variables are crucial for configuring various software and tools, and understanding how to manage them is essential for system administrators, developers, and power users.

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Changing Environment Variables](#changing-environment-variables)
  - [Using the System Properties](#using-the-system-properties)
  - [Using PowerShell](#using-powershell)
- [Using Environment Variables](#using-environment-variables)
- [Best Practices](#best-practices)
- [Troubleshooting](#troubleshooting)
- [Conclusion](#conclusion)

## Introduction

Environment variables are system-level or user-specific settings that are used to configure software applications. They store information such as file paths, system paths, and application-specific settings. Modifying environment variables is often necessary to tailor your system to your needs, or to make specific software work as expected.

This guide will walk you through the process of changing environment variables on Windows 10 and 11, using both graphical user interfaces and PowerShell.

## Prerequisites

Before proceeding, ensure that you have:

- A Windows 10 or 11 operating system.
- Administrative rights for system-wide environment variable changes.
- Basic knowledge of the software or application you wish to configure.

## Changing Environment Variables

### Using the System Properties

1. **Open the System Properties:**
   - Right-click on **This PC** or **My Computer**.
   - Select **Properties**.
   - Click on **Advanced system settings**.
   - In the System Properties window, click on the **Environment Variables** button.

2. **Modify or Add a Variable:**
   - In the Environment Variables window, under "User variables" or "System variables," select the variable you want to modify or click **New** to create a new one.
   - Provide the variable name and value.
   - Click **OK** to save your changes.

### Using PowerShell

1. **Open PowerShell:**
   - Type `PowerShell` in the Windows search bar.
   - Right-click on **Windows PowerShell** and select **Run as administrator**.

2. **Modify Environment Variables:**
   - To change user-level variables:
     ```powershell
     [System.Environment]::SetEnvironmentVariable("VARIABLE_NAME", "NEW_VALUE", "User")
     ```

   - To change system-level variables:
     ```powershell
     [System.Environment]::SetEnvironmentVariable("VARIABLE_NAME", "NEW_VALUE", "Machine")
     ```

3. **Verify Changes:**
   - Close and reopen applications that rely on the environment variable to ensure the new setting is recognized.

## Using Environment Variables

Once you've changed the environment variables, you can configure applications to use them. Each application will have its own method for utilizing environment variables, so consult the documentation or settings of the specific software or tool.

## Best Practices

- Use descriptive variable names.
- Backup important variables before making changes.
- Understand the scope of user-level and system-level variables.
- Keep a record of changes for reference.

## Troubleshooting

- Check for typos in variable names.
- Verify that the changes have taken effect by restarting the application.
- Ensure that the variable values are correctly formatted.

## Conclusion

Understanding how to change environment variables in Windows 10 and 11 is a valuable skill for optimizing your system and configuring applications to your needs. This guide has walked you through the process, offering both GUI and PowerShell methods for making these changes.

Feel free to explore and experiment with environment variables to enhance your Windows experience and make your software work more effectively.

For any questions, feedback, or suggestions, please feel free to reach out. Happy configuring!

**Author:** [Lalatendu](https://github.com/Lalatenduswain)
