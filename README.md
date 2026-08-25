# Task 1 (reverse_string)

A simple Python utility function that reverses a given string.

## Function

```python
def reverse_string(s):
    return s[::-1]
```

## How It Works

The function uses Python's extended slice syntax `s[::-1]`:
- The first two colon-separated fields (`start` and `stop`) are left empty, meaning "the whole string."
- The third field, `-1`, is the **step**, telling Python to move backward one character at a time.

The result is a new string with the characters in reverse order.

## Usage

```python
print(reverse_string("hello"))  # Output: "olleh"
```

## Parameters

| Name | Type  | Description                  |
|------|-------|-------------------------------|
| `s`  | `str` | The string to be reversed.    |

## Returns

`str` — the reversed version of the input string.

## Notes

- Works on any string, including empty strings (`""` returns `""`).
- Since strings in Python are immutable, this returns a **new** string rather than modifying the original.
- Time complexity: O(n), where n is the length of the string.
