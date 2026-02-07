# SynergyChat

Kubernetes deployment for a multi-service chat application with a web frontend, API backend, and crawler service.

## Deploy

```bash
kubectl create namespace crawler
kubectl apply -f .
```

## Services

- **Web**: Frontend at `synchat.internal` (auto-scales 1-4 pods)
- **API**: Backend at `synchatapi.internal` (persistent storage)
- **Crawler**: Content indexing service (3 containers, dedicated namespace)

## License

This project is part of the Boot.dev curriculum.
