# Password Generator CLI

A Node.js CLI app.
It creates random passwords.
You control output with flags.

## Quick Start

Install packages:

```bash
npm install
```

Run app:

```bash
node passwordGenerator.js [flags]
```

Run tests:

```bash
npm test
```

## Flags

- `--help`
Show help message.

- `--length <number>`
Set password length.
Must be a positive integer.

- `--lowercase`
Use lowercase letters.

- `--uppercase`
Use uppercase letters.

- `--numbers`
Use digits.

## Defaults

- No `--length` flag:
Length defaults to `8`.

- No character flags:
Lowercase is used by default.

## Examples

```bash
node passwordGenerator.js
node passwordGenerator.js --length 12 --uppercase --numbers
node passwordGenerator.js --length 16 --lowercase --uppercase --numbers
node passwordGenerator.js --help
```

## Error Handling

Prints errors for:

- Unknown flags.
- Missing value after `--length`.
- Invalid `--length` values.
- Unexpected non-flag arguments.

## Testing

Unit tests verify flag use and 

Run tests:

```bash
npm test
```