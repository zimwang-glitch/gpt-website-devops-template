# Wang Lab Website Architecture

## Production architecture

```
GPT assistant
    |
    v
GitHub repository
zimwang-glitch/zimengwang-lab-site
    |
    v
GitHub Actions
    |
    v
Alibaba Cloud OSS
zimengwang-lab-site-prod-2026
    |
    v
www.zimengwang.org.cn
```

## Design principles

- GitHub is the single source of truth.
- Production deployment is automated.
- Domain configuration is separated from content management.
- Legacy websites are preserved as archives.

## Components

| Component | Responsibility |
|---|---|
| GPT | Website planning and modification interface |
| GitHub | Source control and history |
| GitHub Actions | Build and deployment automation |
| OSS | Production hosting |
| DNS | Domain resolution |
