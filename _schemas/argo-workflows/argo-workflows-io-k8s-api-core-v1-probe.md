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
source_filename: argo-workflows-io-k8s-api-core-v1-probe-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-probe-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.Probe\",\n  \"description\": \"Probe describes a health check to be performed against a container to determine whether it is alive or ready to receive traffic.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exec\": {\n      \"description\": \"Exec specifies a command to execute in the container.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ExecAction\"\n    },\n    \"failureThreshold\": {\n      \"description\": \"Minimum consecutive failures for the probe to be considered failed after having succeeded. Defaults to 3. Minimum value is 1.\",\n      \"type\": \"integer\"\n    },\n    \"grpc\": {\n      \"description\": \"GRPC specifies a GRPC HealthCheckRequest.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.GRPCAction\"\
  \n    },\n    \"httpGet\": {\n      \"description\": \"HTTPGet specifies an HTTP GET request to perform.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.HTTPGetAction\"\n    },\n    \"initialDelaySeconds\": {\n      \"description\": \"Number of seconds after the container has started before liveness probes are initiated. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes\",\n      \"type\": \"integer\"\n    },\n    \"periodSeconds\": {\n      \"description\": \"How often (in seconds) to perform the probe. Default to 10 seconds. Minimum value is 1.\",\n      \"type\": \"integer\"\n    },\n    \"successThreshold\": {\n      \"description\": \"Minimum consecutive successes for the probe to be considered successful after having failed. Defaults to 1. Must be 1 for liveness and startup. Minimum value is 1.\",\n      \"type\": \"integer\"\n    },\n    \"tcpSocket\": {\n      \"description\": \"TCPSocket specifies a connection to a TCP port.\"\
  ,\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.TCPSocketAction\"\n    },\n    \"terminationGracePeriodSeconds\": {\n      \"description\": \"Optional duration in seconds the pod needs to terminate gracefully upon probe failure. The grace period is the duration in seconds after the processes running in the pod are sent a termination signal and the time when the processes are forcibly halted with a kill signal. Set this value longer than the expected cleanup time for your process. If this value is nil, the pod's terminationGracePeriodSeconds will be used. Otherwise, this value overrides the value provided by the pod spec. Value must be non-negative integer. The value zero indicates stop immediately via the kill signal (no opportunity to shut down). This is a beta field and requires enabling ProbeTerminationGracePeriod feature gate. Minimum value is 1. spec.terminationGracePeriodSeconds is used if unset.\",\n      \"type\": \"integer\"\n    },\n    \"timeoutSeconds\": {\n      \"description\"\
  : \"Number of seconds after which the probe times out. Defaults to 1 second. Minimum value is 1. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-probe-schema.json
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
