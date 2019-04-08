1. Update `.envrc` to change the value of `$LOCAL_SUBDOMAIN`.
2. Run `brew bundle`
3. Create certificate for `bosh.${LOCAL_SUBDOMAIN}` using `certbot` (scripts depend on the file locations it uses)
4. Run `create` to create your director.
