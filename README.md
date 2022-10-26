# GitLeaks Bug

You just have to install `pre-commit` and try to commit, even if the `gitleaks.toml` file exists it will not ignore the `some.key` file and will fail.

`pip install pre-commit==2.20.0`

`pre-commit install`

`git commit -m "something"`

This first commit was created using the `SKIP=gitleaks` environment variable, so it will not fail.
