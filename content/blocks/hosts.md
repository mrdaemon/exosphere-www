+++
title = "runs on"
render = false

[extra]
# Icon names map to static/icons/<name>.svg
# Displayed by the template, for platforms where Exosphere runs.
# Did I mention it was easier to compose this here? It was.
#
# Windows and macOS get homebrew stand-ins rather than their real logos.
# I am in no mood to deal with lawyers lol.
platforms = [
  { icon = "window",  name = "Windows" },
  { icon = "linux",   name = "Linux" },
  { icon = "command", name = "macOS" },
  { icon = "freebsd", name = "FreeBSD" },
  { icon = "openbsd", name = "OpenBSD" },
  { icon = "netbsd",  name = "NetBSD" },
]
+++

…and anywhere else Python 3.13 or above runs.
