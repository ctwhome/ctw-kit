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

When you push to main with conventional commits, the automation will:
1. Analyze commit messages and determine version bump
2. Update package.json version
3. Generate/update CHANGELOG.md
4. Create a GitHub release
5. Automatically publish to npm

For example:
```bash
# Add your changes
git add .

# Commit with conventional commit message
git commit -m "feat: add new component"  # for new features
git commit -m "fix: resolve styling issue"  # for bug fixes
git commit -m "feat!: redesign API"  # for breaking changes

# Push to main to trigger release
git push origin main
```

The automation handles everything - no manual steps needed.

## License

MIT
