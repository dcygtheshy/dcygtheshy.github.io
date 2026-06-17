# Deployment Checklist

## Replace Placeholders

The identity and GitHub URL are already set to `朱昊` and `dcygtheshy`.

Optional assets to replace:

- `src/assets/images/demo-avatar.png`
- `src/assets/images/demo-banner.png`

Core files to update:

- `src/config.ts`
- `src/content/spec/about.md`
- `src/content/posts/building-this-site.md`
- `astro.config.mjs`

## Local Commands

```powershell
$env:ASTRO_TELEMETRY_DISABLED='1'
$env:COREPACK_HOME='D:\codex\tools\corepack-home'
$env:USERPROFILE='D:\codex\tools\tmp'
$env:APPDATA='D:\codex\tools\tmp'
$env:LOCALAPPDATA='D:\codex\tools\tmp'
$env:TEMP='D:\codex\tools\tmp'
$env:TMP='D:\codex\tools\tmp'
$env:PNPM_HOME='D:\codex\tools\pnpm-home'
$env:PATH='D:\codex\tools\node-v22.12.0-win-x64;' + $env:PATH

D:\codex\tools\node-v22.12.0-win-x64\corepack.cmd pnpm install --store-dir D:\codex\tools\pnpm-store
D:\codex\tools\node-v22.12.0-win-x64\corepack.cmd pnpm build
D:\codex\tools\node-v22.12.0-win-x64\corepack.cmd pnpm preview --host 127.0.0.1 --port 4321
```

## Publish to GitHub Pages

Publish to `dcygtheshy.github.io`:

```powershell
D:\codex\tools\PortableGit\bin\git.exe init
D:\codex\tools\PortableGit\bin\git.exe branch -M main
D:\codex\tools\PortableGit\bin\git.exe add .
D:\codex\tools\PortableGit\bin\git.exe commit -m "Launch Astro personal blog"
D:\codex\tools\PortableGit\bin\git.exe remote add origin https://github.com/dcygtheshy/dcygtheshy.github.io.git
D:\codex\tools\PortableGit\bin\git.exe push -u origin main
```

In the GitHub repository settings, set Pages source to GitHub Actions if it is not selected automatically.
