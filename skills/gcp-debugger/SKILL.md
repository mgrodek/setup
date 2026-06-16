## Safety rules

- Start with read-only diagnostics only.
- Allowed by default: kubectl get, describe, logs, top, config current-context, config get-contexts.
- Allowed by default: gcloud config list, gcloud logging read.
- Ask before running authentication scripts.
- Ask before kubectl exec or port-forward.
- Never run kubectl delete, apply, replace, patch, scale, rollout restart, drain, cordon or uncordon unless the user explicitly asks for that exact command.
- Never change DEV/UAT/PROD resources as part of diagnosis.
- First summarize the planned commands and wait for confirmation when the environment is unclear.

Example:

1.

/gcp-debugger

Dry run. Do not run commands yet.
I want to debug DEV environment. First list the read-only kubectl and gcloud commands you would run and explain why.
Do not use exec, port-forward, restart, patch, scale, delete, apply or update.

2.

Run only the read-only commands from the plan. Stop before any command that could modify the cluster or access a shell inside a pod.