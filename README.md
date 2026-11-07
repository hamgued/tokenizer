# Tokeniser Explorer

An interactive teaching tool that compares two meanings of "token":

- **LLM tokeniser** – splits text the way OpenAI models do (o200k_base and cl100k_base encodings), with colour-coded tokens, token IDs and tokens-per-word.
- **Linguistic tokeniser** – word and sentence tokens, types, type/token ratio, mean sentence and word length, and a frequency list.

Includes a short explainer, four guided tasks and a Sources tab.

Designed by [Hamid Guedra](https://www.linkedin.com/in/hagu1/) (Language Centre, [LAB University of Applied Sciences](https://lab.fi/en)).

## Technical notes

- Single file: `index.html`. No build step.
- The LLM tab loads [gpt-tokenizer](https://github.com/niieani/gpt-tokenizer) 2.9.0 (MIT) from jsDelivr on first use (about 2 MB per encoding).
- The linguistic tab uses the browser's built-in `Intl.Segmenter`.
- All text stays in the user's browser.

## Publish on GitHub Pages

1. Create a new public repository on GitHub and upload `index.html` and `README.md`.
2. Go to **Settings → Pages**, set **Source** to *Deploy from a branch*, branch `main`, folder `/ (root)`, and save.
3. The tool appears at `https://<your-username>.github.io/<repository-name>/` within a few minutes.
