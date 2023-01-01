## Default Browser

Disabling cookies and other tracking feature and setting qutebrowser as the
default browser makes qutebrowser block direct access to your primary browser
with a lot of cookies. Kinda like Firefox Focus for desktop.

```
# ~/Library/Preferences/qutebrowser/autoconfig.yml
  content.cookies.accept:
    global: never
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
