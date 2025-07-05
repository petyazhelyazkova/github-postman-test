# GitHub API Collection with Postman

This project demonstrates how to use GitHub's REST API via Postman for:

- Authentication
- Creating repositories
- Creating and commenting on issues
- Closing issues
- Deleting repositories

It also supports CLI execution using Newman.

---

## 🧰 Requirements

- [Node.js and npm](https://nodejs.org/)
- [Postman](https://www.postman.com/downloads/)
- GitHub Personal Access Token with `repo` scope

---

## 🚀 Getting Started

1. Clone or download this repository
2. Open Postman and import:
   - `github-postman-collection.json`
   - `github-environment.json`

3. In Postman:
   - Go to ⚙️ **Manage Environments**
   - Select the `GitHub Environment`
   - **Fill in your own GitHub credentials**:

| Variable | Value |
|----------|-------|
| `token`  | your GitHub Personal Access Token |
| `username` | your GitHub username |

4. Save the environment and select it from the top-right dropdown

## ▶️ Run the collection via CLI

```bash
newman run github-postman-collection.json -e github-environment.json
