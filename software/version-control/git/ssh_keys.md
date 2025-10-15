# Version Control - git SSH

You can use SSH keys to authenticate your dev machine with your git accounts on websites like GitHub. They enable cloning with an SSH link for example.

## Windows

- Open Powershell
- Use command for generating keys
- Find and copy your public key
- Upload it to your account's SSH keys

### Generate Key

First enter:

```bash
ssh-keygen
```

Hit enter unless you know what you are doing and want it stored elsewhere.

```bash
ssh-keygen
Generating public/private ed25519 key pair.
Enter file in which to save the key <YOU WILL SEE YOUR DEFAULT DIRECTORY HERE>:
Enter passphrase (empty for no passphrase):
```

Next enter no password and confirm the no password

```bash
ssh-keygen
Generating public/private ed25519 key pair.
Enter file in which to save the key <YOU WILL SEE YOUR DEFAULT DIRECTORY HERE>:
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in <unique to your system>
Your public key has been saved in <location_of_public_key>.ssh/id_ed25519.pub
The key fingerprint is: <unique to you>
SHA256: <unique to you>
The key's randomart image is:
+--[ED25519 256]--+
<unique to you>
+----[SHA256]-----
```

### Copy your key

In the same shell type:

```bash
    Get-Content  <location_of_public_key>.ssh/id_ed25519.pub
```

Your content will be shown. For obvious reasons the real keys wont be shown below so use some common sense.

```bash
ssh-ed25519 <key> <some identifier>
```

copy from your output starting at "ssh-ed25519" and ending the end of the `<key>`.

### Upload your key

There wont be screenshots or step by step as this can vary per website and across updates. If you need a step by step here is a video from YouTube but no gaurantees it is current or even availabe.

[Video describing the Process](https://www.youtube.com/watch?v=IS2VBS9NSYc)

## TODO Linux based OSs
