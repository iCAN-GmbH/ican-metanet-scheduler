# iCAN METANET acceptance scheduler

This repository requests an acceptance check at minutes 04, 19, 34 and 49 each hour. GitHub Actions sends a repository dispatch event to the configured deployment repository. **Dispatch acceptance check** also supports a manual run.

The workflow obtains a short-lived GitHub App installation token from the `acceptance-dispatch` environment on `main`. The deployment and its configuration are maintained in the private deployment repository.
