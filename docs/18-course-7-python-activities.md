# 18 Course 7 Python Activities

This chapter turns the Course 7 Python materials into hands-on activities. Each activity is designed for cybersecurity learners who need to practice the concept and explain the result clearly.

Read [17 Python for Security Automation](17-python-for-security-automation.md) first.

## Source-to-practice map

| Source material | Main concept | Activity |
| --- | --- | --- |
| `googlenotes.md` Course 7 notes | Python environments, data types, variables, conditionals, loops, modules, readability, file parsing | Activities 1-10 |
| Course 7 glossary | Vocabulary | Activity 11 |
| Python concepts from module 2 | Functions, built-ins, imports, comments | Activities 4, 5, 10 |
| Python concepts from module 3 | Strings, lists, indexes, regex | Activities 6, 7 |
| Python concepts from module 4 | Files, `.read()`, `.write()`, `.split()`, `.join()` | Activities 8, 9 |
| Reference guide for Course 7 | Combined syntax reference | Used across all activities |
| Algorithm for file updates in Python | Allow-list update workflow | Activity 9 and capstone |
| Instructions for including Python code | Portfolio presentation of code | Activity 12 |

## Activity 1: Pick the right Python data type

Fill in a data type for each security use case.

| Use case | Best data type | Why |
| --- | --- | --- |
| A username such as `bmoreno` |  |  |
| A failed-login count |  |  |
| Whether a user is approved |  |  |
| A list of blocked IP addresses |  |  |
| A unique set of suspicious domains |  |  |
| Parsed log fields such as user, IP, and status |  |  |

Answer key:

| Use case | Best data type |
| --- | --- |
| Username | String |
| Failed-login count | Integer |
| Approved or not approved | Boolean |
| Blocked IP addresses | List |
| Unique suspicious domains | Set |
| Parsed log fields | Dictionary |

## Activity 2: Write conditional logic

Scenario: You have an HTTP status code from a web log. Write a decision that prints a message.

Starter code:

```python
status = 503

# Add your conditional statement here
```

Expected solution:

```python
status = 503

if status == 200:
    print("Request succeeded")
elif status >= 500:
    print("Server error - investigate availability")
elif status >= 400:
    print("Client-side error - review request path")
else:
    print("Review status code")
```

Explain:

- `if` checks the first condition.
- `elif` checks another condition only if earlier checks are false.
- `else` handles everything not already matched.

## Activity 3: Loop through indicators

Scenario: Print each suspicious IP address from a list.

Starter code:

```python
suspicious_ips = ["10.10.4.23", "207.148.109.242", "192.168.1.25"]
```

Expected solution:

```python
suspicious_ips = ["10.10.4.23", "207.148.109.242", "192.168.1.25"]

for ip in suspicious_ips:
    print(ip)
```

Follow-up:

Add a condition that prints a special message when the IP is `207.148.109.242`.

```python
for ip in suspicious_ips:
    if ip == "207.148.109.242":
        print("Review external indicator:", ip)
```

## Activity 4: Create a function

Scenario: Calculate the percentage of login attempts that failed.

Starter code:

```python
total_attempts = 100
failed_attempts = 12
```

Expected solution:

```python
def calculate_fail_percentage(total_attempts, failed_attempts):
    fail_percentage = failed_attempts / total_attempts
    return fail_percentage

result = calculate_fail_percentage(100, 12)
print(result)
```

Explain:

- `total_attempts` and `failed_attempts` are parameters in the function definition.
- `100` and `12` are arguments in the function call.
- `return` sends the result back to the caller.

## Activity 5: Use built-ins and imports

Scenario: You have monthly failed-login counts.

```python
monthly_failed_attempts = [8, 12, 15, 9, 21, 11]
```

Tasks:

1. Print the highest value.
2. Print the lowest value.
3. Sort the values.
4. Calculate the mean with the `statistics` module.

Expected solution:

```python
import statistics

monthly_failed_attempts = [8, 12, 15, 9, 21, 11]

print(max(monthly_failed_attempts))
print(min(monthly_failed_attempts))
print(sorted(monthly_failed_attempts))
print(statistics.mean(monthly_failed_attempts))
```

## Activity 6: Work with strings and lists

Scenario: You need to normalize and update approved usernames.

Starter code:

```python
username = "SecurityAnalyst"
approved_users = ["elarson", "bmoreno", "tshah"]
```

Tasks:

1. Convert `username` to lowercase.
2. Append `btang` to the approved list.
3. Insert `wjaffrey` at index `2`.
4. Remove `elarson`.
5. Print the index of `tshah`.

Expected solution:

```python
username = "SecurityAnalyst"
approved_users = ["elarson", "bmoreno", "tshah"]

print(username.lower())

approved_users.append("btang")
approved_users.insert(2, "wjaffrey")
approved_users.remove("elarson")
print(approved_users.index("tshah"))
print(approved_users)
```

## Activity 7: Search with regular expressions

Scenario: Extract IP addresses from a log line.

Starter code:

```python
log_line = "Failed login for user bmoreno from 192.168.1.25"
```

Expected solution:

```python
import re

log_line = "Failed login for user bmoreno from 192.168.1.25"
ip_matches = re.findall(r"\d+\.\d+\.\d+\.\d+", log_line)
print(ip_matches)
```

Explain:

| Regex piece | Meaning |
| --- | --- |
| `\d+` | One or more digits |
| `\.` | Literal period |
| `re.findall()` | Return all matches as a list |

## Activity 8: Read and parse a file

Scenario: A file contains approved IP addresses separated by whitespace.

Example file text:

```text
192.168.25.60 192.168.140.81 192.168.203.198
```

Expected code:

```python
with open("allow_list.txt", "r") as file:
    file_text = file.read()

ip_addresses = file_text.split()
print(ip_addresses)
```

Explain:

- `with` helps manage and close the file.
- `"r"` opens the file for reading.
- `.read()` turns file contents into a string.
- `.split()` turns the string into a list.

## Activity 9: Update an allow-list file

Scenario: You need to remove IP addresses that no longer belong on the allow list.

Starter values:

```python
import_file = "allow_list.txt"
remove_list = ["192.168.25.60", "192.168.140.81"]
```

Expected algorithm:

```python
import_file = "allow_list.txt"
remove_list = ["192.168.25.60", "192.168.140.81"]

with open(import_file, "r") as file:
    ip_addresses = file.read()

ip_addresses = ip_addresses.split()

for element in remove_list:
    if element in ip_addresses:
        ip_addresses.remove(element)

ip_addresses = "\n".join(ip_addresses)

with open(import_file, "w") as file:
    file.write(ip_addresses)
```

Answer these questions:

| Question | Answer |
| --- | --- |
| Why use `.split()`? | To convert the file string into a list of IP addresses |
| Why loop through `remove_list`? | To check each IP that should be removed |
| Why check `if element in ip_addresses`? | To avoid removing a value that is not present |
| Why use `.join()`? | To convert the list back into text for the file |
| What does `"w"` do? | Opens the file for writing and replaces existing content |

## Activity 10: Debug broken code

Broken code:

```python
approved_users = ["bmoreno", "tshah", "elarson"]

for user in approved_users
print(user)
```

Problems:

- Missing colon after the `for` statement.
- `print(user)` is not indented inside the loop.

Fixed code:

```python
approved_users = ["bmoreno", "tshah", "elarson"]

for user in approved_users:
    print(user)
```

Debugging checklist:

1. Read the error message.
2. Check the line number.
3. Look for missing colons.
4. Check indentation.
5. Check data types.
6. Print small values to confirm logic.

## Activity 11: Vocabulary drill

Write one security-focused sentence for each term.

| Term | Your sentence |
| --- | --- |
| Algorithm |  |
| Automation |  |
| Boolean data |  |
| Bracket notation |  |
| Built-in function |  |
| Comment |  |
| Conditional statement |  |
| Debugging |  |
| File path |  |
| Function |  |
| Global variable |  |
| Immutable |  |
| Index |  |
| Interpreter |  |
| Iterative statement |  |
| Library |  |
| List concatenation |  |
| Local variable |  |
| Logic error |  |
| Method |  |
| Module |  |
| Notebook |  |
| Parameter |  |
| Parsing |  |
| PEP 8 style guide |  |
| Regular expression |  |
| Return statement |  |
| Syntax error |  |
| Type error |  |
| User-defined function |  |
| Variable |  |

## Activity 12: Prepare code for a portfolio

Use this checklist before sharing Course 7 Python work publicly.

| Check | Done |
| --- | --- |
| Code is your own work or allowed lab output |  |
| Raw lab directions are not included as screenshots |  |
| Code is readable in a monospaced font or clear screenshot |  |
| Sensitive usernames, IPs, account IDs, and session IDs are masked when needed |  |
| Comments explain intent |  |
| The writeup explains the scenario, algorithm, and result |  |

Short portfolio paragraph:

```text
I wrote a Python algorithm that opens an allow-list file, reads its contents, converts the contents into a list, removes IP addresses that should no longer have access, joins the updated list back into text, and writes the revised content back to the file. This automates a repetitive access-management task while keeping the steps clear and auditable.
```

## Capstone: automate an access update

Create a mini project with these sections:

1. Scenario: why the allow list must be updated.
2. Input: sample allow-list content and remove list.
3. Algorithm: plain-language steps.
4. Code: Python solution.
5. Output: updated allow-list content.
6. Security explanation: why this reduces risk.
7. Debugging notes: what you tested.
8. Portfolio note: what you would share publicly and what you would mask.

## Quick self-test

1. What does `.split()` return?
2. What does `.join()` return?
3. Why does a list work well for approved IP addresses?
4. Why is a set useful for unique indicators?
5. What is the risk of writing to a file with `"w"`?
6. What does `return` do inside a function?
7. What kind of error occurs when code runs but produces the wrong result?
8. What should be included when presenting Python code in a portfolio?
