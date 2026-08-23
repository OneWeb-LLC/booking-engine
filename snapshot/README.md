# Booking Engine Snapshot

The Snapshot is the installable Salesflow configuration that implements the Booking Engine methodology for a service business.

The methodology remains universal. The Snapshot is versioned implementation.

## Component catalog

- [Manifest](manifest.yaml)
- [Native and Custom Fields](fields/README.md)
- [Workflows](workflows/README.md)
- [Pipelines](pipelines/README.md)
- [Calendars](calendars/README.md)
- [Phone and Routing](phone-and-routing/README.md)
- [Dispositions](dispositions/README.md)
- [Navigation](navigation/README.md)
- [Dashboards](dashboards/README.md)

## Status

The namespace and contracts are defined in v0.5.0. Concrete exported assets, identifiers, screenshots, and installation validation will be added when the Snapshot is built.

## Design rules

- Prefer native Salesflow objects before creating custom replacements.
- Custom fields must represent durable state or required workflow input.
- Every workflow must map to a methodology transition and named owner.
- Every component must have an installation, verification, upgrade, and rollback note.
- Client-specific values belong in configuration, not universal workflow logic.
