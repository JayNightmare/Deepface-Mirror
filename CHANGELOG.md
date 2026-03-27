# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased]

### Fixed
- Fixed `KeyError` crashes in `test_verify.py` and `test_analyze.py` by ensuring `modeling.py` dictionary global cache is correctly initialized.
- Fixed `FileNotFoundError` in API tests by replacing hard-coded Unix `/tmp/` paths with cross-platform `tempfile.gettempdir()`.
