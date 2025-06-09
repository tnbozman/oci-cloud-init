# OL9 Cloud-Init Template

This template generates a **cloud-init** configuration file for setting up a Oracle Linux 9 with a development user with docker.


## Configuration Parameters

The following parameters are used in this template. You can customize them to meet your specific requirements:

| Parameter          | Default Value               | Description                                                |
|--------------------|-----------------------------|------------------------------------------------------------|
| `username`         | `developer`                | The name of the primary development user to be created <surname><initial>.    |
| `user_groups`      | `developers`               | Groups that the development user should belong to.         |
| `user_public_key`  | `ssh-rsa AAAA...your-key`  | SSH public key for the development user.                   |
| `admin_password`   | `password`                 | Password for the administrator account.                    |

## Usage

### Step 1: Ensure Cookiecutter is installed

```bash
cookiecutter --version
```
If fails following instructions to [install cookiecutter](../../README.md)

### Step 2: Run the Template
Run the template by providing the path to the template directory:

```bash
cookiecutter --config-file=.cookiecutterrc ol9-cloud-init
```