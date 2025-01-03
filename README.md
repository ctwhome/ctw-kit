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

### First-time Setup

You'll need to set up two tokens in your repository's secrets (Settings → Secrets and variables → Actions):

1. `PAT_TOKEN`: A GitHub Personal Access Token with repo permissions
   - Go to GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
   - Generate new token (classic)
   - Select scopes: `repo` (full control of private repositories)
   - Copy the token and add it as a repository secret named `PAT_TOKEN`

2. `NPM_TOKEN`: An npm automation token
   - Go to npmjs.com → Access Tokens → Generate New Token
   - Select type: Automation
   - Copy the token and add it as a repository secret named `NPM_TOKEN`

After setting up these tokens, the automation will handle everything else - just push your changes to main using conventional commits.

## License

MIT
