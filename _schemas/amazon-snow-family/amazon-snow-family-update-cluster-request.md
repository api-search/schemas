---
description: UpdateClusterRequest schema from Amazon Snow Family API
layout: schema
name: UpdateClusterRequest
properties_list:
- description: ''
  name: ClusterId
  type: object
- description: ''
  name: RoleARN
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Resources
  type: object
- description: ''
  name: OnDeviceServiceConfiguration
  type: object
- description: ''
  name: AddressId
  type: object
- description: ''
  name: ShippingOption
  type: object
- description: ''
  name: Notification
  type: object
- description: ''
  name: ForwardingAddressId
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-update-cluster-request-schema.json
slug: amazon-snow-family-update-cluster-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-update-cluster-request-schema.json\",\n  \"title\": \"UpdateClusterRequest\",\n  \"description\": \"UpdateClusterRequest schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClusterId\"\n        },\n        {\n          \"description\": \"The cluster ID of the cluster that you want to update, for example <code>CID123e4567-e89b-12d3-a456-426655440000</code>.\"\n        }\n      ]\n    },\n    \"RoleARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleARN\"\n        },\n        {\n          \"description\": \"The new role Amazon Resource Name (ARN) that you want to associate with this cluster. To create a role ARN, use the\
  \ <a href=\\\"https://docs.aws.amazon.com/IAM/latest/APIReference/API_CreateRole.html\\\">CreateRole</a> API action in Identity and Access Management (IAM).\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The updated description of this cluster.\"\n        }\n      ]\n    },\n    \"Resources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobResource\"\n        },\n        {\n          \"description\": \"The updated arrays of <a>JobResource</a> objects that can include updated <a>S3Resource</a> objects or <a>LambdaResource</a> objects.\"\n        }\n      ]\n    },\n    \"OnDeviceServiceConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OnDeviceServiceConfiguration\"\n        },\n        {\n          \"description\": \"Specifies the service or services on the Snow Family\
  \ device that your transferred data will be exported from or imported into. Amazon Web Services Snow Family device clusters support Amazon S3 and NFS (Network File System).\"\n        }\n      ]\n    },\n    \"AddressId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressId\"\n        },\n        {\n          \"description\": \"The ID of the updated <a>Address</a> object.\"\n        }\n      ]\n    },\n    \"ShippingOption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShippingOption\"\n        },\n        {\n          \"description\": \"The updated shipping option value of this cluster's <a>ShippingDetails</a> object.\"\n        }\n      ]\n    },\n    \"Notification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Notification\"\n        },\n        {\n          \"description\": \"The new or updated <a>Notification</a> object.\"\n        }\n      ]\n    },\n    \"ForwardingAddressId\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressId\"\n        },\n        {\n          \"description\": \"The updated ID for the forwarding address for a cluster. This field is not supported in most regions.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ClusterId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-update-cluster-request-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: UpdateClusterRequest
---
