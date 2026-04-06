# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2026-02-11

### Added
- GSAP node animations — entrance, hover, click, expand/collapse
- Interactive hover and click animations on graph connectors
- GSAP-animated draw-in for graph connectors
- PRD vertical sidebar list replacing horizontal pills
- Board view enhancements — filters, assignee, blocked, sorting

### Fixed
- Board filter bar wraps to two lines, always shows assignee filter
- ESLint security/detect-object-injection warnings in graph.ts
- PRD sidebar layout and sizing

## [0.9.4] - 2026-02-08

### Fixed
- Pass `--limit 0` to `bd list --all` to return all issues

## [0.9.3] - 2026-01-05

### Added
- ARM64-only release workflow

### Fixed
- Allow viewing closed tickets in tasks/:id view
- Simplified release workflow with mise and native builds

## [0.9.0] - 2026-01-03

### Added
- **Graph View**: Horizontal org-chart tree visualization replacing Cytoscape.js
- **Graph View**: Horizontal epic selector with pagination arrows
- **Graph View**: Curved SVG Bezier connectors with gradient fade
- **Graph View**: Status and type indicator dots on nodes
- **Graph View**: Hover glow effect on child nodes
- **PRDs View**: Horizontal PRD selector dropdown (matching graph style)
- **Theming**: Theme switcher with 6 themes (nacre-dark, nacre-light, catppuccin-mocha/macchiato/frappe/latte)
- **Theming**: Semantic color palette with theme-aware chart colors
- **Header**: Project folder name display below logo
- **Metrics**: Refactored to pure functions for improved testability (17 new unit tests)

### Changed
- **Graph View**: Tasks display in multiple rows with wrapping
- **Graph View**: Legend width matches epic selector box
- **Board View**: Added max-width and centering for consistency
- **Charts**: Use yellow instead of grey for Resolved bars

### Fixed
- **Metrics**: Cycle time calculation now correctly excludes issues without InProgress transitions
- **Metrics**: EventType parsing includes Deleted event type
- **Metrics**: Always show cycle time chart even with limited data
- **Board View**: Theme selector now visible
- **Markdown**: Table borders display correctly
- **Graph View**: Lighter nodes and darker lines for better readability

## [0.8.0] - 2026-01-01

### Added
- GFM tables and strikethrough support via `pulldown_cmark` options
- XML syntax highlighting for code blocks
- Chart navigation bar on `/metrics` page with anchor links
- Human-readable latency formatting
- ESLint configuration with security plugin for TypeScript

### Changed
- Refactored static assets to use `include_dir` crate

### Fixed
- Object injection warnings in frontend TypeScript
- Chart nav alignment with metrics grid

## [0.7.0] - 2025-12-30

### Added
- Initial tracked release

[1.0.0]: https://github.com/vectorian-rs/nacre/compare/v0.9.4...v1.0.0
[0.9.4]: https://github.com/vectorian-rs/nacre/compare/v0.9.3...v0.9.4
[0.9.3]: https://github.com/vectorian-rs/nacre/compare/v0.9.0...v0.9.3
[0.9.0]: https://github.com/vectorian-rs/nacre/compare/v0.8.0...v0.9.0
[0.8.0]: https://github.com/vectorian-rs/nacre/compare/v0.7.0...v0.8.0
[0.7.0]: https://github.com/vectorian-rs/nacre/releases/tag/v0.7.0
