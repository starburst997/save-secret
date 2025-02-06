# save-secret

GitHub Action that takes secret value and saves it in the repository secrets.

## Usage

```yaml
uses: starburst997/save-secret@v1
with:
  # Your Personal Access Token (PAT) that has repo permissions 
  github_token: ${{ secrets.GH_PAT }}
  secret_name: YOUR_SECRET_NAME
  secret_value: "path/to/secret.txt"
```

The secret value is a path to a file since we don't want to leak those in the log!