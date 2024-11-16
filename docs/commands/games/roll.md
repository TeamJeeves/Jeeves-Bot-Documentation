## Roll Command

### Description
The `roll` command generates a random number between 1 and 100 by default, or within a custom range specified by the user.

### Usage
```
/roll [range]
```

### Options
- **range** (optional): Specify a custom range to roll between. You can provide a single number (e.g., `50`) to roll between 1 and that number, or two numbers (e.g., `5-1337`) to roll between those numbers.

### Permissions
- **User**: No special permissions required.
- **Bot**: No special permissions required.

### Examples
- Roll a number between 1 and 100:
  ```
  /roll
  ```
- Roll a number between 1 and 50:
  ```
  /roll range:50
  ```
- Roll a number between 5 and 1337:
  ```
  /roll range:5-1337
  ```

### Notes
- Ensure that the custom range is valid and contains no more than two numbers.
- The bot will reply with an error message if the range is invalid or if the specified number is too large.