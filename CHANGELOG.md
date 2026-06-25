# Changelog

## Unreleased

- Support variable-length element types (e.g. `String`) in `savecube`/`savedataset` by no
  longer requiring a definite `sizeof` for the element type
- Estimate the copy-buffer size for `String` arrays by sampling actual element lengths
  instead of assuming a pointer-sized element, so `max_cache` is respected more closely
- DiskArrayEngine integration
