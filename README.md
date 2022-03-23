# A setup for using JuliaFormatter, JuliaProjectFormatter, and reviewdog/action-suggester

Usage example:

```yaml
# .github/workflows/code-style.yml
name: Code style

on:
  pull_request:

jobs:
  code-style:
    runs-on: ubuntu-latest
    steps:
      - uses: tkf/julia-code-style-suggesters@v1
```

Links:

* https://github.com/domluna/JuliaFormatter.jl
* https://github.com/tkf/JuliaProjectFormatter.jl
* https://github.com/reviewdog/action-suggester
