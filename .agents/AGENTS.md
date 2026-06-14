# Opencode Project Context

Before scanning the whole repository, use the existing project knowledge graph.

Required startup workflow:

1. Read `AGENTS.md`.
2. Read `graphify-out/AI_GRAPH_GUIDE.md`.
3. Query `graphify-out/graph.json` before scanning the whole repo.
4. Use `graphify-out/GRAPH_REPORT.md` for the project map and core hubs.

Useful graph commands:

```bash
graphify query "what are the core abstractions" --graph graphify-out/graph.json
graphify query "what connects the data layer to the api" --graph graphify-out/graph.json
graphify explain "package:flutter_grocery/helper/route_helper.dart" --graph graphify-out/graph.json
```

Refresh the graph after meaningful code changes:

```bash
graphify update .