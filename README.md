# Spam Filter

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
