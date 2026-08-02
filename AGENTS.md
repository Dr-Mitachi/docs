# Documentation project instructions

## About this project

- This is the internal communication handbook for Clinica Dr. Mitachi, built on [Mintlify](https://mintlify.com)
- Content is written in Romanian
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Non-technical managers edit content occasionally via the Mintlify web editor — keep MDX simple and robust
- Use the Mintlify MCP server, `https://mcp.mintlify.com`, to edit content and settings via MCP
- Use the Mintlify docs MCP server, `https://www.mintlify.com/docs/mcp`, to query information about using Mintlify via MCP

## Terminology

{/* Add product-specific terms and preferred usage */}
{/* Example: Use "workspace" not "project", "member" not "user" */}

## Style preferences

{/* Add any project-specific style rules below */}

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Component conventions

Keep it minimal — only convert where the mapping is obvious; leave normal instructions as plain text.

- Literal messages/scripts to **send or say to a patient** → blockquote (start each line with `> `)
- `NOTA BENE` notes → `<Note>` callout
- Standalone `ATENȚIE` cautions (their own line, not mid-sentence) → `<Warning>` callout
- Collapsible details / Q&A → `<Accordion>` inside `<AccordionGroup>`
- Step-by-step flows → `<Steps>` / `<Step>` (an `icon` on each `<Step>` is optional)
- Links between handbook pages use Mintlify heading anchors, e.g. `[text](/comunicare-chat#call-center-a1-apel-initial)`; the anchor is the heading lowercased with spaces → hyphens, so it breaks if the target heading is renamed

## Content boundaries

{/* Define what should and shouldn't be documented */}
{/* Example: Don't document internal admin features */}
