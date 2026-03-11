# ProjectSetup

A ready-to-use template for quickly starting new .NET web API projects with essential tools pre-configured.

## Purpose

This template eliminates boilerplate setup work by providing a clean project structure with development tools, logging, API documentation, and Docker support already configured. Start building your application logic immediately without spending time on repetitive configuration.

## What's Included

- **Serilog** — structured logging with easy configuration
- **Swagger UI** — interactive API documentation for development
- **Docker Compose** — containerized deployment ready out of the box
- **Resilience patterns** — built-in retry and fault-handling capabilities
- **Code quality tools** — static analysis to maintain clean code
- **Centralized package management** — consistent dependency versions across all projects

## Configuration Files

### `.editorconfig`
Pre-configured coding conventions and style rules for consistent codebase:
- Naming conventions (PascalCase for types, `I` prefix for interfaces)
- Code style preferences (expression-bodied members, pattern matching, null-checks)
- Formatting rules (indentation, spacing, newlines)
- Enforced as errors to maintain code quality

### `Directory.Build.props`
Shared build properties applied to all projects automatically:
- Nullable reference types enabled
- Implicit usings enabled
- Strict code analysis with SonarAnalyzer

### `Directory.Packages.props`
Central Package Management — all NuGet versions defined in one place for easy updates and no version conflicts.

## Docker Support

Ready-to-use Docker configuration:
- **`Dockerfile`** — optimized container build for the API
- **`docker-compose.yml`** — orchestrate multi-container deployments
- **`.dockerignore`** — excludes unnecessary files from build context

Run with Docker:
```bash
docker-compose up --build
```

## Quick Start

```bash
dotnet run --project Web.Api
```

Swagger UI: `https://localhost:5001/swagger` (development mode)
