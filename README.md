# LibreOffice to PDF conversion service

by [@Porantim](https://github.com/Porantim)

Lightweight Web API built in Go (Golang) designed to convert LibreOffice Writer documents into PDF files. The service encapsulates LibreOffice within a containerized environment and exposes a simple, well‑structured HTTP interface for seamless document conversion in automated workflows or server-side applications.
The project includes:

- A [Go-based Web API](main.go) responsible for receiving Writer documents, processing them through LibreOffice, and returning the resulting PDF.
- [Dockerfile](Dockerfile) and [docker-compose.yml](docker-compose.yml) for building and deploying the service in containerized environments.
- A Kubernetes [deployment.yaml](deployment.yaml) for cloud or cluster-based setups.
- Auxiliary script [entrypoint.sh](entrypoint.sh) to streamline startup the environment.
- A curl file [test.curl](test.curl) to test de service
- A complete [OpenAPI/Swagger specification](swagger.json), which documents all available endpoints, request payloads, and response formats.

This makes the service easy to integrate with other systems, providing a standardized and automated way to convert .odt or other Writer-supported formats into PDF files via REST API calls.
