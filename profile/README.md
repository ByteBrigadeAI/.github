# ByteBrigadeAI

A reusable demo organization for GitHub and GitHub Copilot, built around
fictional applications with real issues, review PRs, and scanner findings.

| Application | Stack | Start here |
| --- | --- | --- |
| [AssetTrack](https://github.com/ByteBrigadeAI/assettrack) | .NET, Java, Python, Astro, React | [Issues](https://github.com/ByteBrigadeAI/assettrack/issues), [review PR](https://github.com/ByteBrigadeAI/assettrack/pull/9), [security](https://github.com/ByteBrigadeAI/assettrack/security) |
| [GameHub](https://github.com/ByteBrigadeAI/gamehub) | Astro, TypeScript, SQLite | [Issues](https://github.com/ByteBrigadeAI/gamehub/issues), [review PR](https://github.com/ByteBrigadeAI/gamehub/pull/10), [security](https://github.com/ByteBrigadeAI/gamehub/security) |

Each app has eight curated issue scenarios and an open fix PR. Security
examples include SQL injection, DOM XSS, and generated, never-issued
AWS-shaped patterns detected by secret scanning. Code quality uses optional
manual CodeQL reliability and maintainability scans, not the separately
billed GitHub Code Quality product.

## Prepare before presenting

1. Open either app's **Actions > Prepare demo assets > Run workflow**.
2. Select **demo-baseline** and leave the defaults for an idempotent refresh.
3. Select **scan_quality** only when you want a fresh security-and-quality scan.
4. Open the run summary for links to the prepared assets.

No scheduled or automatic push/PR workflows run. Existing review PRs are
reused. Actions-created replacement PRs require an owner to enable the
organization/repository permission and select **create_pull_requests**;
otherwise preparation reports a comparison link without a failing API call.

Follow the [15-minute walkthrough and reset instructions](https://github.com/ByteBrigadeAI/demo-hub).
Use synthetic data and isolated development environments; the intentionally
vulnerable samples are demo applications, not production services.
