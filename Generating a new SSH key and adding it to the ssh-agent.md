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


## 3 At the prompt, type a secure passphrase.
> Enter passphrase (empty for no passphrase): [Type a passphrase]
> 
> Enter same passphrase again: [Type passphrase again]


--


# Adding your SSH key to the ssh-agent
## 1 Start the ssh-agent in the background.
```sh
eval "$(ssh-agent -s)"
```
> Agent pid 59566

## 2 Add your SSH private key to the ssh-agent.
> If you created your key with a different name, or if you are adding an existing key that has a different name, replace id_ed25519 in the command with the name of your private key file.
```sh
ssh-add ~/.ssh/id_ed25519
```


## 3 Add the SSH public key to your account on GitHub. For more information
> see [Adding a new SSH key to your GitHub account](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account).


