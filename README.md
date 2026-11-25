# CamperSpot API

![Status](https://img.shields.io/badge/status-in%20development-orange)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)

## Overview

CamperSpot API is an open-source project designed to provide
access to geospatial information about motorhome stopovers,
parking areas, campsites and related facilities.

The project aims to provide a public REST API and an interactive
web application, initially focused on Italy, with the possibility
of expanding across Europe.

## Project Goals

- Provide an open and documented REST API.
- Build a reliable geospatial database.
- Collect and normalize data from open sources.
- Support location-based searches and filtering.
- Provide an interactive map-based web application.
- Enable third-party integrations.
- Maintain a modular and scalable architecture.
- Minimize initial development and infrastructure costs.

## Planned Features

- Search motorhome stopovers by location.
- Search within a specified geographic radius.
- Filter by price, facilities and parking restrictions.
- Retrieve detailed information about parking areas.
- Display parking areas on an interactive map.
- Import and normalize OpenStreetMap data.
- Allow users to report incorrect information.
- Allow users to suggest new locations.

## Technology Stack

| Component | Technology |
|---|---|
| Backend | Python, FastAPI |
| Database | PostgreSQL, PostGIS |
| ORM | SQLAlchemy, GeoAlchemy2 |
| Database migrations | Alembic |
| Frontend | React, TypeScript |
| Interactive maps | Leaflet |
| Geospatial data | OpenStreetMap |
| API documentation | OpenAPI, Swagger UI |
| Testing | Pytest |
| Containerization | Docker |
| Local orchestration | Docker Compose |
| CI/CD | GitHub Actions |

## Project Structure

```text
CamperSpot-API/
├── backend/
├── frontend/
├── docs/
│   └── decisions/
├── infra/
├── scripts/
│   └── ingestion/
├── .editorconfig
├── .env.example
├── .gitignore
├── CHANGELOG.md
├── LICENSE
└── README.md
```

## Documentation

- [Requirements](docs/requirements.md)
- [Architecture](docs/architecture.md)
- [Roadmap](docs/roadmap.md)
- [Architecture Decisions](docs/decisions/)
- [Changelog](CHANGELOG.md)

## Getting Started

Installation and development instructions will be added
as the project evolves.

## Data Sources and Attribution

The project plans to use OpenStreetMap and other compatible
open data sources.

OpenStreetMap data is available under the Open Database
License (ODbL).

© OpenStreetMap contributors.

https://www.openstreetmap.org/copyright

Additional data sources and their respective licenses
will be documented before integration.

## Contributing

Contributions, suggestions and issue reports are welcome.

Contribution guidelines will be added in a future release.

## License

The source code license is available in the LICENSE file.

External datasets are subject to their respective licenses.

## Project Status

CamperSpot API is currently in the initial development phase.

A public API and production deployment are not yet available.
