# Changelog

All notable changes are documented here. Versions follow Semantic Versioning.

## Unreleased

### Added

- Initial generic OCI Language MCP server.
- Seven atomic shared-pretrained tools for language detection, text classification, NER, key
  phrases, sentiment analysis, PII processing, and synchronous text translation.
- API-aligned action-oriented tool identifiers with human-readable MCP titles, exposed by
  the generic `oci-language-mcp` server identity.
- Stdio and hardened Streamable HTTP transports.
- OAuth resource-server mode, OCI workload identities, bounded execution, payload-safe
  telemetry, typed results, packaging, container, registry metadata, and public documentation.
- Bounded, safely quoted, domain-oriented human output for NER, key phrases, and detailed
  sentiment while retaining complete typed `structuredContent`.
- Correct non-authentication OCI 4xx classification, domain-specific failure headlines,
  PII exclusion disclosure, and sanitized `RELEXIFY` operational errors.

### Changed

- Use the shared `oracle-mcp-common` authentication context for outbound OCI Language clients.
- Document every supported runtime configuration and clarify the separate inbound and outbound
  authentication models.
- Make the container's prepared Python environment safe for non-root, read-only runtime use.
