## AT commands

The communication between user and modem is usually a serial type of communication with usage by way of AT commands.

AT command set, or AT commands are the most common way to control your modem. They are a command set consisting of a series of short text strings which
can be combined to produce operations such as dialing, hanging up, and changing the parameters of the connection.

There are basically 4 Types of at-cmd's

1. Set Commands - AT+<cmd>=<value> - Used to store values.
```
AT+CREG=1
```

2. Get Commands - AT+<cmd>? - Used to determine stored values.
```
AT+CREG?
```

3. Test Commands - AT+<cmd>=? - used to determine range of values supported.
```
AT+CREG=?
```

4. Execution commands - AT+<cmd>  - used to invoke a particular function.
```
AT+CREG
```


# Part 1: Command Type Parser
Write a function that can identify what type of AT command is given as input. The function should categorize the command as one of the following:
    1. Set Command (e.g., AT+CREG=1)
    2. Get Command (e.g., AT+CREG?)
    3. Test Command (e.g., AT+CREG=?)
    4. Execution Command (e.g., AT+CREG)

# Part 2: Command Storage Mechanism
Create a system to store multiple AT commands. This could be as simple as storing the commands in a dictionary or another data structure that makes it easy to retrieve them later.

# Part 3: Command Search Function
Implement a search function to look up a specific AT command in the stored data. If the command exists, return its details 
(e.g., type, stored value, or additional info). If it doesn't exist, return an appropriate message.

# Part 4
Add robust error handling to manage situations like:
    - Invalid AT commands.
    - Trying to search for a command that doesn’t exist.
    - Unexpected inputs (e.g., empty strings or malformed commands).

Make sure the system provides clear error messages to the user.







