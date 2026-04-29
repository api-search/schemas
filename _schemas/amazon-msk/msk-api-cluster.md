---
description: <p>Returns information about a cluster.</p>
layout: schema
name: Cluster
properties_list:
- description: ''
  name: ActiveOperationArn
  type: object
- description: ''
  name: ClusterType
  type: object
- description: ''
  name: ClusterArn
  type: object
- description: ''
  name: ClusterName
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: CurrentVersion
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: StateInfo
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Provisioned
  type: object
- description: ''
  name: Serverless
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-cluster-schema.json
slug: msk-api-cluster
source_filename: msk-api-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-cluster-schema.json\",\n  \"title\": \"Cluster\",\n  \"description\": \"\\n            <p>Returns information about a cluster.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActiveOperationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"activeOperationArn\"\n          },\n          \"description\": \"\\n            <p>The Amazon Resource Name (ARN) that uniquely identifies a cluster operation.</p>\"\n        }\n      ]\n    },\n    \"ClusterType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClusterType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clusterType\"\n          },\n          \"description\": \"\\n    \
  \        <p>Cluster Type.</p>\"\n        }\n      ]\n    },\n    \"ClusterArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clusterArn\"\n          },\n          \"description\": \"\\n            <p>The Amazon Resource Name (ARN) that uniquely identifies the cluster.</p>\"\n        }\n      ]\n    },\n    \"ClusterName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clusterName\"\n          },\n          \"description\": \"\\n            <p>The name of the cluster.</p>\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"creationTime\"\n          },\n          \"description\": \"\\n            <p>The\
  \ time when the cluster was created.</p>\"\n        }\n      ]\n    },\n    \"CurrentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"currentVersion\"\n          },\n          \"description\": \"\\n            <p>The current version of the MSK cluster.</p>\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClusterState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"state\"\n          },\n          \"description\": \"\\n            <p>The state of the cluster. The possible states are ACTIVE, CREATING, DELETING, FAILED, HEALING, MAINTENANCE, REBOOTING_BROKER, and UPDATING.</p>\"\n        }\n      ]\n    },\n    \"StateInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StateInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"stateInfo\"\n          },\n          \"description\": \"\\n            <p>State Info for the Amazon MSK cluster.</p>\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"\\n            <p>Tags attached to the cluster.</p>\"\n        }\n      ]\n    },\n    \"Provisioned\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Provisioned\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"provisioned\"\n          },\n          \"description\": \"\\n            <p>Information about the provisioned cluster.</p>\"\n        }\n      ]\n    },\n    \"Serverless\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Serverless\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"serverless\"\n    \
  \      },\n          \"description\": \"\\n            <p>Information about the serverless cluster.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-cluster-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Cluster
---
