# M4riana

> The talking version of M3gan. Except this time, her name is M4riana.

M4riana is an open-source chatbot built with Next.js, inspired by the character M3gan. It keeps the cold, intelligent, and slightly unsettling tone of the character. You can change the persona to fit your own needs by editing a few files.

## Features

- Chat interface (Next.js + Tailwind + shadcn/ui)
- Persona defined in a separate file, so you can change the character without touching the core code
- Safety rule that breaks character and responds supportively when needed
- Run with Docker in a single command

## Setup

### Requirements
- Node.js 18+
- An LLM API key (added to `.env`)

### Steps

```bash
git clone https://github.com/CodeBrend/m4riana.git
cd m4riana
cp .env.example .env   # add your API key to .env
npm install
npm run dev
```

Open `http://localhost:3000` in your browser.

### With Docker

```bash
docker compose up --build
```

## Changing the persona

The character's personality is defined in `configuration/persona.ts`. Speaking style, rules, and example dialogues are set there.

## Tests

```bash
npm test
```

## License

This project is distributed under the license in the [LICENSE](./LICENSE) file.
