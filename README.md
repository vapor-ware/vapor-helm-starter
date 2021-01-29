# vapor-helm-starter

A [starter template](https://v2.helm.sh/docs/developing_charts/#chart-starter-packs) for Helm charts for generic applications at Vapor IO.

Instead of having to create the same base set of resources and do many of the same modifications to the
default generated Helm templates, use this starter to provide the basic resource definitions for what a
typical Helm Chart looks like at Vapor.

## Installing

- Clone or link this repo into `$HELM_HOME/starters` (e.g. `~/.helm/starters`)
- Install with the [`helm-starter`](https://github.com/salesforce/helm-starter) plugin.

  ```
  helm plugin install https://github.com/salesforce/helm-starter.git
  
  helm starter fetch https://github.com/vapor-ware/vapor-helm-starter.git
  ```

## Usage

```console
# Create a new chart using the starter
$ helm create NAME --starter vapor-helm-starter
```

## Notes

This starter is just that -- a starting point to make it easier to author a new Helm Chart. While the starter
provides a lot of basics and sane defaults, it is up to you to go through and ensure the Chart is configured
correctly for your application. Not all applications are the same, so this starting point will need to be tweaked
and expanded upon to fit the needs of your application.

In particular, you will need to ensure the metadata in `Chart.yaml` is updated and correct.
