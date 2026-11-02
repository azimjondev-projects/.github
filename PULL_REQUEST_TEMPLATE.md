## What changed

<!-- one or two lines -->

## Checklist

- [ ] Tests pass locally and in CI
- [ ] No secrets, client data or `.env` files in the diff
- [ ] Migrations are expand-only (no DROP / RENAME of columns in use)
- [ ] Append-only data (sales, payments, ledger) is never updated or deleted, fixes go through reversal entries
- [ ] Reports: golden tests updated, and every change in numbers is explained
- [ ] New feature is behind a flag if it is not ready for users
