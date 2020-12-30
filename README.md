0. Make sure you have the source for `bosh-deployment` in the directory above this one.
1. Update `.envrc` to change the value of `$LOCAL_SUBDOMAIN`.
2. Run `brew bundle`
3. Create certificate for `bosh.${LOCAL_SUBDOMAIN}` using `certbot` (scripts depend on the file locations it uses)
4. Run `create` to create your director.
5. Create a directory for your deployment named for the deployment (matching the deployment name in your manifest)
6. Copy the manifest, releases, and stemcells for your deployment to the deployment directory.
7. Run `upload <deployment-name>`
8. Run `deploy <deployment-name>`
