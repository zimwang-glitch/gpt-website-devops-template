# Deployment Guide

## Target architecture

GPT assistant
↓
GitHub repository
↓
CI/CD pipeline
↓
Cloud hosting
↓
Public website

## Deployment requirements

A production deployment should include:

1. Build validation
2. Static/runtime checks
3. Deployment
4. Public URL verification

## Failure diagnosis order

When local preview and public website differ:

1. Check GitHub commit
2. Check workflow status
3. Check deployment target
4. Check DNS records
5. Check CDN cache

## Release record

Each release should record:

- change summary
- commit ID
- deployment time
- verification result
