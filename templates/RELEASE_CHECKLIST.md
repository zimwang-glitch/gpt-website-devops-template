# Production Release Checklist

## Before deployment

- [ ] Change request reviewed
- [ ] Source repository confirmed
- [ ] Build succeeds
- [ ] Critical pages checked

## Deployment

- [ ] Git commit created
- [ ] CI/CD workflow completed
- [ ] Cloud deployment completed

## Verification

- [ ] Public URL accessible
- [ ] HTTPS valid
- [ ] Release version matches commit
- [ ] Mobile layout checked

## Rollback

If problems occur:

1. Identify last stable commit
2. Deploy previous version
3. Verify public release
4. Record incident
