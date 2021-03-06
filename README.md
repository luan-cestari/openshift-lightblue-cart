# OpenShift Lightblue Cartridge


# Getting Started with OpenShift
If you don't have an OpenShift account, don't worry.  It's FREE!

Check out this [Getting Started](https://developers.openshift.com/en/getting-started-overview.html) guide provided by [OpenShift](https://www.openshift.com/).

# Creating a lightblue application
With this downloadable cart it's really simple.  For now, I'm documenting the way to do it with the ```rhc``` command.

NOTE: this cart works only with lightblue version 1.1 or greater.  At this time 1.1 is not released, so snapshots must be used.

```
rhc app create -e SNAPSHOT=true https://raw.githubusercontent.com/jewzaam/openshift-lightblue-cart/master/metadata/manifest.yml -a <YOUR APP NAME>
```

That's it.  This deploys JBoss EAP and MongoDB then installs and configures lightblue.  After this command completes you have a working instance of lightblue!  Check out the README.md at the root of your gear's source for some quick things to do to try out lightblue and links to documentation, forums, and source.
