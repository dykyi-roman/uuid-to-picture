# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2026-02-23

### Added

- UUID to dot-matrix picture encoding with customizable segment colors
- Picture to UUID decoding via PNG upload or drag & drop
- Random UUID v4 generation using `crypto.getRandomValues()`
- PNG and SVG export support
- One-click clipboard copy of decoded UUIDs
- Responsive design for desktop and mobile
- 6x6 grid layout with 2x2 dot matrices per hex character
- 5 distinct color segments matching UUID structure
- Roundtrip verification (encode then decode produces original UUID)
