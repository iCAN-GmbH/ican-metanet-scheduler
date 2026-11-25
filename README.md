# iCAN METANET acceptance scheduler

cron-job.org dispatches **Dispatch acceptance check** at minutes 04, 19, 34 and 49 each hour. The GitHub workflow sends a repository dispatch event to the configured deployment repository. It also supports a manual run.

The workflow obtains a short-lived GitHub App installation token from the `acceptance-dispatch` environment on `main`. The deployment and its configuration are maintained in the private deployment repository.
