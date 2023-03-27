# security-tool-box

Security Tool Box is a container image that it has been builded via apko and melange. It's useful while source code analysis because you can easly access a bunch of tool with single docker image. Also it is very useful in CI/CD process.

It contains following tools:
- **Development**
  - Git
  - Python 3.11
  - Pip3
- **Static Application Security Testing**
  - Semgrep
- **Container Security**
  - Grype
  - Trivy
- **Software Bill of Material**
  - Syft
- **IaC**
  - Checkov
