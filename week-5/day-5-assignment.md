**Goal:** Practice the week’s skills by reading from the GitHub API and showing useful output.

## Steps

1. Create `index.html` and `script.js`. Fetch your GitHub user info from `https://api.github.com/users/<your-username>` and log:
   - Username
   - Public repo count
   - Profile URL
2. Fetch `https://api.github.com/users/<your-username>/repos` and render the names of the first five repositories on the page using `textContent`.
3. Optional (challenge): Create a repo via `POST https://api.github.com/user/repos` using a personal access token (read docs carefully). **Do not** commit the token to a github repo.
4. Keep code small and readable; handle network/HTTP errors gracefully; commit after each feature (ACP).

**Deliverable:** Public repo `w5-d5-github-api` with your code and a short `README.md` (how to run, what you built).

## Rubric (20 pts)

- **GET Request** (0–4): User info fetch works; correct fields shown.
- **List Repos** (0–4): Repo list shows up (first five) with safe rendering.
- **Error Handling** (0–4): Clear message for network/HTTP problems.
- **Clarity & Organization** (0–4): Small functions; readable code; tidy repo.
- **ACP Workflow** (0–4): Meaningful commits as you add features.
