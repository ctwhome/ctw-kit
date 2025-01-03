# CTW Kit

Custom components and utilities for Svelte and TailwindCSS (DaisyUI)

## Installation

```bash
bun add ctw-kit
# or
npm install ctw-kit
```

## Components

- [SEO](src/lib/components/SEO/README.md) - SEO meta tags management including Open Graph and Twitter cards

## Development

1. Clone the repository
```bash
git clone https://github.com/ctwhome/ctw-kit.git
cd ctw-kit
```

2. Install dependencies
```bash
bun install
```

3. Start development server
```bash
bun run dev
```

4. Build the package
```bash
bun run build
```

## Publishing

This package uses fully automated releases. Simply write commits using [Conventional Commits](https://www.conventionalcommits.org/) format and push to main:

```bash
# New features (minor version bump)
git commit -m "feat: add new button component"

# Bug fixes (patch version bump)
git commit -m "fix: correct button styling"

# Breaking changes (major version bump)
git commit -m "feat!: redesign component API"
```

When you push to main, the automation will:
- Update the version based on commit messages
- Generate CHANGELOG.md
- Create a GitHub release
- Publish to npm

Everything happens automatically - no manual steps or approvals needed.

## License

MIT
