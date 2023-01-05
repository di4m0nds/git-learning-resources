# Configure your local SSH keys

1. First go home in your terminal
2. Then execute next command to generate your SHH keys
```bash
ssh-keygen -t rsa -b 4096 -C "example@email.com"
```
3. Put up your "server" of SHH keys of your computer (windows & linux)
```bash
eval $(ssh-agent -s)

# or mac

eval "$(ssh-agent -s)"
```
4. Create (if not exists) a config file into "~/.ssh/", and add your SHH key to the "server", 
```bash
# -----------------------------------
# Create config file into "~/.ssh/" like "~/.ssh/config" and add the content below 
# Host alias
#     HostName hostname
#     User <some-name>
# -----------------------------------

ssh-add <path-of-your-priv-key>
```
or mac
```bash
# -----------------------------------
# Create config file into "~/.ssh/" like "~/.ssh/config" and add the content below 
# Host *
#   AddKeysToAgent yes
#   UseKeychain yes
#   IdentityFile <path-of-your-priv-key>
# -----------------------------------

ssh-add -K <path-of-your-priv-key>
```
Read more about SSH config files: https://linux.die.net/man/5/ssh_config