+++
title = "supported remote platforms"
render = false

[extra]
# Icon names map to static/icons/<name>.svg
# Displayed by the template. It was easier to compose this here.
platforms = [
  { icon = "debian",  name = "Debian-likes",  detail = "apt" },
  { icon = "redhat",  name = "Red Hat-likes", detail = "yum / dnf" },
  { icon = "freebsd", name = "FreeBSD",       detail = "pkg" },
  { icon = "openbsd", name = "OpenBSD",       detail = "pkg_add" },
]
+++

…and their derivatives. Other POSIX systems get connectivity checks.
