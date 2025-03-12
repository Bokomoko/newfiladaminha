# Development Environment with Dev Containers

Using Dev Containers offers several advantages:

1. **Consistency**: Ensures a consistent development environment across different machines.
2. **Isolation**: Isolates dependencies and tools, preventing conflicts.
3. **Portability**: Easily share and reproduce development environments.
4. **Scalability**: Simplifies scaling development environments for larger teams.
5. **Integration**: Seamlessly integrates with CI/CD pipelines for automated testing and deployment.

## Dockerfile

### Container Characteristics

- [ ] Minimal Linux distribution
- [ ] astral.sh UV package manager
- [ ] astral.sh ruff linter from astral.sh for linting Python code

### devcontainer.json Attributes

- [ ] Ensure extensions used in the current host configuration of the dev container

## Project Configuration

We will be using the UV Python package manager. Therefore, all information for dependency resolution, the Python version to be used, and tools will be contained in the `project.toml` file produced with the `uv init` command or a similar command.
