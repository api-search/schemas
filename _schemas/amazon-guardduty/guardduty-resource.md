---
description: Contains information about the Amazon Web Services resource associated with the activity that prompted GuardDuty to generate a finding.
layout: schema
name: Resource
properties_list:
- description: ''
  name: AccessKeyDetails
  type: object
- description: ''
  name: S3BucketDetails
  type: object
- description: ''
  name: InstanceDetails
  type: object
- description: ''
  name: EksClusterDetails
  type: object
- description: ''
  name: KubernetesDetails
  type: object
- description: ''
  name: ResourceType
  type: object
- description: ''
  name: EbsVolumeDetails
  type: object
- description: ''
  name: EcsClusterDetails
  type: object
- description: ''
  name: ContainerDetails
  type: object
- description: ''
  name: RdsDbInstanceDetails
  type: object
- description: ''
  name: RdsDbUserDetails
  type: object
- description: ''
  name: LambdaDetails
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-resource-schema.json
slug: guardduty-resource
source_filename: guardduty-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-resource-schema.json\",\n  \"title\": \"Resource\",\n  \"description\": \"Contains information about the Amazon Web Services resource associated with the activity that prompted GuardDuty to generate a finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessKeyDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessKeyDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accessKeyDetails\"\n          },\n          \"description\": \"The IAM access key details (user information) of a user that engaged in the activity that prompted GuardDuty to generate a finding.\"\n        }\n      ]\n    },\n    \"S3BucketDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketDetails\"\n  \
  \      },\n        {\n          \"xml\": {\n            \"name\": \"s3BucketDetails\"\n          },\n          \"description\": \"Contains information on the S3 bucket.\"\n        }\n      ]\n    },\n    \"InstanceDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"instanceDetails\"\n          },\n          \"description\": \"The information about the EC2 instance associated with the activity that prompted GuardDuty to generate a finding.\"\n        }\n      ]\n    },\n    \"EksClusterDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EksClusterDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"eksClusterDetails\"\n          },\n          \"description\": \"Details about the EKS cluster involved in a Kubernetes finding.\"\n        }\n      ]\n    },\n    \"KubernetesDetails\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/KubernetesDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kubernetesDetails\"\n          },\n          \"description\": \"Details about the Kubernetes user and workload involved in a Kubernetes finding.\"\n        }\n      ]\n    },\n    \"ResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resourceType\"\n          },\n          \"description\": \"The type of Amazon Web Services resource.\"\n        }\n      ]\n    },\n    \"EbsVolumeDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EbsVolumeDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ebsVolumeDetails\"\n          },\n          \"description\": \"Contains list of scanned and skipped EBS volumes with details.\"\n        }\n      ]\n    },\n    \"EcsClusterDetails\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EcsClusterDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ecsClusterDetails\"\n          },\n          \"description\": \"Contains information about the details of the ECS Cluster.\"\n        }\n      ]\n    },\n    \"ContainerDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Container\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"containerDetails\"\n          }\n        }\n      ]\n    },\n    \"RdsDbInstanceDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RdsDbInstanceDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rdsDbInstanceDetails\"\n          },\n          \"description\": \"Contains information about the database instance to which an anomalous login attempt was made.\"\n        }\n      ]\n    },\n    \"RdsDbUserDetails\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RdsDbUserDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rdsDbUserDetails\"\n          },\n          \"description\": \"Contains information about the user details through which anomalous login attempt was made.\"\n        }\n      ]\n    },\n    \"LambdaDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lambdaDetails\"\n          },\n          \"description\": \"Contains information about the Lambda function that was involved in a finding.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-resource-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: Resource
---
