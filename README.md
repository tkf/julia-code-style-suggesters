# A setup for using JuliaFormatter, JuliaProjectFormatter, and reviewdog/action-suggester

## Notes

This Action exists mainly for a very selfish reason: simplifying managing workflows for my
projects.  So, I don't think I can respond to feature requests and pull requests.  If you
want to add some features, the best approach probably is to fork this repository or to
simply copy the steps in [`action.yml`](action.yml) into your workflow file.

(A secondary reason is to noting how to compose interesting Julia packages and GitHub
Actions.)

## Usage example

Create `.github/workflows/code-style.yml` with the following content:

```yaml
name: Code style

on:
  pull_request:

jobs:
  code-style:
    runs-on: ubuntu-latest
    steps:
      - uses: tkf/julia-code-style-suggesters@v1
```

## Links

* https://github.com/domluna/JuliaFormatter.jl
* https://github.com/tkf/JuliaProjectFormatter.jl
* https://github.com/reviewdog/action-suggester
