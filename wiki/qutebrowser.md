## Default Browser

Disabling cookies and other tracking feature and setting qutebrowser as the
default browser makes qutebrowser block direct access to your primary browser
with a lot of cookies. Kinda like Firefox Focus for desktop.

```
# ~/Library/Preferences/qutebrowser/autoconfig.yml
  content.cookies.accept:
    global: never
```

## Ergonomic

qutebrowser accomplish tasks with less keystrokes. Take paste URL from
clipboard for example, qutebrowser requires 2 keystrokes.

```
pp
```

While Firefox requires 4 keystrokes.

```
cmd-l cmd-v
```

Or with mouse 3 clicks

```
hover to location bar then right click then click paste and go
```

## Per-Site Settings

qutebrowser natively supports per site setting.

E.g. only send `accept-language: zh-tw` header to `zh.wikipedia.org`.

```
# ~/Library/Preferences/qutebrowser/autoconfig.yml
  content.headers.accept_language:
    zh.wikipedia.org: zh-TW
```

Or disable JavaScript globally by default and enable only on `qute://*` pages
and `search.brave.com`.

```
# ~/Library/Preferences/qutebrowser/autoconfig.yml
  content.javascript.enabled:
    global: false
    qute://*: true
    search.brave.com: true
```
