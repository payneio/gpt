# gpt

A simple OpenAI text-generation utility.

Generates text with OpenAI's GPT models from a prompt given as an argument or on
stdin. Requires an OpenAI API key (`OPENAI_API_KEY`).

## Usage

```bash
gpt "Write a haiku about programming"     # Generate from a prompt
gpt -m gpt-4 "Explain quantum computing"  # Use a specific model
gpt -t 0.7 "Write a creative story"       # Adjust temperature
cat prompt.txt | gpt                      # Read the prompt from stdin
```

Composes well in pipelines:

```bash
pdf2md paper.pdf | gpt "summarize this"
```

## Install

```bash
uv tool install --editable .
```

## License

Copyright (C) 2026 Paul Payne. Licensed under the GNU AGPLv3 — see [LICENSE](LICENSE).
