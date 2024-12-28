# AT Commands: Modem Communication Challenge

Modem communication often relies on **AT commands**, which are short text strings used to control modem functions such as dialing, hanging up, and managing connection parameters. These commands typically use serial communication and are categorized into four main types:

1. **Set Commands**: `AT+<cmd>=<value>` – Store values.  
   Example: `AT+CREG=1`

2. **Get Commands**: `AT+<cmd>?` – Retrieve stored values.  
   Example: `AT+CREG?`

3. **Test Commands**: `AT+<cmd>=?` – Determine the range of supported values.  
   Example: `AT+CREG=?`

4. **Execution Commands**: `AT+<cmd>` – Invoke a specific function.  
   Example: `AT+CREG`

## Problem Breakdown:

### Objective:
Design a system to manage AT commands efficiently, including parsing, storage, retrieval, and error handling. Implement the following functionalities:

---

### **Part 1: Command Type Parser**
Write a function to identify the type of an AT command based on its structure. The function should classify the command into one of the following categories:
- Set Command (e.g., `AT+CREG=1`)
- Get Command (e.g., `AT+CREG?`)
- Test Command (e.g., `AT+CREG=?`)
- Execution Command (e.g., `AT+CREG`)

---

### **Part 2: Command Storage Mechanism**
Develop a system to store and manage multiple AT commands. Use a data structure like a dictionary or a similar mechanism that allows:
- Storing the commands efficiently.
- Retrieving commands and their details based on user queries.

---

### **Part 3: Command Search Function**
Implement a search functionality that allows users to:
- Look up a specific AT command in the stored data.
- Return details such as its type, stored value, or any additional information.
- Provide a clear message if the command doesn’t exist.

---

### **Part 4: Error Handling**
Incorporate robust error handling to ensure the system can manage unexpected inputs and errors gracefully. For example:
- Handle invalid or malformed AT commands.
- Return meaningful error messages for empty strings or unsupported command formats.
- Provide clear feedback when trying to search for a nonexistent command.

---

### **Bonus Points:**
- Design the system for scalability, so it can handle a large number of commands.
- Include unit tests for the core functionalities (command parsing, storage, search, and error handling).
- Optimize for performance and readability.

---

### **Evaluation Criteria:**
- **Correctness:** Does the solution categorize, store, and retrieve AT commands correctly?
- **Clarity:** Are the code and error messages easy to understand and maintain?
- **Robustness:** Does the solution handle edge cases and unexpected inputs effectively?
- **Scalability:** Can the system handle more commands or adapt to additional functionality in the future?

This task is designed to evaluate your problem-solving skills, coding ability, and attention to detail. Feel free to use any programming language of your choice!

