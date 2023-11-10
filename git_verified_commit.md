# Git Verified Commit

```

gpg --list-secret-keys --keyid-format=long

gpg --full-generate-key
gpg --list-secret-keys --keyid-format=long


git config --global user.signingkey 0AF1928AA8601AAE
git config --global commit.pgpsign true
git log --show-signature -1


gpg --armor --export 0AF1928AA8601AAE 
gpg --export --armor 0AF1928AA8601AAE > ./gpg-key.pub
gpg --export-secret-keys --armor 2F2E4E774B8FDEDFCEF149890AF1928AA8601AAE > ./gpg-key.asc

```

Signing verification
no sign verification