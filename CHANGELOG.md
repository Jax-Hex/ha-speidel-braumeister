# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.0.3] - 2026-03-03

### Fixed
- Fixed "'DeviceDataResult' object is not a mapping" error when converting Pydantic v2 models to dictionaries in coordinator
- Added robust conversion with multiple fallback strategies (model_dump for Pydantic v2, dict for v1, vars fallback)
- Added debug logging to help diagnose future data conversion issues
- Improved error handling for API data conversion edge cases

### Technical Details
- The issue occurred when all data sources (XHR, Web API, Cloud API) failed for a device, leaving the coordinator with a DeviceDataResult object that couldn't be converted to a dict
- The fix ensures proper conversion regardless of Pydantic version or edge cases
- Debug logging now tracks which conversion method is being used (e.g., "Using model_dump() for conversion", "Using dict() for Pydantic v1", etc.)

## [2.0.2] - Previous Release

## [2.0.1] - Previous Release

## [2.0.0] - Previous Release
