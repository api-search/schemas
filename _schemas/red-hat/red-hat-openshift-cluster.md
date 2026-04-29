---
description: Schema for an OpenShift cluster managed through the Red Hat OpenShift Cluster Manager, representing a Kubernetes cluster deployed on a cloud provider.
layout: schema
name: Red Hat OpenShift Cluster
properties_list:
- description: The unique identifier of the cluster assigned by the Cluster Manager.
  name: id
  type: string
- description: The name of the cluster, used as a human-readable identifier.
  name: name
  type: string
- description: The display name of the cluster shown in the Hybrid Cloud Console.
  name: display_name
  type: string
- description: The current lifecycle state of the cluster.
  name: state
  type: string
- description: The cloud provider where the cluster is deployed.
  name: cloud_provider
  type: object
- description: The cloud provider region where the cluster is deployed.
  name: region
  type: object
- description: Whether the cluster spans multiple availability zones for high availability.
  name: multi_az
  type: boolean
- description: The OpenShift version running on the cluster.
  name: openshift_version
  type: string
- description: The node configuration of the cluster.
  name: nodes
  type: object
- description: The cluster API server configuration.
  name: api
  type: object
- description: The OpenShift web console configuration.
  name: console
  type: object
- description: The network configuration of the cluster.
  name: network
  type: object
- description: The subscription associated with this cluster.
  name: subscription
  type: object
- description: The date and time when the cluster was created in ISO 8601 format.
  name: creation_timestamp
  type: string
- description: The date and time when the cluster is set to expire, if applicable.
  name: expiration_timestamp
  type:
  - string
  - 'null'
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-openshift-cluster-schema.json
slug: red-hat-openshift-cluster
source_filename: red-hat-openshift-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.openshift.com/schemas/red-hat/openshift-cluster.json\",\n  \"title\": \"Red Hat OpenShift Cluster\",\n  \"description\": \"Schema for an OpenShift cluster managed through the Red Hat OpenShift Cluster Manager, representing a Kubernetes cluster deployed on a cloud provider.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"state\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the cluster assigned by the Cluster Manager.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the cluster, used as a human-readable identifier.\",\n      \"minLength\": 1,\n      \"maxLength\": 54,\n      \"pattern\": \"^[a-z][a-z0-9-]*$\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the cluster shown in the Hybrid Cloud\
  \ Console.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current lifecycle state of the cluster.\",\n      \"enum\": [\n        \"error\",\n        \"hibernating\",\n        \"installing\",\n        \"pending\",\n        \"powering_down\",\n        \"ready\",\n        \"resuming\",\n        \"uninstalling\",\n        \"unknown\",\n        \"validating\",\n        \"waiting\"\n      ]\n    },\n    \"cloud_provider\": {\n      \"type\": \"object\",\n      \"description\": \"The cloud provider where the cluster is deployed.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The cloud provider identifier.\",\n          \"enum\": [\"aws\", \"gcp\", \"azure\"]\n        },\n        \"display_name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the cloud provider.\"\n        }\n      },\n      \"required\": [\"id\"]\n    },\n    \"region\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"The cloud provider region where the cluster is deployed.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The region identifier (e.g., us-east-1, europe-west1).\"\n        },\n        \"display_name\": {\n          \"type\": \"string\",\n          \"description\": \"The human-readable region name.\"\n        }\n      },\n      \"required\": [\"id\"]\n    },\n    \"multi_az\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the cluster spans multiple availability zones for high availability.\",\n      \"default\": false\n    },\n    \"openshift_version\": {\n      \"type\": \"string\",\n      \"description\": \"The OpenShift version running on the cluster.\",\n      \"pattern\": \"^\\\\d+\\\\.\\\\d+\\\\.\\\\d+$\"\n    },\n    \"nodes\": {\n      \"type\": \"object\",\n      \"description\": \"The node configuration of the cluster.\",\n      \"properties\": {\n        \"\
  master\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of master nodes.\",\n          \"minimum\": 1\n        },\n        \"compute\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of compute (worker) nodes.\",\n          \"minimum\": 0\n        },\n        \"infra\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of infrastructure nodes.\",\n          \"minimum\": 0\n        },\n        \"compute_machine_type\": {\n          \"type\": \"object\",\n          \"description\": \"The instance type for compute nodes.\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\",\n              \"description\": \"The machine type identifier.\"\n            }\n          }\n        }\n      }\n    },\n    \"api\": {\n      \"type\": \"object\",\n      \"description\": \"The cluster API server configuration.\",\n      \"properties\": {\n        \"url\": {\n          \"type\"\
  : \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL of the cluster API server.\"\n        },\n        \"listening\": {\n          \"type\": \"string\",\n          \"description\": \"The API server listening mode.\",\n          \"enum\": [\"external\", \"internal\"]\n        }\n      }\n    },\n    \"console\": {\n      \"type\": \"object\",\n      \"description\": \"The OpenShift web console configuration.\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL of the OpenShift web console.\"\n        }\n      }\n    },\n    \"network\": {\n      \"type\": \"object\",\n      \"description\": \"The network configuration of the cluster.\",\n      \"properties\": {\n        \"machine_cidr\": {\n          \"type\": \"string\",\n          \"description\": \"The CIDR block for machine network.\",\n          \"pattern\": \"^\\\\d+\\\\.\\\\d+\\\\.\\\\d+\\\\.\\\\d+/\\\\\
  d+$\"\n        },\n        \"service_cidr\": {\n          \"type\": \"string\",\n          \"description\": \"The CIDR block for Kubernetes services.\"\n        },\n        \"pod_cidr\": {\n          \"type\": \"string\",\n          \"description\": \"The CIDR block for Kubernetes pods.\"\n        },\n        \"host_prefix\": {\n          \"type\": \"integer\",\n          \"description\": \"The prefix length for per-node pod CIDR allocation.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The network plugin type.\",\n          \"enum\": [\"OpenShiftSDN\", \"OVNKubernetes\"]\n        }\n      }\n    },\n    \"subscription\": {\n      \"type\": \"object\",\n      \"description\": \"The subscription associated with this cluster.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The subscription identifier.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n   \
  \       \"description\": \"The subscription status.\"\n        }\n      }\n    },\n    \"creation_timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the cluster was created in ISO 8601 format.\"\n    },\n    \"expiration_timestamp\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the cluster is set to expire, if applicable.\"\n    }\n  },\n  \"$defs\": {\n    \"MachinePool\": {\n      \"type\": \"object\",\n      \"description\": \"A machine pool defining a group of compute nodes with shared configuration.\",\n      \"required\": [\"id\", \"instance_type\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the machine pool.\"\n        },\n        \"instance_type\": {\n          \"type\": \"string\",\n          \"description\": \"The cloud provider instance\
  \ type for nodes in this pool.\"\n        },\n        \"replicas\": {\n          \"type\": \"integer\",\n          \"description\": \"The fixed number of nodes.\",\n          \"minimum\": 0\n        },\n        \"autoscaling\": {\n          \"type\": \"object\",\n          \"description\": \"Autoscaling configuration.\",\n          \"properties\": {\n            \"min_replicas\": {\n              \"type\": \"integer\",\n              \"minimum\": 0\n            },\n            \"max_replicas\": {\n              \"type\": \"integer\",\n              \"minimum\": 1\n            }\n          }\n        },\n        \"availability_zones\": {\n          \"type\": \"array\",\n          \"description\": \"The availability zones for node placement.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"labels\": {\n          \"type\": \"object\",\n          \"description\": \"Kubernetes labels applied to nodes.\",\n          \"additionalProperties\": {\n\
  \            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"examples\": [\n    {\n      \"id\": \"1n2j3b4k5l6m7n8o9p0q\",\n      \"name\": \"production-cluster\",\n      \"display_name\": \"Production Cluster\",\n      \"state\": \"ready\",\n      \"cloud_provider\": {\n        \"id\": \"aws\",\n        \"display_name\": \"Amazon Web Services\"\n      },\n      \"region\": {\n        \"id\": \"us-east-1\",\n        \"display_name\": \"US East (N. Virginia)\"\n      },\n      \"multi_az\": true,\n      \"openshift_version\": \"4.15.2\",\n      \"nodes\": {\n        \"master\": 3,\n        \"compute\": 6,\n        \"infra\": 3,\n        \"compute_machine_type\": {\n          \"id\": \"m5.2xlarge\"\n        }\n      },\n      \"api\": {\n        \"url\": \"https://api.production-cluster.example.com:6443\",\n        \"listening\": \"external\"\n      },\n      \"console\": {\n        \"url\": \"https://console-openshift-console.apps.production-cluster.example.com\"\
  \n      },\n      \"creation_timestamp\": \"2024-01-15T10:30:00Z\",\n      \"expiration_timestamp\": null\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-openshift-cluster-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: Red Hat OpenShift Cluster
---
