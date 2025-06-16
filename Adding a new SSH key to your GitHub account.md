
# Adding a new SSH key to your GitHub account

### 1 Copy the SSH public key to your clipboard.
>
> If your SSH public key file has a different name than the example code, modify the filename to match your current setup. When copying your key, don't add any newlines or whitespace.

```sh
cat ~/.ssh/id_ed25519.pub
```

>  Then select and copy the contents of the id_ed25519.pub file displayed in the terminal to your clipboard

### 2 In the upper-right corner of any page on GitHub, click your profile photo, then click  **Settings.**

### 3 In the "Access" section of the sidebar, click  SSH and GPG keys.

### 4 Click New SSH key or Add SSH key.

### 5 In the "Title" field, add a descriptive label for the new key. For example, if you're using a personal laptop, you might call this key "Personal laptop".

### 6 Select the type of key, either authentication or signing. For more information about commit signing, see About commit signature verification.

### 7 In the "Key" field, paste your public key.

### 8 Click Add SSH key.

### 9 If prompted, confirm access to your account on GitHub. For more information, see Sudo mode.
