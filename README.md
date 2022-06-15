# Config SSH Mac 

Save keys on ssh config file to don't have to add the key at the moment of access to something by SSH (ssh-add /path/of/the/key):

```bash
# Create a config file:
$ vim $ /User/user_folder/.ssh/config
```

```bash
# And write this:
 Host *
   UseKeychain yes
   AddKeysToAgent yes
   IdentityFile ~/.ssh/id_rsa
```

#### Multiple keys

```bash
 Host *
   UseKeychain yes
   AddKeysToAgent yes
   IdentityFile ~/.ssh/id_rsa
   IdentityFile ~/.ssh/id_rsa2
```

## Gist

Link: https://gist.github.com/ralcorta/4008bde40ba99299e27d031b19d89098
