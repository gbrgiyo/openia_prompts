
## AI-prompts-




| NAME                     | PROMPT              | DESCRIPTION                                 | EXAMPLE                                                    |
|--------------------------|---------------------|---------------------------------------------|------------------------------------------------------------|
| app.yaml                 | kind: Pod;app;gcr.io/k8s-k3s/demo:v1.0.0;ports  | Manifest defining a basic application.      | [Example](./yaml/app.yaml)                                |
| app-livenessProbe.yaml    |    app-livenessProbe;namespace: demo;gcr.io/k8s-k3s/demo:v1.0.0   | Manifest demonstrating a liveness probe.   | [Example](./yaml/app-livenessProbe.yaml)                   |
| app-readinessProbe.yaml   | app-readinessprob;gcr.io/k8s-k3s/demo:v2.0.0;livenessProbe;readinessProbe;ports     | Manifest showing a readiness probe.         | [Example](./yaml/app-readinessProbe.yaml)                  |
| app-volumeMounts.yaml     | kubectl ai "kind: Pod;app-volume;gcr.io/kuar-demo/kuard-amd64:1;livenessProbe;readinessProbe;ports;volumeMounts"       | Manifest with volume mount configurations.  | [Example](./yaml/app-volumeMounts.yaml)                    |
| app-cronjob.yaml          | app-cronjob apiVersion: batch/v1beta1             | Manifest defining a cron job.               | [Example](./yaml/app-cronjob.yaml)                         |
| app-job.yaml              | app-job-rsync batch/v1 gcePersistentDisk image google/cloud-sdk:275.0.0-alpine command -/bin/sh volumeMounts                 | Manifest for running a one-off job.         | [Example](./yaml/app-job.yaml)                             |
| app-multicontainer.yaml   | app-multi-containers | Manifest for a multi-container application. | [Example](./yaml/app-multicontainer.yaml)                  |
| app-resources.yaml        | kind: Pod;app-livenessprob;gcr.io/k8s-k3s/demo:v1.0.0;ports     | Manifest demonstrating resource limits.     | [Example](./yaml/app-resources.yaml)                       |
| app-secret-env.yaml       | kind: Pod;app-secret-env   | Manifest using secrets as environment vars. | [Example](./yaml/app-secret-env.yaml)                      |
