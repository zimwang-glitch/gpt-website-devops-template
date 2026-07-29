# Domain Management Principles

## Single production path

One public domain should map to one production deployment source.

Recommended architecture:

User
↓
DNS
↓
CDN / edge layer
↓
Cloud hosting
↓
Website files

## Avoid multiple production controllers

Do not simultaneously use multiple systems as production sources for the same domain:

- GitHub Pages
- ChatGPT Sites
- OSS static hosting
- third-party builders

## Domain checklist

Before changing DNS:

- identify current production source
- confirm target hosting
- check SSL certificate
- verify redirects
- verify DNS propagation

## Rollback principle

Never delete old infrastructure immediately. Keep previous versions available until the new production path is verified.
