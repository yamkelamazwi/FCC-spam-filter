# Spam Filter

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)

![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

A simple spam detection tool built with JavaScript and Regular Expressions.

This project scans user messages for common spam phrases and catches attempts to bypass filters by replacing letters with numbers or symbols.

## Features

- Detects common spam phrases
- Handles leetspeak substitutions
- Case-insensitive matching
- Whole-word phrase matching
- Uses JavaScript Regular Expressions

## Spam Patterns Detected

### Free Money

Matches variations such as:

- free money
- fr3e money
- fre3 money
- fr33 m0n3y

Example regex:

```js
const freeRegex = /(?:^|\s)fr[e3][e3] m[o0]n[e3]y(?:$|\s)/i;
