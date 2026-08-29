# Documentation project instructions

## About this project

- This is a documentation site built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- The active product contract is exposed at `https://mcp.standatpd.com/api/codex/schema`
- Separate shipped behavior from planned behavior in every page

## Terminology

- Use `Source` for the persisted type and “Fuente” in user-facing explanations.
- Use “Perfil” for an `Actor` with `is_profile = true`.
- Do not call `Post` or `Snippet` official Codex items; they are auxiliary storage types.
- Use “preset” as a template of fields, not as a new item type.
- Use `field_key` as identity and `label` as presentation text.

## Style preferences

{/* Add any project-specific style rules below */}

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Content boundaries

- Document public Codex, REST and MCP behavior.
- Do not publish secrets, service-role keys, private user data or raw access tokens.
- Do not describe a proposed endpoint as active until it can be verified in the deployed service.
