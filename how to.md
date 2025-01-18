======================================================================= Annotated Tags vs Lightweight Tags========================================

- **Annotated Tags**:
  - Contains metadata like the tagger's name, email, and the date it was created.
  - Stored as full objects in the Git database.
  - Can be signed with GPG to verify authenticity.
  - Example: `git tag -a v1.7 -m "Release version 1.7"`

- **Lightweight Tags**:
  - Simply a pointer to a specific commit, without additional metadata.
  - Stored as a simple reference in the Git database.
  - Faster to create but not as rich in information as annotated tags.
  - Example: `git tag v1.7`

======================================================================When to Use Git Rebase=========================================================

- **Rebase** is used to apply your changes on top of another branch, creating a clean, linear history.
- It is useful when you want to integrate the latest changes from `main` (or another branch) into your feature branch.
- Rebase helps in:
  - Keeping the commit history clean and linear.
  - Avoiding unnecessary merge commits.
  - Making collaboration easier by rebasing your changes onto the latest commits.

To rebase your branch onto `main`, use:

```bash
git rebase main



====================how to delete tags=========================

ex : git push origin --delete v2





list tags =>>> git tag



