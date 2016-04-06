[![wercker status](https://app.wercker.com/status/1e7cd59501d48a3d6edb6ccefe4a4a69/m "wercker status")](https://app.wercker.com/project/bykey/1e7cd59501d48a3d6edb6ccefe4a4a69)

# wercker-playground
CD Playground

Deploys to http://apps.moinz.de/wercker-example/

Required ENVs for building:

* FS_USER - credentials to upload the artifact. See https://github.com/zeisss/fs-php/blob/master/fs.php
* FS_PASSWORD - Password for the given user
* FS_ENDPOINT - URL of the fs.php endpoint

Required ENVs for deployments:

* DEPLOY_TOKEN - token for `deploy.php` script (custom)
* DEPLOY_SITENAME - Sitename at the deploy endpoint
* DEPLOY_ENDPOINT - URL to use to trigger the deploy
* DEPLOY_SLACK_URL - If set, sends a slack notification after a successful deployment
