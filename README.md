# oci-cloud-init

## Install cookiecutter

```sh
python -m pip install --user cookiecutter
```

## Setup Cookiecutter configuration file

This file will contain the admin credentials for cloud inits

1. At itops/ create '.cookiecutterrc'

```sh
---
default_context:
    admin_username: "<replace_with_admin>"
    admin_password: "<replace-with-admin-password>"
```

## Run Cookiecutter

Use the readme within the folders to run the cookiecutters
