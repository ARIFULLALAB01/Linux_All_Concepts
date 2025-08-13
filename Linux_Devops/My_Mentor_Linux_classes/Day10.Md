# Regular Expressions
  - [Refer Here](https://cheatography.com/davechild/cheat-sheets/regular-expressions/#google_vignette) for regular expressions cheatsheet

  - Next steps
    - sed
    - awk

   | Pattern | Description | Example |
| --- | --- | --- |
| ^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$ | Matches a valid email address | example@example.com[1][2] |
| ^https?:\/\/(?:www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\/?$ | Matches a basic URL | https://www.example.com[2] |
| \b\d{3}[-.]?\d{3}[-.]?\d{4}\b | Matches a US phone number in xxx-xxx-xxxx format | (123) 456-7890[1][2] |
| \b\d{5}(?:[-\s]?\d{4})?\b | Matches a US ZIP code in xxxxx or xxxxx-xxxx format | 12345 or 12345-6789[1][2] |
| ^[0-9]{1,2}\/[0-9]{1,2}\/[0-9]{4}$ | Matches a date in MM/DD/YYYY format | 12/25/2022[1][2] |
| ^[0-9]{1,2}:[0-9]{2}$ | Matches a time in HH:MM format | 17:30[1][2] |
| ^[a-zA-Z]+(?:[-'\s][a-zA-Z]+)*$ | Matches a name with optional spaces, hyphens, and apostrophes | John Doe or Mary-Ann O'Connor[2] |
| ^[1-9]\d*$ | Matches a positive integer | 42[2] |
| `^-?[1-9]\d*	^0$` | Matches an integer (positive, negative, or zero) |  |
| ^[1-9]?\d*\.\d+$ | Matches a floating-point number | 3.14, -1.5, 42.0[2] |
| ^[a-zA-Z0-9]+(?:_[a-zA-Z0-9]+)*$ | Matches a snake_case string | my_variable, snake_case_string[2] |
| ^[a-zA-Z0-9]+(?:-[a-zA-Z0-9]+)*$ | Matches a kebab-case string | my-variable, kebab-case-string[2] |