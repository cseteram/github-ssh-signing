# github-ssh-signing

1. Generate a new SSH key.
   ```
   ssh-keygen -t ed25519 -c "your_comment"
   ```

2. Configure Git.
   ```bash
   git config gpg.format ssh
   git config user.signingKey "~/.ssh/id_ed25519.pub"
   git config commit.gpgsign true
   ```

3. Add the SSH public key to GitHub.  
   You should select the key type as *Signing Key*.
   ```
   cat ~/.ssh/id_ed25519.pub
   # GitHub > Settings > SSH and GPG keys > New SSH key
   ```
