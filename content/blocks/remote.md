+++
title = "supported remote platforms"
render = false

[extra]
# Icon names map to static/icons/<name>.svg
# Displayed by the template. It was easier to compose this here.
# Red Hat gets a stand-in because their licensing is uptight.
# No one likes having lawyers in their lives.
platforms = [
  { icon = "debian",  name = "Debian-likes",  detail = "apt" },
  { icon = "package", name = "Red Hat-likes", detail = "yum / dnf" },
  { icon = "freebsd", name = "FreeBSD",       detail = "pkg" },
  { icon = "openbsd", name = "OpenBSD",       detail = "pkg_add" },
]
+++

...and their derivatives. Other POSIX systems get connectivity checks.
