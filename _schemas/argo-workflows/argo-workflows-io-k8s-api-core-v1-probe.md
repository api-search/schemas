---
description: Probe describes a health check to be performed against a container to determine whether it is alive or ready to receive traffic.
layout: schema
name: io.k8s.api.core.v1.Probe
properties_list:
- description: Exec specifies a command to execute in the container.
  name: exec
  type: object
- description: Minimum consecutive failures for the probe to be considered failed after having succeeded. Defaults to 3. Minimum value is 1.
  name: failureThreshold
  type: integer
- description: GRPC specifies a GRPC HealthCheckRequest.
  name: grpc
  type: object
- description: HTTPGet specifies an HTTP GET request to perform.
  name: httpGet
  type: object
- description: 'Number of seconds after the container has started before liveness probes are initiated. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes'
  name: initialDelaySeconds
  type: integer
- description: How often (in seconds) to perform the probe. Default to 10 seconds. Minimum value is 1.
  name: periodSeconds
  type: integer
- description: Minimum consecutive successes for the probe to be considered successful after having failed. Defaults to 1. Must be 1 for liveness and startup. Minimum value is 1.
  name: successThreshold
  type: integer
- description: TCPSocket specifies a connection to a TCP port.
  name: tcpSocket
  type: object
- description: 'Optional duration in seconds the pod needs to terminate gracefully upon probe failure. The grace period is the duration in seconds after the processes running in the pod are sent a termination signal '
  name: terminationGracePeriodSeconds
  type: integer
- description: 'Number of seconds after which the probe times out. Defaults to 1 second. Minimum value is 1. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes'
  name: timeoutSeconds
  type: integer
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-probe-schema.json
slug: argo-workflows-io-k8s-api-core-v1-probe
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.Probe
---
