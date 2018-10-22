# Bash Credential Manager

This is a simple credential manager for bash scripts with static credentials.

## Useage

Store all credentials inside `creds.yml` like so:
```
key1: value1
key2: value2
```

To retrieve a credential, call `get_credential.sh` (make sure you source the script):
```
. get_credential key1
echo $(KEY1)
```

Note that the created variable is now upper case

## Security
This is a simple solution for prototyping, make sure `creds.yml` is included in .gitignore
