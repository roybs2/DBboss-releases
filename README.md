# DBboss

<p align="center">
  <img src="https://img.shields.io/badge/macOS-14%2B-007AFF?style=for-the-badge&logo=apple&logoColor=white" alt="macOS 14+" />
  <img src="https://img.shields.io/badge/PostgreSQL-Client-336791?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL Client" />
  <img src="https://img.shields.io/badge/Native-SwiftUI-FF6A00?style=for-the-badge&logo=swift&logoColor=white" alt="Native SwiftUI" />
</p>

<p align="center">
  <strong>A native macOS workspace for PostgreSQL.</strong><br />
  Browse schemas, run SQL, inspect tables, and keep common database work close at hand.
</p>

<p align="center">
  <a href="https://github.com/roybs2/DBboss-releases/releases"><img src="https://img.shields.io/badge/Download-Releases-34C759?style=for-the-badge" alt="Download DBboss" /></a>
</p>

---

## What DBboss Does

DBboss is a desktop PostgreSQL client built for macOS. It is designed for developers who want a fast, focused database workspace without leaving a native Mac app.

With DBboss you can:

- Save and manage PostgreSQL connections.
- Browse databases, schemas, tables, and columns.
- Open SQL tabs and run queries.
- Run the current SQL statement or the whole editor.
- Inspect query results in a grid.
- Browse table data with paging, search, and filters.
- Export result data as CSV, JSON, or SQL insert statements.
- Keep multiple database work tabs open in one workspace.
- Use a clean macOS interface with native menus, settings, and keyboard shortcuts.

## Download

Get the newest build from the **Releases** page:

<https://github.com/roybs2/DBboss-releases/releases>

For most testers, download the `.dmg` file, open it, then drag `DBboss.app` to your Applications folder.

## Install

1. Open the downloaded `DBboss-<version>.dmg`.
2. Drag `DBboss.app` into `Applications`.
3. Open DBboss from `Applications`.
4. Add a PostgreSQL connection and start working.

### macOS Security Notice

Current tester builds are not Apple Developer ID notarized yet. macOS may show a warning the first time you open the app.

If that happens:

1. Open Finder.
2. Go to `Applications`.
3. Right-click `DBboss.app`.
4. Choose **Open**.
5. Confirm that you want to open it.

This is expected for early tester builds distributed outside the Mac App Store.

## Updating

For now, updates are manual:

1. Download the newest release.
2. Quit DBboss if it is running.
3. Replace the old `DBboss.app` in `Applications` with the new one.
4. Open DBboss again.

Your settings and saved app data should remain in place when replacing the app.

## Your Data

DBboss stores app data outside the app bundle, so replacing `DBboss.app` does not normally remove your saved data.

Typical macOS locations:

- App: `/Applications/DBboss.app`
- App data: `~/Library/Application Support/DBboss/`
- Preferences: `~/Library/Preferences/com.royb.DBboss.plist`

Keep this in mind if you ever want to fully remove DBboss and its local data.

## Privacy And Network Access

DBboss connects to the PostgreSQL servers you configure. It does not need an account for this release repository, and this release repository does not contain the app source code.

Connection details are stored locally on your Mac. Be careful when using tester builds with production databases, and use read-only database users when possible.

## Checksums

Each release may include a `SHA256SUMS-<version>.txt` file. You can use it to verify that your downloaded `.dmg` or `.zip` matches the published artifact.

Example:

```bash
shasum -a 256 DBboss-<version>.dmg
```

Compare the output with the checksum file attached to the release.

## About This Repository

This is the public, release-only repository for DBboss downloads.

It intentionally contains only:

- Installer files
- Release notes
- Checksums
- Public download instructions

The DBboss source code is not published here.

## Author

DBboss was written by **Roy B.**
