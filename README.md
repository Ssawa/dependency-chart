# Depedency Chart
Graph a simple dependency graph based on a project's package.json and package-lock.json

# Example
List all dependencies for a project

```
$ ./deps /tmp/dependency-chart/

dependency-chart@1.0.0
├── archy@1.0.0
├─┬ argparse@1.0.10
│ └── sprintf-js@1.0.3
└── npm-logical-tree@1.2.1
```

Filter dependency chains to dependencies that match a regex

```
$ ./deps /tmp/dependency-chart/ -f sprintf

dependency-chart@1.0.0
└─┬ argparse@1.0.10
  └── sprintf-js@1.0.3
```
