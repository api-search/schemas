---
description: 'LoadBalancerIngress represents the status of a load-balancer ingress point: traffic intended for the service should be sent to an ingress point.'
layout: schema
name: v1LoadBalancerIngress
properties_list:
- description: ''
  name: hostname
  type: string
- description: ''
  name: ip
  type: string
- description: ''
  name: ipMode
  type: string
- description: ''
  name: ports
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1-load-balancer-ingress-schema.json
slug: argo-cd-v1-load-balancer-ingress
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1LoadBalancerIngress
---
