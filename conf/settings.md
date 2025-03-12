# SETTINGS Documentation

- `"debug": false`: only to development
- `"contact":None`: `"contact": [{"name": "Full name","e_mail": ["email@example.com"],"phones": ["+55 31 99999-1234"]}],`
- `"tr_url":None`: Regular expression to translate URLs before check permition
- `"time_zone": "America/Chicago"`: Local time zone <https://en.wikipedia.org/wiki/List_of_tz_zones_by_name>
- `"tz": true`: timezone
- `"language": "pt_br"`: Language of system <http://www.i18nguy.com/unicode/language-identifiers.html>
- `"cookie":{"name": "project","age": null,"domain": null,"path": "/","secure": false,"httponly": false,"samesite": null,}`: cookie settings
- `"charset": "utf-8"`: default charset to use
- `"email": {}`: email config
- formats: <https://docs.djangoproject.com/en/dev/ref/templates/builtins/#date> <https://docs.python.org/library/datetime.html#strftime-behavior>

- Cache to store session data if using the cache session backend

SESSION_CACHE_ALIAS = "default"

- Cookie name. This can be whatever you want

SESSION_COOKIE_NAME = "sessionid"

- Age of cookie, in seconds (default: 2 weeks)

SESSION_COOKIE_AGE = 60 *60* 24 *7* 2

- A string like "example.com", or null for standard domain cookie

SESSION_COOKIE_DOMAIN = null

- Whether the session cookie should be secure (https:// only)

SESSION_COOKIE_SECURE = false

- The path of the session cookie

SESSION_COOKIE_PATH = "/"

- Whether to use the HttpOnly flag

SESSION_COOKIE_HTTPONLY = True

- Whether to set the flag restricting cookie leaks on cross-site requests

- This can be "Lax", "Strict", "null", or false to disable the flag

SESSION_COOKIE_SAMESITE = "Lax"

- Whether to save the session data on every request

SESSION_SAVE_EVERY_REQUEST = false

- Whether a user"s session cookie expires when the web browser is closed

SESSION_EXPIRE_AT_BROWSER_CLOSE = false

- The module to store session data

SESSION_ENGINE = "django.contrib.sessions.backends.db"

- Directory to store session files if using the file session module. If null

- the backend will use a sensible default

SESSION_FILE_PATH = null

- class to serialize session data

SESSION_SERIALIZER = "django.contrib.sessions.serializers.JSONSerializer"

SECURE_CONTENT_TYPE_NOSNIFF = True
SECURE_CROSS_ORIGIN_OPENER_POLICY = "same-origin"
SECURE_HSTS_INCLUDE_SUBDOMAINS = false
SECURE_HSTS_PRELOAD = false
SECURE_HSTS_SECONDS = 0
SECURE_REDIRECT_EXEMPT = []
SECURE_REFERRER_POLICY = "same-origin"
SECURE_SSL_HOST = null
SECURE_SSL_REDIRECT = false
