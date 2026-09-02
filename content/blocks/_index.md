+++
# Not actually a page. Entire "blocks" section exists solely to contain
# the landing page's content blocks, one per file.
#
# The blocks carry all of their content: title, extra metadata if any,
# and body text as markdown.
#
# Zola 0.23 apparently templates body with a new parser that can read and
# access config.toml values directly, instead of needing shortcodes, and
# we ABSOLUTELY use the shit out of this. Static, external URLs are all
# defined in config.toml, and the blocks reference them directly.
#
# Section is marked as render = false, since it's not a page.
# Zola will whine about orphans, but that is intended.
#
render = false
+++