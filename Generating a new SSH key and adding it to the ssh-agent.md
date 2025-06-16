# Generating a new SSH key and adding it to the ssh-agent


## 1 Open Terminal.

## 2 Paste the text below, replacing the email used in the example with your GitHub email address.
```sh
ssh-keygen -t ed25519 -C "shikomatlala@gmail.com"
```
> This creates a new SSH key, using the provided email as a label.

> Generating public/private ALGORITHM key pair.
> 
> When you're prompted to "Enter a file in which to save the key", you can press Enter to accept the default file location. Please note that if you created SSH keys previously, ssh-keygen may ask you to rewrite another key, in which case we recommend creating a custom-named SSH key. To do so, type the default file location and replace id_ALGORITHM with your custom key name.
