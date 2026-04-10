# workflows

reusable workflows

*How to use in node project*

```yaml
name: Node Build Process

on:
  push:
    branches:
      - "*"
  pull_request:
    branches:
      - "*"

jobs:    

  ci:
    uses: yadickson/workflows/.github/workflows/integration.yml@v1
    with:
      container-image: node:22-slim
    secrets: inherit
```
*How to use in python project*

```yaml
name: Python Build Process

on:
  push:
    branches:
      - "*"
  pull_request:
    branches:
      - "*"

jobs:    

  ci:
    uses: yadickson/workflows/.github/workflows/integration.yml@v1
    with:
      container-image: python:3.12-slim
    secrets: inherit
```

*How to use in csharp project*

```yaml
name: CSharp Build Process

on:
  push:
    branches:
      - "*"
  pull_request:
    branches:
      - "*"

jobs:    

  ci:
    uses: yadickson/workflows/.github/workflows/integration.yml@v1
    with:
      container-image: mcr.microsoft.com/dotnet/sdk:8.0
    secrets: inherit
```

*How to use in maven project*

```yaml
name: Maven Build Process

on:
  push:
    branches:
      - "*"
  pull_request:
    branches:
      - "*"

jobs:    

  ci:
    uses: yadickson/workflows/.github/workflows/integration.yml@v1
    with:
      container-image: maven:3.6.3-openjdk-8-slim
    secrets: inherit
```