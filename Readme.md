# Cleanslate Screener


App for screening for PA clean slate eligibility.


## Deployment with azure pipeline

The file `azure-pipelines.yml` describes an azure devops pipeline for deploying the app to an azure app service.

In azure devops, the devops project will find this pipeline, but you need to configure a couple varibles:

```
azureServiceConnectionId=
environmentName=
webAppName=
```

The code is in github (obviously!). I like to add an azure repo as a remote, called `azure`. Then when I'm ready to deploy, I `git push azure master`. This triggers the azure pipeline.