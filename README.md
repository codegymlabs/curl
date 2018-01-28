# Dockerized curl executable

Based on Alpine Linux.

Usage
---

```bash
docker run --rm codegymlabs/curl [args]
```

Sample:

```bash
docker run --rm codegymlabs/curl -fsSL https://curl.haxx.se/
```

Alias
---

Add this funtion into autoload script (`.profile`, `.bashrc`, etc):

```bash
curl () {
    (docker run -it --rm codegymlabs/curl "$@")
}
```

Curl's manpage: [https://curl.haxx.se/docs/manpage.html](https://curl.haxx.se/docs/manpage.html)