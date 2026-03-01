# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project follows [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.0] - 2026-03-01

### Added

- Rule builder: support for up to 2 conditions with `AND` / `OR`.
- Rules modal split views: `Available Rules` and `Create Rule`.
- Domain input hint and validation for `domain` match type.
- Bookmark Rules UI localization coverage for newly added labels and hints.
- Welcome modal and onboarding polish.
- Build metadata stamping for release artifacts.
- Expanded localized screenshots for store listings.
- Added auto-close when entering fullscreen setting.
- Added Cmd+Shift+K / Ctrl+Shift+K to open the sidebar.

### Changed

- Rules/tag layout and mode-toggle UX improvements.
- Screenshot flow now closes modals with `Esc`.
- Release/prepare pipeline improvements (version bumping, packaging, and publish flow).
- Settings and toolbar copy updates across locales.
- Screenshot capture automation updates and sync flow.

### Fixed

- Modal and popover keyboard-close behavior (`Esc`) consistency.
- Rules builder validation and interaction edge cases.
- Search/filter cleanup (including duplicate URL legacy cleanup).

## [1.0.0] - 2026-02-23

### Added

- Initial public release of Bookmark Keep (Chrome + Firefox extension + website).
