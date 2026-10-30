<div align="center">

<img src="assets/icon.png" alt="Vera app icon" width="120" />

# Vera

**A calmer way to browse.**

A personal browser project focused on a clean browsing experience, useful shortcuts, saved pages, and privacy controls.

[Latest Releases](https://github.com/theDevstars/Vera/releases) · [Builds](https://github.com/theDevstars/Vera/actions) · [SideStore Source](sidestore-source.json)

</div>

---

## App preview

> **Real app screenshots coming soon.** The repository currently contains the Vera app icon but not screenshots of the running app. We’ll add the actual iPhone home screen, webpage view, and settings screens here once they’re supplied, so the gallery accurately represents the app.

| Home screen | Browsing | Settings |
|:--:|:--:|:--:|
| *Screenshot pending* | *Screenshot pending* | *Screenshot pending* |

## About Vera

Vera is built with Expo and React Native. The project is being developed with iPhone as the current release target, while keeping the project organized for future Android and Windows work.

### Current release focus

- **iPhone:** unsigned IPA produced through GitHub Actions on the `macos-26-intel` runner.
- **SideStore:** source manifest is maintained in this repository.
- **Android and Windows:** future build paths are kept separate from the current iOS release workflow.

An unsigned IPA is not App Store-signed. Installation requires a compatible signing and provisioning method, such as SideStore.

## Get Vera

1. Open the [GitHub Releases](https://github.com/theDevstars/Vera/releases) page.
2. Download the latest Vera IPA asset.
3. Install it using your compatible signing workflow.

To add Vera's SideStore source, use the raw manifest:

[`sidestore-source.json`](https://raw.githubusercontent.com/theDevstars/Vera/main/sidestore-source.json)

## Build from source

Requirements: Node.js 20+ and the platform-specific build tools.

Install JavaScript dependencies:

```bash
npm install --legacy-peer-deps
```

Generate the iOS native project:

```bash
npx expo prebuild --platform ios --no-install
```

The primary iOS build is automated in [GitHub Actions](https://github.com/theDevstars/Vera/actions).

## Project structure

```text
.
├── .github/workflows/   # Automated build workflows
├── assets/              # Vera app icon and artwork
├── App.js               # Main application
├── app.json             # Expo app configuration
├── package.json         # Project dependencies and scripts
└── sidestore-source.json# SideStore source manifest
```

## Screenshots and contributions

When sharing screenshots, please use captures from the actual Vera app. Place them in a `screenshots/` folder and update the preview table above with their paths. Avoid mockups or unrelated images so the repository stays an accurate showcase of Vera.

---

<div align="center">

**Vera** · Built with care by [theDevstars](https://github.com/theDevstars)

</div>
