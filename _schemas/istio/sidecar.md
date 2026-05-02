---
description: A Sidecar configuration describes the sidecar proxy that mediates inbound and outbound communication to the workload instance it is attached to. By default, Istio configures every sidecar proxy to accept traffic on all ports and reach every service in the mesh. The Sidecar resource can restrict the set of services a sidecar can reach.
layout: schema
name: Istio Sidecar
properties_list:
- description: Criteria used to select the specific set of pods/VMs on which this Sidecar configuration should be applied.
  name: workloadSelector
  type: object
- description: Ingress specifies the configuration of the sidecar for processing inbound traffic to the attached workload instance.
  name: ingress
  type: array
- description: Egress specifies the configuration of the sidecar for processing outbound traffic from the attached workload instance.
  name: egress
  type: array
- description: Configuration for the outbound traffic policy.
  name: outboundTrafficPolicy
  type: object
- description: Settings controlling the volume of inbound connections.
  name: inboundConnectionPool
  type: object
provider_name: Istio
provider_slug: istio
schema_file: json-schema/sidecar.json
slug: sidecar
source_filename: sidecar.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/istio/blob/main/json-schema/sidecar.json\",\n  \"title\": \"Istio Sidecar\",\n  \"description\": \"A Sidecar configuration describes the sidecar proxy that mediates inbound and outbound communication to the workload instance it is attached to. By default, Istio configures every sidecar proxy to accept traffic on all ports and reach every service in the mesh. The Sidecar resource can restrict the set of services a sidecar can reach.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workloadSelector\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"labels\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"One or more labels that indicate a specific set of pods/VMs on which the configuration should be applied.\"\n        }\n      },\n\
  \      \"description\": \"Criteria used to select the specific set of pods/VMs on which this Sidecar configuration should be applied.\"\n    },\n    \"ingress\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"port\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"number\": {\n                \"type\": \"integer\",\n                \"description\": \"A valid non-negative integer port number.\"\n              },\n              \"protocol\": {\n                \"type\": \"string\",\n                \"description\": \"The protocol exposed on the port.\"\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"Label assigned to the port.\"\n              }\n            },\n            \"required\": [\"number\", \"protocol\"]\n          },\n          \"bind\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"The IP address to which the listener should be bound.\"\n          },\n          \"captureMode\": {\n            \"type\": \"string\",\n            \"enum\": [\"DEFAULT\", \"IPTABLES\", \"NONE\"],\n            \"description\": \"How traffic to the listener is expected to be captured.\"\n          },\n          \"defaultEndpoint\": {\n            \"type\": \"string\",\n            \"description\": \"The IP endpoint or Unix domain socket to which traffic should be forwarded.\"\n          },\n          \"tls\": {\n            \"type\": \"object\",\n            \"description\": \"TLS settings for the listener.\"\n          }\n        },\n        \"required\": [\"port\"]\n      },\n      \"description\": \"Ingress specifies the configuration of the sidecar for processing inbound traffic to the attached workload instance.\"\n    },\n    \"egress\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"port\": {\n        \
  \    \"type\": \"object\",\n            \"properties\": {\n              \"number\": {\n                \"type\": \"integer\"\n              },\n              \"protocol\": {\n                \"type\": \"string\"\n              },\n              \"name\": {\n                \"type\": \"string\"\n              }\n            }\n          },\n          \"bind\": {\n            \"type\": \"string\",\n            \"description\": \"The IP address or Unix domain socket to which the listener should be bound.\"\n          },\n          \"captureMode\": {\n            \"type\": \"string\",\n            \"enum\": [\"DEFAULT\", \"IPTABLES\", \"NONE\"],\n            \"description\": \"How traffic to the listener is expected to be captured.\"\n          },\n          \"hosts\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"One or more service hosts in namespace/dnsName format.\"\n          }\n     \
  \   },\n        \"required\": [\"hosts\"]\n      },\n      \"description\": \"Egress specifies the configuration of the sidecar for processing outbound traffic from the attached workload instance.\"\n    },\n    \"outboundTrafficPolicy\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"mode\": {\n          \"type\": \"string\",\n          \"enum\": [\"REGISTRY_ONLY\", \"ALLOW_ANY\"],\n          \"description\": \"Determines the handling of outbound traffic to services not defined in the service registry.\"\n        },\n        \"egressProxy\": {\n          \"type\": \"object\",\n          \"description\": \"Specifies the details of the egress proxy to which unknown traffic should be forwarded.\"\n        }\n      },\n      \"description\": \"Configuration for the outbound traffic policy.\"\n    },\n    \"inboundConnectionPool\": {\n      \"type\": \"object\",\n      \"description\": \"Settings controlling the volume of inbound connections.\",\n      \"properties\": {\n\
  \        \"tcp\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"maxConnections\": {\n              \"type\": \"integer\",\n              \"description\": \"Maximum number of connections.\"\n            },\n            \"connectTimeout\": {\n              \"type\": \"string\",\n              \"description\": \"TCP connection timeout.\"\n            }\n          }\n        },\n        \"http\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"h2UpgradePolicy\": {\n              \"type\": \"string\",\n              \"enum\": [\"DEFAULT\", \"DO_NOT_UPGRADE\", \"UPGRADE\"]\n            },\n            \"http1MaxPendingRequests\": {\n              \"type\": \"integer\"\n            },\n            \"http2MaxRequests\": {\n              \"type\": \"integer\"\n            },\n            \"maxRequestsPerConnection\": {\n              \"type\": \"integer\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/json-schema/sidecar.json
tags:
- CNCF
- Kubernetes
- Microservices
- Open Source
- Service Mesh
title: Istio Sidecar
---
