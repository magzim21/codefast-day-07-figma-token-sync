# Codefast Day 07 · Figma Token Sync

## Mission
- Synchronize design tokens from Figma into JSON, Style Dictionary, and Tailwind layers on every push.
- Detect breaking token changes, notify relevant teams, and keep documentation current.

## Implementation Checklist
1. Configure token export pipeline using Figma REST API or Tokens Studio.
2. Normalize tokens into Style Dictionary categories and generate Tailwind config artifacts.
3. Publish tokens to npm or internal CDN, versioned and annotated with commit metadata.
4. Add drift detection comparing production CSS variables to latest token set.

## Telemetry & QA
- Emit Datadog RUM events when token changes propagate to runtime UI.
- Add unit tests for token transforms and schema validation for incoming payloads.

## Deliverables
- README covering setup, environment variables, and release workflow.
- Change log template for communicating visual diffs to stakeholders.
