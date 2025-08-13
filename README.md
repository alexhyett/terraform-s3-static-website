# alexhyett/terraform-s3-static-website

This repository has been moved to my [personal git instance](https://git.alexhyett.com/alexhyett/terraform-s3-static-website).

## Why?
GitHub hasn't quite been the same since being acquired by Microsoft in [2018](https://en.wikipedia.org/wiki/GitHub#Acquisition_by_Microsoft). I stuck with it for a while but as of [August 2025](https://www.theverge.com/news/757461/microsoft-github-thomas-dohmke-resignation-coreai-team-transition) GitHub is going to be part of Microsoft's CoreAI team.

Clearly GitHub is being viewed as a wealth of training data for the next AI rather than a platform for developers.

## How?
In case you also want to move a repository, here's how I moved this repository:

1. Create a new local and orphaned branch: `git checkout --orphan gone`
2. Delete all content: `git rm -r --cached . && git clean -df .`
3. Added this `README.md` with `git add -A`
4. Commit the changes: `git commit -m "Moved project"`
4. Delete the `main` branch: `git branch -D main`
5. Rename the current branch to `main`: `git branch -m main`
6. Force push to main: `git push -f origin main`

After that I archived the GitHub repository, effectively setting it to read-only and updated the description accordingly.

## Why not just deleting the repository?

This was a public repository. Deleting it from GitHub will cause the following to happen:

> When you delete a public repository, the oldest, active public fork is chosen to be the new upstream repository. All other repositories are forked off of this new upstream and subsequent pull requests go to this new upstream repository.

Source: [Deleting a public repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/what-happens-to-forks-when-a-repository-is-deleted-or-changes-visibility#deleting-a-public-repository)
