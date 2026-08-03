# Documentation project instructions

## About this project

- This is the internal **knowledge base** for Clinica Dr. Mitachi, built on [Mintlify](https://mintlify.com)
- Content is written in Romanian
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Non-technical managers edit content occasionally via the Mintlify web editor — keep MDX simple and robust
- Use the Mintlify MCP server, `https://mcp.mintlify.com`, to edit content and settings via MCP
- Use the Mintlify docs MCP server, `https://www.mintlify.com/docs/mcp`, to query information about using Mintlify via MCP

## Structure (multi-domain)

- The KB is organized by **domain**. Each domain is a top-level **Tab** (`docs.json` → `navigation.tabs`) whose pages live in a **folder** of the same name.
  - `comunicare/` — "Comunicare cu clienții" (the first and most complete domain)
  - `receptie/`, `sisteme/` — scaffolded future domains (placeholder landing pages)
- `index.mdx` (root) is the KB landing that routes into the tabs. Shared/global pages (landing) stay at root.
- **Each domain follows the same internal shape:** Start aici → concepte/overview → proceduri/how-to → referință → resurse. Reuse this when building a new domain.
- **To add a domain:** create a `<domain>/` folder, add its pages, add a new tab in `navigation.tabs`. Don't reshuffle existing domains.
- **When moving/renaming a page,** add a `redirects` entry (`docs.json` → `redirects`) from the old path so bookmarks/links don't break.
- Internal links use absolute paths including the folder, e.g. `[Etapa Contact](/comunicare/etapa-contact)`; anchors use Mintlify heading slugs.
- Pages marked "Pagină în lucru" contain `de completat de manager` placeholders (KPIs, common mistakes, escalation, CRM screenshots) awaiting internal input.

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
