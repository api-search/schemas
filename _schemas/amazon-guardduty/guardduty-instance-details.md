---
description: Contains information about the details of an instance.
layout: schema
name: InstanceDetails
properties_list:
- description: ''
  name: AvailabilityZone
  type: object
- description: ''
  name: IamInstanceProfile
  type: object
- description: ''
  name: ImageDescription
  type: object
- description: ''
  name: ImageId
  type: object
- description: ''
  name: InstanceId
  type: object
- description: ''
  name: InstanceState
  type: object
- description: ''
  name: InstanceType
  type: object
- description: ''
  name: OutpostArn
  type: object
- description: ''
  name: LaunchTime
  type: object
- description: ''
  name: NetworkInterfaces
  type: object
- description: ''
  name: Platform
  type: object
- description: ''
  name: ProductCodes
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-instance-details-schema.json
slug: guardduty-instance-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-instance-details-schema.json\",\n  \"title\": \"InstanceDetails\",\n  \"description\": \"Contains information about the details of an instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AvailabilityZone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"availabilityZone\"\n          },\n          \"description\": \"The Availability Zone of the EC2 instance.\"\n        }\n      ]\n    },\n    \"IamInstanceProfile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamInstanceProfile\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"iamInstanceProfile\"\n          },\n          \"description\": \"The profile information of the\
  \ EC2 instance.\"\n        }\n      ]\n    },\n    \"ImageDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"imageDescription\"\n          },\n          \"description\": \"The image description of the EC2 instance.\"\n        }\n      ]\n    },\n    \"ImageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"imageId\"\n          },\n          \"description\": \"The image ID of the EC2 instance.\"\n        }\n      ]\n    },\n    \"InstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"instanceId\"\n          },\n          \"description\": \"The ID of the EC2 instance.\"\n        }\n      ]\n    },\n    \"InstanceState\": {\n      \"allOf\": [\n   \
  \     {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"instanceState\"\n          },\n          \"description\": \"The state of the EC2 instance.\"\n        }\n      ]\n    },\n    \"InstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"instanceType\"\n          },\n          \"description\": \"The type of the EC2 instance.\"\n        }\n      ]\n    },\n    \"OutpostArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outpostArn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) of the Amazon Web Services Outpost. Only applicable to Amazon Web Services Outposts instances.\"\n        }\n      ]\n    },\n    \"LaunchTime\": {\n      \"allOf\": [\n        {\n    \
  \      \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"launchTime\"\n          },\n          \"description\": \"The launch time of the EC2 instance.\"\n        }\n      ]\n    },\n    \"NetworkInterfaces\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkInterfaces\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkInterfaces\"\n          },\n          \"description\": \"The elastic network interface information of the EC2 instance.\"\n        }\n      ]\n    },\n    \"Platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"platform\"\n          },\n          \"description\": \"The platform of the EC2 instance.\"\n        }\n      ]\n    },\n    \"ProductCodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProductCodes\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"productCodes\"\n          },\n          \"description\": \"The product code of the EC2 instance.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The tags of the EC2 instance.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-instance-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: InstanceDetails
---
