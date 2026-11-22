## ADDED Requirements

### Requirement: PostgreSQL validation and Helm client version

The PostgreSQL integration jobs and Helm database setup and migration jobs SHALL use PostgreSQL 18 images.

#### Scenario: CI verifies PostgreSQL compatibility

- **WHEN** CI runs a PostgreSQL integration job
- **THEN** the job starts PostgreSQL 18

#### Scenario: Helm runs a database job

- **WHEN** Helm renders a database setup or migration job
- **THEN** the job uses a PostgreSQL 18 client image
