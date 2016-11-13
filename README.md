# FastBoot Google Cloud Storage Notifier

``` js
const GCSNotifier = require('fastboot-gcs-notifier');

const notifier = new GCSNotifier({
  bucket: 'bucket-name',                    // required
  key: 'path/to/fastboot-deploy-info.json', // required
  poll: 10 * 1000,                          // optional; default: 3000 (in milliseconds)
  authentication: {                         // optional; see below
    projectId: 'project-id',
    keyFilename: 'path/to/key'
  }
});
```

For details on authentication, see [Google Cloud Node.js documentation](https://googlecloudplatform.github.io/google-cloud-node/#/docs/google-cloud/guides/authentication).
