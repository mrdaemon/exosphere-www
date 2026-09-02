+++
title = "install"
render = false

[extra]
# Install method boxes. It was, once more, easier to compose this here.
methods = [
  { label = "pipx", cmd = "pipx install exosphere-cli",    note = "If you already have Python 3.13 or later." },
  { label = "uv",   cmd = "uv tool install exosphere-cli", note = "Fetches and manages a Python runtime for you." },
]
+++

Or, see our detailed [installation guide]({{ config.extra.install_url }}). Then run `exosphere` and follow the
[quickstart guide →]({{ config.extra.quickstart_url }})
