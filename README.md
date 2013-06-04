pushify
=======

A small script that will add a push-url to the current project.

Assumes you are using ssh-keys.

Usage
-----

```bash
code/watchfiles$ git remote show origin
* remote origin
  Fetch URL: https://github.com/sergeio/watchfiles.git
  Push  URL: https://github.com/sergeio/watchfiles.git
  HEAD branch: master
  Remote branch:
    master tracked
  Local branch configured for 'git pull':
    master merges with remote master
  Local ref configured for 'git push':
    master pushes to master (up to date)
code/watchfiles$ pushify
code/watchfiles$ git remote show origin
WARNING: gnome-keyring:: couldn't connect to: /tmp/keyring-zseNu9/pkcs11: No such file or directory
* remote origin
  Fetch URL: https://github.com/sergeio/watchfiles.git
  Push  URL: git@github.com:sergeio/watchfiles.git
  HEAD branch: master
  Remote branch:
    master tracked
  Local branch configured for 'git pull':
    master merges with remote master
  Local ref configured for 'git push':
    master pushes to master (up to date)
```

Note that the `Push URL` is now using ssh.
