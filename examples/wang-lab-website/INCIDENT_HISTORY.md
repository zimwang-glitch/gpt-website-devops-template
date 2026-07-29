# Wang Lab Website Incident History

## Incident 001 — Multiple production sources

### Symptom

GPT preview showed updates, but the public website did not consistently update.

### Root cause

Multiple possible production paths existed:

- ChatGPT Sites
- Multiple GitHub repositories
- Multiple OSS buckets
- Mixed DNS records

### Resolution

Unified architecture:

```
GPT
 |
GitHub
 |
GitHub Actions
 |
OSS production bucket
 |
Canonical domain
```

---

## Incident 002 — False deployment failure

### Symptom

GitHub Actions reported failure after deployment.

### Root cause

The OSS upload succeeded, but the final verification step failed because metadata checking was not aligned with deployment permissions.

### Resolution

Replace storage-level verification with public release verification.

---

## Lessons learned

- Keep one production source.
- Separate preview and production environments.
- Verify the public release, not only the upload process.
