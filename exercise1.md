Neural Networks is a field of research of great interest to me, and Python is by far the most commonly used language for that matter.

To manage **linting**, *Pylint* is the first result Google returns. It has some haters, though, as it is quite opinionated and returns messy warnings. *pycodestyle* is less opinionated and just detects against PEP 8 style conventions. For logic linters, *Bandit* is a security linter that detects common issues. 

For **testing**, *unittest* is the standard Python library. *Pytest* is a non-standard alternative that has simpler syntax. *Doctest* is interesting too, as it describes the tests inside the docs themselves.

For **building**, you can make a `pyproject.tomlp` that manages how `pip` and `build`, the main build tools, work. This creates a zipped customizable distribution with items such as `README.md`, `LICENSE`, ready for shipping.

About **CI/CD alternatives** to Jenkins and GitHub Actions , all I could find was *CircleCi* thrown around often. *Bitbucket Pipelines* is a service built into Bitbucket. GitLab has quite the name too and there is an open source branch, called *GitLab Community Edition*, you can host yourself.

This project would probably have to be self-hosted, as GPUs are a prime requirement for NNs and, although there are multiple ways to get cloud GPUs, there are other issues. I would feel more confident knowing only the team has a hold of the NNs and training data. Training data can, depending on the project, easily reach orders of magnitude of TBs. There are just too many issues on how badly it scales with cloud services to make big research, so I prefer to just go with self-hosting.
