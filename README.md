# one-pager webtools

Single-file browser tools. No build step, no backend, no install — open the HTML file and it runs.

## Universal Prompt Generator

`prompt-generator.html`

A prompt authoring workbench for three distinct prompt shapes, because they fail in different ways:

| Type | Fields it structures |
|---|---|
| **System** | Role, guiding principles, environment constraints, output structure |
| **Chat** | Persona & tone, communication style, example dialogue, custom instructions |
| **Agent** | Role & mission, high-level policies, capabilities & tools, workflow, thinking process |

- Per-field **Generate** buttons — draft one section at a time instead of staring at a blank prompt
- Side-by-side diff of your version against the model-refined version, so you can see what the refinement actually changed
- Copy-to-clipboard on both
- Backends: Gemini 2.0 Flash or OpenAI GPT-4, selectable at runtime

**On API keys:** you supply your own, and the page calls the provider directly from your browser. There is no server here to proxy or store anything — this is a static file. Keys live only in the page session.

Built with vanilla JS and Tailwind. One file, ~zero dependencies.

## Running it

Clone and open `prompt-generator.html` in a browser, or serve the folder with any static server.

## License

GPL-3.0
