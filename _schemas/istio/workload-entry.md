---
description: A WorkloadEntry enables the addition of non-Kubernetes workloads such as virtual machines and bare metal servers into an Istio service mesh. It provides a way to describe the properties of a single non-Kubernetes workload so that Envoy sidecars on VMs and external endpoints can be treated uniformly with Kubernetes pods.
layout: schema
name: Istio WorkloadEntry
properties_list:
- description: Istio networking API version.
  name: apiVersion
  type: string
- description: Resource kind.
  name: kind
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: spec
  type: object
provider_name: Istio
provider_slug: istio
schema_file: json-schema/workload-entry.json
slug: workload-entry
source_filename: workload-entry.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/istio/blob/main/json-schema/workload-entry.json\",\n  \"title\": \"Istio WorkloadEntry\",\n  \"description\": \"A WorkloadEntry enables the addition of non-Kubernetes workloads such as virtual machines and bare metal servers into an Istio service mesh. It provides a way to describe the properties of a single non-Kubernetes workload so that Envoy sidecars on VMs and external endpoints can be treated uniformly with Kubernetes pods.\",\n  \"type\": \"object\",\n  \"required\": [\"apiVersion\", \"kind\", \"metadata\", \"spec\"],\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Istio networking API version.\",\n      \"enum\": [\"networking.istio.io/v1\", \"networking.istio.io/v1beta1\", \"networking.istio.io/v1alpha3\"]\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Resource kind.\"\
  ,\n      \"enum\": [\"WorkloadEntry\"]\n    },\n    \"metadata\": {\n      \"$ref\": \"#/$defs/ObjectMeta\"\n    },\n    \"spec\": {\n      \"$ref\": \"#/$defs/WorkloadEntrySpec\"\n    }\n  },\n  \"$defs\": {\n    \"ObjectMeta\": {\n      \"type\": \"object\",\n      \"title\": \"ObjectMeta\",\n      \"description\": \"Standard Kubernetes object metadata.\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the WorkloadEntry resource.\"\n        },\n        \"namespace\": {\n          \"type\": \"string\",\n          \"description\": \"Kubernetes namespace for the WorkloadEntry.\"\n        },\n        \"labels\": {\n          \"type\": \"object\",\n          \"description\": \"Labels to attach to this resource.\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        },\n        \"annotations\": {\n          \"type\": \"object\",\n          \"description\": \"Annotations\
  \ to attach to this resource.\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"WorkloadEntrySpec\": {\n      \"type\": \"object\",\n      \"title\": \"WorkloadEntrySpec\",\n      \"description\": \"Specification describing the properties of the non-Kubernetes workload.\",\n      \"required\": [\"address\"],\n      \"properties\": {\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"Address of the workload, typically an IP address of a VM or bare metal host. Can also be a DNS name when the resolution field of the associated ServiceEntry is set to DNS.\"\n        },\n        \"ports\": {\n          \"type\": \"object\",\n          \"description\": \"Port mapping from service port names to endpoint ports. If omitted, the endpoint port is assumed to be the same as the service port.\",\n          \"additionalProperties\": {\n            \"type\": \"integer\",\n            \"description\": \"Endpoint port\
  \ number.\",\n            \"minimum\": 1,\n            \"maximum\": 65535\n          }\n        },\n        \"labels\": {\n          \"type\": \"object\",\n          \"description\": \"Labels associated with the workload, used to match this endpoint to WorkloadGroup or ServiceEntry selectors.\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        },\n        \"network\": {\n          \"type\": \"string\",\n          \"description\": \"Network name this endpoint belongs to. Used for multi-network Istio deployments to ensure traffic routes via an appropriate gateway.\"\n        },\n        \"locality\": {\n          \"type\": \"string\",\n          \"description\": \"Locality of the endpoint in region/zone/subzone format (e.g., us-east-1/us-east-1a). Used for locality-aware load balancing.\"\n        },\n        \"weight\": {\n          \"type\": \"integer\",\n          \"description\": \"Load balancing weight for this endpoint. Higher weight means more traffic. Defaults\
  \ to 1.\",\n          \"minimum\": 1\n        },\n        \"serviceAccount\": {\n          \"type\": \"string\",\n          \"description\": \"Kubernetes service account associated with this workload, used for mTLS identity assignment in multi-cluster scenarios.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/json-schema/workload-entry.json
tags:
- CNCF
- Kubernetes
- Microservices
- Open Source
- Service Mesh
title: Istio WorkloadEntry
---
