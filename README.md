# sitecore-publishing-module
Repo to host the Sitecore publishing service module package converted to scwdp

[Sitecore docker images](https://github.com/Sitecore/docker-images) uses the Sitecore web deploy packages (.scwdp.zip extension) technique  to install the package on base images.

On Sitecore official dev.sitecore.com site, the Sitecore Pubishing module is only available as traditionl Sitecore package which will cause an issue when used for building the docker images. This repository is created to host the module in scwdp format to consume while building the docker images.

## Where to add the link to scwdp?

For example, in the packages json file at https://github.com/Sitecore/docker-images/blob/master/sitecore-packages.json, add the link to the scwdp under

```
"Sitecore Publishing Module 9.3.0.0 rev. r00546.2197.scwdp.zip": {
    "url": "https://github.com/phaniav/sitecore-publishing-module/blob/master/Sitecore%20Publishing%20Module%209.3.0.0%20rev.%20r00546.2197.scwdp.zip?raw=true"
  }
```
