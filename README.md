# k8s-campaigns

This repository contains the campaign specs for the [Sourcegraph campaigns](https://docs.sourcegraph.com/@main/user/campaigns) we have on our dogfood instance at [k8s.sgdev.org/campaigns](https://k8s.sgdev.org/campaigns).

All of the campaigns have been created in the `campaigns-team` namespace with the following command:

```bash
for f in *.campaigns.yaml;
do
  src campaign apply -f "${f}" -namespace campaigns-team
done
```
