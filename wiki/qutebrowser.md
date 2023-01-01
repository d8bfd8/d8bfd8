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
