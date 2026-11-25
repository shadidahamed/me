# Rendering & compatibility checks

- Chromium browser rendering: **5/5 SVGs passed**.
- CSS animation instances detected: **all five SVGs animate**.
- Reduced-motion preference: **passed for all five SVGs**.
- Mobile image width test at 390px: **no horizontal overflow**.
- Animated GitHub GIF previews: **5/5 contain multiple frames**.
- README local image/link targets: **7/7 resolve inside this package**.
- Workflow YAML syntax: **passed**.
- External image dependencies in README: **none**.

This is a local Chromium and file-reference test, not a live GitHub upload test. GitHub's rendered SVG view does not play SVG animation, so README embeds the local GIF previews and links each SVG source. The contribution-city image is replaced by the workflow after its first successful run.
