# github-ssh-signing

```bash
git config gpg.format ssh
git config user.signingKey "~/.ssh/id_ed25519.pub"
git config commit.gpgsign true
```

```bash
git show --show-signature
```
