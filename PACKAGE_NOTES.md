# Package notes

- `README.md` uses local animated GIF previews because GitHub's own documentation states that SVG images do not support inline scripting or animation in its rendered view. The matching animated SVG sources are supplied at the root and linked under each preview.
- SVGs retain a visible static state underneath their motion. Their CSS and SMIL animation is suppressed when the viewer requests reduced motion (in viewers that honor the SVG media rule).
- Character portraits are embedded directly as PNG data URIs inside the SVGs. The SVGs do not request remote images or web fonts. Text uses local system font stacks; no font download is needed. Font files are not bundled—the text falls back to fonts already installed on the viewer’s system.
- There is no JavaScript in the delivered SVG or README assets. CSS keyframes and SMIL are used for SVG motion, with static visible content as the fallback.
- The SVGs are self-contained, but an SVG data URI can be subject to host-specific sanitization. GitHub README uses the corresponding GIF files for dependable motion and retains links to the source SVGs.
- The dashboard does not invent follower, star, repository or contribution numbers. It links to the profile for live data.

## Install

1. Create a public repository named exactly `shadidahamed` under the account `shadidahamed` (GitHub's profile README convention).
2. Upload the contents of this package to the repository root, preserving `.github/workflows/` and `previews/`.
3. Open **Actions** → **GitHub-Profile-3D-Contrib** → **Run workflow** once. Approve Actions if GitHub asks you to enable it.
4. The package includes a visual placeholder at `profile-3d-contrib/profile-night-view.svg`. When the first run succeeds, the action overwrites it with the generated live 3D contribution calendar. Scheduled runs then refresh it daily.

## Personalization boundary

Only the details supplied in the request are present. GitHub is the only social URL included. No follower count, project title, email, or other social account was guessed.
