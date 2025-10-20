# Python pre-commit hooks

This python tool help you manage [precommit hooks](precommit.md) and works will managing them in a team.

```bash
pip install pre-commit
```

---

If you run into this in the install:

```bash
  WARNING: The script nodeenv is installed in '<redacted>/.local/bin' which is not on PATH.
  Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
  WARNING: The script identify-cli is installed in '<redacted>/.local/bin' which is not on PATH.
  Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
  WARNING: The script virtualenv is installed in '<redacted>/.local/bin' which is not on PATH.
  Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
  WARNING: The script pre-commit is installed in '<redacted>/.local/bin' which is not on PATH.
  Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
```

Then the next command may not work so you should update your `~/.bashrc` or `~/.zshrc`  with this:

```bash
export PATH="$HOME/.local/bin:$PATH"
```

In your terminal you may need to refresh it using `source ~/.bashrc` to get access to the updated PATH.

---
In your git repo run

```bash
pre-commit install
```
