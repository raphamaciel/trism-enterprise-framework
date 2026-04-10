# Branch Protection Setup (GitHub)

Use this guide to enforce TRiSM pull request controls on the `main` branch.

## Recommended Rules

- Protect `main` branch.
- Require pull request before merging.
- Require at least 2 approvals.
- Require review from Code Owners.
- Dismiss stale approvals when new commits are pushed.
- Require conversation resolution before merge.
- Require status checks to pass before merge.
- Restrict force pushes and branch deletion.

## Suggested Required Status Checks

- `TRiSM Governance Checklist`
- `Risk Register Linked`
- `Gate Checklist Complete`

## GitHub UI Path

1. Open repository Settings.
2. Go to Branches.
3. Add a branch protection rule for `main`.
4. Enable recommended rules above.
5. Save changes.

## Optional GitHub CLI Example

Run from repository root after `gh auth login`:

```powershell
gh api \
  --method PUT \
  -H "Accept: application/vnd.github+json" \
  /repos/<OWNER>/<REPO>/branches/main/protection \
  -f required_status_checks.strict=true \
  -f required_pull_request_reviews.dismiss_stale_reviews=true \
  -f required_pull_request_reviews.require_code_owner_reviews=true \
  -f required_pull_request_reviews.required_approving_review_count=2 \
  -f enforce_admins=true \
  -f restrictions=
```

Replace `<OWNER>` and `<REPO>` with your GitHub organization and repository name.
