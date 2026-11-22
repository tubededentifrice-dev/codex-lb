## Why

Use PostgreSQL 18 in CI and the Helm database jobs to match the bundled database and Docker Compose.

## What Changes

- Run PostgreSQL integration tests against major version 18.
- Use the PostgreSQL 18 client for database setup and migrations in Helm.
- Preserve the documented migration from existing PostgreSQL 16 Compose volumes.

## Impact

- Affected specs: deployment-installation
- Affected code: CI workflow and Helm database jobs
