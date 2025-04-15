# Elasticsearch Cluster on Docker Swarm

This project deploys a production-grade Elasticsearch cluster using Docker Swarm, with Traefik for routing.

## 🐳 Services

- 3 Master Nodes: `es01`, `es02`, `es03`
- 6 Data Nodes: `es04` to `es09`
- Traefik is used as a reverse proxy to expose Elasticsearch over a path prefix.

## 📦 Requirements

- Docker Swarm initialized
- Docker node labels set (e.g., `role=manager`, `role=worker1`, `role=worker2`)
- Traefik running in Swarm mode

## 🚀 Deploy

```bash
docker stack deploy -c stack.yml elastic
```

## 💖 Support the Project
This project took a lot of time, effort, and coffee to get just right. If you've found this project helpful or if it’s made your life a bit easier, consider supporting me! Every donation helps me keep improving it and gives me more reasons to keep coding (and refilling my coffee cup!).

Your support would mean the world to me! Thank you for helping me continue working on amazing projects like this. 🙌💻

<noscript><a href="https://liberapay.com/swarmhunter/donate"><img alt="Donate using Liberapay" src="https://liberapay.com/assets/widgets/donate.svg"></a></noscript>