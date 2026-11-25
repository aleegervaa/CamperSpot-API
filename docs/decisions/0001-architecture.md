# ADR-0001: Adopt a Modular Monolith and Monorepo

## Status

Accepted

## Context

CamperSpot API is an open-source project that requires
a backend API, a geospatial database, a web application
and a data ingestion pipeline.

The initial development team consists of a single developer.

The architecture must prioritize maintainability,
simplicity, low infrastructure costs and future scalability.

## Alternatives Considered

### Option 1: Unstructured Monolith

A single application without clear module boundaries.

Advantages:

- Fast initial development.
- Minimal initial configuration.

Disadvantages:

- Reduced maintainability.
- Increased coupling.
- Difficult long-term testing.

### Option 2: Modular Monolith

A single backend application organized into modules
with clearly defined responsibilities.

Advantages:

- Clear separation of concerns.
- Simplified deployment.
- Lower infrastructure complexity.
- Improved testability.

Disadvantages:

- Requires architectural discipline.
- Modules share the same deployment lifecycle.

### Option 3: Microservices

Multiple independently deployed backend services.

Advantages:

- Independent service deployment.
- Independent service scaling.

Disadvantages:

- Increased operational complexity.
- Distributed communication overhead.
- Higher infrastructure requirements.

## Decision

CamperSpot API will adopt a modular monolith architecture.

The backend, frontend, infrastructure, scripts and
documentation will be maintained in a single Git repository.

## Consequences

- Initial development and deployment remain simple.
- Components must maintain clearly defined responsibilities.
- Independent services may be introduced in the future
  if justified by measurable requirements.
- Architectural changes must be documented through ADRs.
