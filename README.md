# example

Use optionally the summarize function to add more information to the ```/info/summary```

```
const summarize = (summary) => {};
require('mxd-info')(config)(app, summarize);
```


# config

List of JSON paths of the info (config and package) which will be disguised for the ```/info/config``` and ```/info/package```

## environment variables

If environment variables are set, the config object will be ignored!

* MXD_INFO: JSON encodet list of JSON paths

## config object

```
{
  "info": []
}
```


# routes

* ```/info``` and ```/info/summary```: response the summary with the most important information
* ```/info/config```: response the config
* ```/info/package```: response the ```package.json```
* ```/info/version```: response the version with the revision
