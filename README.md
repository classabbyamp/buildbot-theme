## buildbot-void-theme

Buildbot plugin that changes some UI elements to match Void Linux's colour scheme, as well as makes some improvements to the functionality and accessibility of the web interface, including:

- reduce or remove some animations (and make them respect `prefers-reduced-motion: reduce`)
- improve discernability of build status colours
- respect `prefers-color-scheme: dark`

### Usage

1. Install the plugin, for example: `pip install buildbot-void-theme`

2. In your `buildmaster.cfg`, add:

```py
# in your buildmaster config object
c["www"]["plugins"] = {'void_view': {}, ...}
```
