# Profile README secrets

## `STATS_PAT` (required for full private totals)

1. Open https://github.com/settings/tokens
2. **Generate new token (classic)**
3. Scopes:
   - `repo` (full control of private repositories)
   - `read:user`
   - `user:email` (recommended — needed to attribute private commits correctly)
4. Copy the token (you will only see it once)
5. Add it as a repository secret:

```bash
gh secret set STATS_PAT --repo Abdelrahmanessam1254/Abdelrahmanessam1254
```

Or: Repo → **Settings** → **Secrets and variables** → **Actions** → **New repository secret**  
Name: `STATS_PAT` · Value: *(paste token)*

6. Run the workflow: **Actions** → **Update Profile Stats** → **Run workflow**

Never commit the token to git or paste it into chat.
