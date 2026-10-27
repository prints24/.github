# Contributing to Super91 Engineering

Welcome to the Super91 engineering team! We build high-throughput print commerce, automated prepress pipelines, and distributed logistics infrastructure.

This guide outlines our development workflow, coding standards, branching strategy, and pull request procedures.

---

## 🚀 Getting Started

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/prints24/<repo-name>.git
   cd <repo-name>
   ```
2. **Install Dependencies:**
   ```bash
   npm install
   ```
3. **Environment Setup:**
   * Copy `.env.example` to `.env` (never commit `.env` or production credentials).
   * Ensure local database and caching connections match your active development profile.

---

## 🌿 Git Branching Strategy

To keep releases predictable and clean across our production hubs and customer storefronts, we use structured branches:

| Branch | Purpose | Deployment Target |
|---|---|---|
| `main` | Production-ready, stable codebase | Production (`super91.com`) |
| `v1.1` / `staging` | Staging, regression testing, and integration verification | Staging environment |
| `feat/<issue#>-<short-description>` | New feature development | Local / Preview |
| `fix/<issue#>-<short-description>` | Bug fixes and patches | Local / Preview |
| `hotfix/<issue#>-<short-description>` | Urgent production incident fixes | Hotfix Staging ➔ `main` |

### Branch Naming Examples:
* `feat/466-dcp-single-user-lock`
* `fix/465-sequence-break-warning-modal`
* `hotfix/470-delivery-otp-sms-retry`

---

## 📝 Commit Conventions

We strictly follow the [Conventional Commits](https://www.conventionalcommits.org/) specification. This keeps Git history readable and automates changelog generation.

### Format:
```
<type>(<scope>): <short description in present tense>

[optional body with background context and ticket reference]

[optional footer: Fixes #466]
```

### Allowed Types:
* `feat`: A new user-facing or platform feature
* `fix`: A bug fix
* `refactor`: Code change that neither fixes a bug nor adds a feature
* `perf`: Performance improvement (e.g. database indexing, query optimization)
* `docs`: Documentation updates (README, API docs, comments)
* `chore`: Build process, dependencies, tooling, or CI updates
* `test`: Adding or updating unit/integration tests

### Examples:
* `feat(prepress): add single-user lock guard on DCP claim`
* `fix(logistics): clear continuous barcode scanner buffer on cancel`
* `perf(orders): add compound index on customerId and createdAt`

---

## 🔄 Development & Pull Request (PR) Workflow

1. **Pick or Create an Issue:**
   * All work must be tied to an open issue on the [SUPER91 Web V1 - Launch Track](https://github.com/orgs/prints24/projects/2) project board.
   * Assign yourself to the issue and move its status to `In progress`.

2. **Develop on a Feature Branch:**
   ```bash
   git checkout main
   git pull origin main
   git checkout -b feat/466-dcp-single-user-lock
   ```

3. **Verify Locally:**
   * Run linter: `npm run lint`
   * Run tests: `npm test`
   * Test user flows thoroughly (storefront PDP, prepress queue, franchise dashboard).

4. **Submit a Pull Request:**
   * Push your branch to GitHub: `git push -u origin feat/...`
   * Open a PR targeting `main` (or `v1.1`).
   * Complete the [Pull Request Template](.github/PULL_REQUEST_TEMPLATE.md):
     * Reference the issue (`Fixes #466`).
     * Attach screenshots or screen recordings for UI changes.
     * Document testing steps and verification evidence.

5. **Code Review:**
   * Request review from team members (`@prints24/engineering` or `@prints24/leads`).
   * Address review comments thoughtfully.
   * Once approved and verified, merge via **Squash and Merge** or **Rebase and Merge** to maintain a linear, clean history.

---

## 🛡️ Definition of Done (DoD)

Before any PR is approved for merge, it must satisfy:
- [ ] Code follows project formatting and linting rules without errors or warnings.
- [ ] No hardcoded secrets, API keys, or private environment variables are committed.
- [ ] Error handling and edge cases (e.g. network drop, empty state, concurrent clicks) are addressed.
- [ ] Database operations are guarded against race conditions where concurrent access occurs.
- [ ] Backward compatibility with existing order schemas and active jobsheets is preserved.
- [ ] Tested successfully on local development and staging environments.

---

## 💬 Questions & Support

Need guidance or blocked on an architecture decision?
* Post in internal engineering channels or open a discussion issue.
* Reach out to `@prints24/leads` or email [support@super91.com](mailto:support@super91.com).
