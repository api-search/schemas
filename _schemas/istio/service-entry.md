---
description: A ServiceEntry enables adding additional entries into Istio's internal service registry so that auto-discovered services in the mesh can access or route to these manually specified services.
layout: schema
name: Istio ServiceEntry
properties_list:
- description: The hosts associated with the ServiceEntry. Could be a DNS name with wildcard prefix.
  name: hosts
  type: array
- description: The virtual IP addresses associated with the service.
  name: addresses
  type: array
- description: The ports associated with the external service.
  name: ports
  type: array
- description: Specify whether the service should be considered external to the mesh or part of the mesh.
  name: location
  type: string
- description: Service discovery mode for the hosts.
  name: resolution
  type: string
- description: One or more endpoints associated with the service.
  name: endpoints
  type: array
- description: Applicable only for MESH_INTERNAL services. Selects workloads to treat as part of this service.
  name: workloadSelector
  type: object
- description: A list of namespaces to which this ServiceEntry is exported.
  name: exportTo
  type: array
- description: A list of subject alternative names for TLS verification.
  name: subjectAltNames
  type: array
provider_name: Istio
provider_slug: istio
schema_file: json-schema/service-entry.json
slug: service-entry
source_filename: service-entry.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/istio/blob/main/json-schema/service-entry.json\",\n  \"title\": \"Istio ServiceEntry\",\n  \"description\": \"A ServiceEntry enables adding additional entries into Istio's internal service registry so that auto-discovered services in the mesh can access or route to these manually specified services.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hosts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The hosts associated with the ServiceEntry. Could be a DNS name with wildcard prefix.\"\n    },\n    \"addresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The virtual IP addresses associated with the service.\"\n    },\n    \"ports\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\
  ,\n        \"properties\": {\n          \"number\": {\n            \"type\": \"integer\",\n            \"description\": \"A valid non-negative integer port number.\"\n          },\n          \"protocol\": {\n            \"type\": \"string\",\n            \"description\": \"The protocol exposed on the port (HTTP, HTTPS, GRPC, HTTP2, MONGO, TCP, TLS).\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Label assigned to the port.\"\n          },\n          \"targetPort\": {\n            \"type\": \"integer\",\n            \"description\": \"The port number on the endpoint where traffic will be received.\"\n          }\n        },\n        \"required\": [\"number\", \"protocol\", \"name\"]\n      },\n      \"description\": \"The ports associated with the external service.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"enum\": [\"MESH_EXTERNAL\", \"MESH_INTERNAL\"],\n      \"description\": \"Specify whether the service\
  \ should be considered external to the mesh or part of the mesh.\"\n    },\n    \"resolution\": {\n      \"type\": \"string\",\n      \"enum\": [\"NONE\", \"STATIC\", \"DNS\", \"DNS_ROUND_ROBIN\"],\n      \"description\": \"Service discovery mode for the hosts.\"\n    },\n    \"endpoints\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"address\": {\n            \"type\": \"string\",\n            \"description\": \"Address associated with the network endpoint (IPv4 or IPv6, or a Unix domain socket path).\"\n          },\n          \"ports\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"type\": \"integer\"\n            },\n            \"description\": \"Set of ports associated with the endpoint.\"\n          },\n          \"labels\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"type\": \"string\"\n            },\n \
  \           \"description\": \"One or more labels associated with the endpoint.\"\n          },\n          \"network\": {\n            \"type\": \"string\",\n            \"description\": \"Network enables Istio to group endpoints resident in the same L3 domain/network.\"\n          },\n          \"locality\": {\n            \"type\": \"string\",\n            \"description\": \"The locality associated with the endpoint in region/zone/sub-zone format.\"\n          },\n          \"weight\": {\n            \"type\": \"integer\",\n            \"description\": \"The load balancing weight associated with the endpoint.\"\n          },\n          \"serviceAccount\": {\n            \"type\": \"string\",\n            \"description\": \"The service account associated with the workload.\"\n          }\n        }\n      },\n      \"description\": \"One or more endpoints associated with the service.\"\n    },\n    \"workloadSelector\": {\n      \"type\": \"object\",\n      \"properties\": {\n       \
  \ \"labels\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"One or more labels that indicate a specific set of pods/VMs.\"\n        }\n      },\n      \"description\": \"Applicable only for MESH_INTERNAL services. Selects workloads to treat as part of this service.\"\n    },\n    \"exportTo\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A list of namespaces to which this ServiceEntry is exported.\"\n    },\n    \"subjectAltNames\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A list of subject alternative names for TLS verification.\"\n    }\n  },\n  \"required\": [\"hosts\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/json-schema/service-entry.json
tags:
- CNCF
- Kubernetes
- Microservices
- Open Source
- Service Mesh
title: Istio ServiceEntry
---
