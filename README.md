# PLP Python Week 6: Safe Functions

## File Descriptions
- `safe_tools.py`: Contains three safe functions (`safe_divide`, `safe_number`, `get_field`) that use `try...except` blocks to prevent crashes, along with the required test cases.
- `README.md`: This file, containing the assignment title, file descriptions, and a brief explanation of exception handling.

## Why an `if` check cannot catch "abc" on its own
An `if` check (such as `if text:`) only evaluates whether a string is empty or not, meaning it will evaluate to `True` for `"abc"`. It does not inherently validate the actual content or type of the string. While you could chain complex conditions (like `.isdigit()`), using a `try...except` block is the most reliable and Pythonic way to directly catch the `ValueError` raised when `int()` fails.
