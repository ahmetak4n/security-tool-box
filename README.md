# security-tool-box

Security Tool Box is a container image that it contains a bunch of security tools. We are providing two different images.
STB RED for red teamss and STB GREEN for devsecops teams.

# stb red 
It is useful for security testing. Small and easy to use. You just need docker to use. It contains following tools:
- **development**
  - Git
  - Pip3
  - Python 3.11
- **sast**
  - semgrep
- **iac**
  - checkov
- **sbom**
  - Syft
- **k8s & container security**
  - Grype
  - Trivy
- **reconnaissance**
  - Nmap
  - Amass
  - Nuclei
  - ExploitDB
  - Gobuster
- **credential access**
  - jwt-tool
- **exfiltration**
  - sqlmap 

## usage
```bash
docker pull ghcr.io/ahmetak4n/security-tool-box:stb-red-$TAG
```
```bash
docker run --privileged --network=host --rm -it -v "${PWD}:${PWD}" -w "${PWD}" ghcr.io/ahmetak4n/security-tool-box:stb-red /bin/bash
```
> :exclamation: `--privileged` flag is required for nmap

> :exclamation: `--network=host` flag is required for scan any address in local

# stb green 
It is a sub set of STB RED, but it more small and focused application security. You can find bunch of tool that useful for DevSecOps. It contains following tools:
- **development**
  - Git
  - Pip3
  - Python 3.11
- **sast**
  - semgrep
- **iac**
  - checkov
- **sbom**
  - Syft
- **k8s & container security**
  - Grype
  - Trivy

## usage
```bash
docker pull ghcr.io/ahmetak4n/security-tool-box:stb-green-$TAG
```
```bash
docker run --rm -it -v "${PWD}:${PWD}" -w "${PWD}" ghcr.io/ahmetak4n/security-tool-box:stb-green /bin/bash
```
