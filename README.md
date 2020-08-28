# aws-monitor

Use prometheus to monitor whatever. Pushing docker-compose setup to ECS via ecs-cli && fargate.

By default prometheus has no security so NGINX is put in front as a reverse proxy to be the Web APP basic security layer.

## UP

```bash
$ ecs-cli compose --project-name prometheus service up --cluster-config fargate-config --ecs-profile prometheus-profile
```

## DOWN

```bash
$ ecs-cli compose --project-name prometheus service down --cluster-config fargate-config --ecs-profile prometheus-profile
```
