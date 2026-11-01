# clearance-deploy-scratch

A scratch repository for Clearance's deployment protection rule (the Hangar Clearance GitHub App,
[clearance docs/provenance-app.md](https://github.com/jfillman/clearance/blob/main/docs/provenance-app.md), phase 2a).

`.github/workflows/deploy.yaml` has one job targeting the `prod` environment. The environment lists Hangar Clearance
under *Deployment protection rules*, so the job starts only when Clearance approves: when the deployment gate has a
cleared change for this repository, the commit and env `prod`. It deploys nothing.
