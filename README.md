# devcontainers
This repository hosts a series of files needed to run different devcontainers for app development

## Warning
If you are using Git for source control, you may run into issues with files being marked as Modified after opening the workspace
in a devcontainer. This is because file permissions are getting adjusted. You can either adjust the Dockerfile to run `chmod` on the `/workspace` directory, or, if file permissions are not essential for your app/workstation, you can configure Git to ignore changes to file permissions.

### Ignore Permission Changes Globally
```bash
git config --global core.fileMode false
```

### Ignore Permission Changes for Current Repository
```bash
git config core.fileMode false
```

## SpringBoot + Postgres
This devcontainer is configured to develop SpringBoot applications alongside an active Postgres server.