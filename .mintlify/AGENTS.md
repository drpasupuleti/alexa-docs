# Documentation Agent Instructions

## Code Examples

- Use TypeScript for all code examples. The SDK and its consumers are TypeScript-first.
- Always include import statements at the top of code examples.
- Show both Builder Pattern and Factory Function approaches for directive construction.
- Use realistic parameter values (e.g., `"episode-42"`, `"https://example.com/podcast.mp3"`) — avoid `foo`/`bar` placeholders.
- Include error handling examples when demonstrating `build()` methods that throw.

## Component Usage

- Use Mintlify `<Tabs>` to show Builder Pattern vs Factory Function side by side.
- Use `<Warning>` callouts for deprecation notices and breaking changes.
- Use `<Info>` callouts for supplementary context and cross-references.
- Use `<Note>` callouts for edge cases and optional parameters.
- Use `<Update>` components with tag filters for changelog entries.
- Use `<CardGroup>` for overview pages listing available modules.

## Style and Formatting

- Write for skill developers with intermediate TypeScript experience.
- Use active voice and second person ("you").
- Keep sentences short and direct. Avoid filler words.
- Use pipe tables for listing methods, error types, enums, and constants.
- Mark deprecated features with "(Deprecated)" in the page title and frontmatter description.
- Include a migration path and deadline when deprecating features.

## Page Structure

- Every directive page should include: description, code examples (tabbed), builder methods table, and validation behavior.
- Every handler page should include: type guards table, extraction utilities, error types, and handler interface.
- Every types page should include: interfaces with inline comments explaining each field.
- Add cross-links between related directive, handler, and type pages.

## Changelog

- Use Mintlify `<Update>` components with `label` (date), `description` (short title), and `tags` for filtering.
- Tag categories: "New Feature", "Deprecation", "Breaking Change", "Documentation".
- Order entries newest first.

## Project Context

- This documents the `alexa-apl-interface` TypeScript SDK for building Alexa skill responses.
- Supported interfaces: APL, APLA (deprecated), APLT, AudioPlayer (V1 + V2), VideoApp (deprecated), HTML, DataStore, PackageManager.
- The SDK provides builder classes, factory functions, type guards, extraction utilities, and validators.
