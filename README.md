# 📖 Guide: Conventional Commits

The repository provides a structured approach to implementing and adhering to the Conventional Commits specification in software development projects. This pattern emphasizes clear, consistent, and meaningful commit messages, which improve collaboration, versioning, and changelog generation.
⠀
⠀
## Why This Format?
Adopting a standardized format for commit messages:

✅ Enables automated changelog generation

✅ Simplifies change tracking and auditing

✅ Improves collaboration in team environments

✅ Integrates with modern DevOps toolchains

✅ Aligns with industry best practices

---
⠀
⠀
⠀
## 💡 Best Practice Checklist

✅ Use imperative mood ("Add feature" not "Added feature")

✅ Keep descriptions ≤50 characters

✅ Reference issues/PRs in footers

✅ Separate distinct changes into atomic commits

✅ Document breaking changes explicitly

✅ Maintain consistent terminology

> "Treat commit messages like you're explaining your changes to a future developer who will maintain your code." – _Industry Best Practice_

---
⠀
⠀
⠀
## Commit Structure
```text
<type>(<scope>): <short description>

[optional body]

[optional footer]
```
⠀
⠀
⠀
## Key Component


| Element          | Required | Description                                                                 |
|------------------|----------|-----------------------------------------------------------------------------|
| **Type**         | ✔️       | Change category (see valid types below)                                     |
| **Scope**        | ❌       | Affected component (e.g., `dashboard`, `payment-gateway`, `api/v2`)        |
| **Description**  | ✔️       | Concise imperative statement ("Update" not "Updated" or "Updating")        |
| **Body**         | ❌       | Context or implementation details                                          |
| **Footer**       | ❌       | References to issues, breaking changes, or co-authors                       |

⠀
⠀
⠀
## Valid Change Types


| **Type**   | **Use Case**                          |
|------------|---------------------------------------|
| feat       | New user-facing functionality        |
| fix        | Bug resolution                        |
| docs       | Documentation improvements            |
| style      | Code formatting (whitespace, syntax)  |
| refactor   | Code restructuring without behavior change |
| test       | Test suite modifications              |
| chore      | Dependency updates/maintenance tasks  |
| build      | Build system configuration            |
| ci         | CI/CD pipeline changes                |
| perf       | Performance optimizations             |
| revert     | Revert previous changes               |
| security   | Security-related patches              |

⠀
⠀
⠀

⠀
⠀
⠀
## Practical Examples

#### Feature implementation:
```git
feat(authentication): add multi-factor auth option
```
#### Bug fix with breaking change:
```git
fix(database)!: update schema validation
BREAKING CHANGE: Requires MySQL 8.0+
```
#### Documentation update:
```git
docs(api): clarify rate limiting policies
```
#### Performance optimization:
```git
perf(rendering): reduce bundle size by 20%
Issue: #456
```



## References

- https://www.conventionalcommits.org/
- https://seesparkbox.com/foundry/semantic_commit_messages
- http://karma-runner.github.io/1.0/dev/git-commit-msg.html 


## License

This repository is licensed. This means you are free to share and adapt this content for any purpose, even commercially, as long as you provide appropriate credit to the original author. For more details, please refer to the [LICENSE.md](https://github.com/fcardan/conventional-commits-pattern/blob/main/LICENSE.md) file.
