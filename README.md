# A repo for delivering binary files

```text
ALGO: SHA256
SALT: b0a459545b5d737f62f47574766ca5096726d80cc78955e6ea613a736aff67fd
```

```python
def run_sha_256(url: str, content: bytes) -> str:
    sha = hashlib.sha256(SALT.encode())
    sha.update(url.encode())
    sha.update(content)
    return sha.hexdigest()
```
