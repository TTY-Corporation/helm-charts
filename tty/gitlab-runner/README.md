# Instructions

Make sure you modify the values.yaml file to match your environment.
- gitlabUrl: The URL of your GitLab instance
- runnerRegistrationToken: The registration token for your GitLab Runner

### Add the GitLab Helm repository

```bash
helm repo add gitlab https://charts.gitlab.io
```

### Helm init
```bash
helm init
```

### Install GitLab Runner

```bash
helm install --namespace <NAMESPACE> gitlab-runner -f values.yaml gitlab/gitlab-runner
```