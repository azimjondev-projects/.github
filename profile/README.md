# Azimjon Dev Projects

Custom software for businesses: POS and back-office systems, mobile apps, Telegram bots and web platforms.
Built and maintained by [Azimjon Abdurasulov](https://azimjondev.uz/).

**Stack:** Go · Flutter · Swift · Kotlin · TypeScript · PostgreSQL

Client repositories are private.

---

## Repository naming

Every repository is named **`<client>-<part>`**.
The shared prefix keeps all repositories of one client next to each other.

| Part      | What lives there                                                 |
| --------- | ---------------------------------------------------------------- |
| `-system` | Main product (monorepo): `backend/`, `app/`, `deploy/`, `tools/` |
| `-mobile` | Separate mobile app, only if it is not part of the `-system` app |
| `-bot`    | Separate bot, only if it uses a different stack or release cycle |
| `-web`    | Public website / landing page                                    |
| `-infra`  | Shared infrastructure, if it outgrows `deploy/`                  |

Rules:

1. `<client>` is lowercase latin, no spaces: `acme`, `greenshop`.
2. Start with one `-system` monorepo. Split a part out only when it has its own stack, team or release cycle.
3. Same stack + same API + same release = folder inside `-system`, not a new repo.
4. Repositories are **private** by default.
5. Topics: `client-<client>` plus the main tech (`go`, `flutter`, `swift`, `kotlin`, `typescript`).

Inside a repo:

- Branches: `main` is always deployable, work happens in `feature/<short-name>`.
- Commits: short, plain English, first person: `added courier report`, `fixed shift close`.
- Go module path = repo path: `github.com/azimjondev-projects/<client>-system/backend`.

## Contact

- Website: [azimjondev.uz](https://azimjondev.uz/)
- Email: azimjondevuz@gmail.com
- Telegram: [@azimjondevuz](https://t.me/azimjondevuz)
- LinkedIn: [Azimjon Abdurasulov](https://www.linkedin.com/in/azimjon-abdurasulov)
