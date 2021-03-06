# Example

Use optionally the summarize function to add more information to the `/info/summary`

```
const info = require('mxd-info')(config, app);

const summarize = summary => {};
info(summarize); 
```


# Config

List of JSON paths of the info (config and package) which will be disguised for the `/info/config`, `/info/package` and `/info/properties`. For `/info/properties` the paths from `/info/config` will also be used

## Environment Variables

If environment variables are set, the config object will be ignored!

* MXD_INFO: JSON encodet list of JSON paths

## 'config' Object

```
{
  "info": []
}
```


# Routes

* `/info` and `/info/summary`: response the summary with the most important information
* `/info/config`: response the config
* `/info/package`: response the `package.json`
* `/info/properties`: response the `config/properties.json`
* `/info/version`: response the version with the revision
