# Prompts

Personal library of LLM and image-generation prompts. Each prompt lives in a
category folder with a parameterized template and filled-in examples.

## Structure

    image/                    # image-generation prompts
    └── <style-name>/
        ├── TEMPLATE.md       # parameterized prompt with [PLACEHOLDERS]
        ├── tips.md           # model-specific flags, aspect ratios, known issues
        └── examples/         # one file per filled-in example
            └── <name>.md

## Adding an example

1. Copy `TEMPLATE.md` into `examples/<your-name>.md`.
2. Replace every `[PLACEHOLDER]` with concrete text.
3. Run it. Note the model and aspect ratio you used in the frontmatter.
4. If something works particularly well or poorly, add a `## Notes` section.

## Adding a new style

Create `image/<new-style>/` with its own `TEMPLATE.md`, `tips.md`, and
`examples/`. Don't add empty category folders (`llm/`, `coding/`) until you
have actual prompts to put in them.

## Conventions

- File names: `kebab-case.md`.
- Templates use `[PLACEHOLDER]` for substitution slots, defined inline at
  the top of each template.
- Examples are self-contained — paste the prompt block into your generator
  and it should run as-is.
