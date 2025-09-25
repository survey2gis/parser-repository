# Survey2GIS Parser Repository

Community repository for parser configurations used by [parser-generator.survey-tools.org](https://parser-generator.survey-tools.org/).

## Repository Structure

```
parser/
├── default.ini
├── testing.ini
└── ...
parser.json
README.md
```

## Adding a Parser

1. **Add your parser file** to the `parser/` directory
2. **Update `parser.json`** with your parser information:

```json
{
  "your-parser-name": {
    "filename": "./parser/your-parser-name.ini",
    "author": "Your Name/Organization",
    "description": "Brief description of what this parser handles"
  }
}
```

## Example parser.json Entry

```json
{
  "default": {
    "filename": "./parser/default.ini",
    "author": "Landesamt für Muster",
    "description": "Ein Parser für Profile …"
  }
}
```

## Contributing

1. Fork this repository
2. Add your parser file to the `parser/` directory
3. Update `parser.json` with your parser information
4. Submit a pull request

Your parser will be available to all users of the Survey2GIS Parser Generator once merged.

## File Requirements

- Parser files must be valid `.ini` format
- Use descriptive filenames (lowercase, hyphens preferred)
- Provide clear, helpful descriptions in `parser.json`
