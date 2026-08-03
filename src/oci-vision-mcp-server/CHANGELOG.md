# Changelog

## [Unreleased]

### Added

- Added public Oracle MCP package layout under `oracle/oci_vision_mcp_server`.
- Added the `oracle.oci-vision-mcp-server` stdio entry point.
- Added OCI SDK additional user-agent telemetry for Vision and Object Storage clients.

### Changed

- Updated runtime dependencies to FastMCP 3.4.2, OCI SDK 2.179.0, and Pydantic 2.12.3.
- Disabled browser-based session authentication by default; it remains available by setting `OCI_MCP_AUTO_AUTH=true`.
- Use the shared `oracle-mcp-common` authentication context for OCI Vision and Object Storage clients.
- Default the OCI profile to `DEFAULT` and defer Vision compartment validation until a Vision operation requires it.
- Restrict Vision image inputs to OCI-supported JPEG/PNG images no larger than 5 MiB.

### Fixed

- Include image-validation and Object Storage download code in the coverage gate.
- Honor `OCI_CONFIG_FILE` during session-token validation and refresh checks.

## 0.1.0

### Added

- Initial OCI Vision MCP server with Vision analysis, Object Storage upload/list, result lookup, and configuration status tools.
