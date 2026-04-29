---
description: UpdateJobRequest schema from Amazon Snow Family API
layout: schema
name: UpdateJobRequest
properties_list:
- description: ''
  name: JobId
  type: object
- description: ''
  name: RoleARN
  type: object
- description: ''
  name: Notification
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
  name: Description
  type: object
- description: ''
  name: SnowballCapacityPreference
  type: object
- description: ''
  name: ForwardingAddressId
  type: object
- description: ''
  name: PickupDetails
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-update-job-request-schema.json
slug: amazon-snow-family-update-job-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-update-job-request-schema.json\",\n  \"title\": \"UpdateJobRequest\",\n  \"description\": \"UpdateJobRequest schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The job ID of the job that you want to update, for example <code>JID123e4567-e89b-12d3-a456-426655440000</code>.\"\n        }\n      ]\n    },\n    \"RoleARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleARN\"\n        },\n        {\n          \"description\": \"The new role Amazon Resource Name (ARN) that you want to associate with this job. To create a role ARN, use the <a href=\\\"https://docs.aws.amazon.com/IAM/latest/APIReference/API_CreateRole.html\\\
  \">CreateRole</a>Identity and Access Management (IAM) API action.\"\n        }\n      ]\n    },\n    \"Notification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Notification\"\n        },\n        {\n          \"description\": \"The new or updated <a>Notification</a> object.\"\n        }\n      ]\n    },\n    \"Resources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobResource\"\n        },\n        {\n          \"description\": \"The updated <code>JobResource</code> object, or the updated <a>JobResource</a> object. \"\n        }\n      ]\n    },\n    \"OnDeviceServiceConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OnDeviceServiceConfiguration\"\n        },\n        {\n          \"description\": \"Specifies the service or services on the Snow Family device that your transferred data will be exported from or imported into. Amazon Web Services Snow Family supports Amazon S3\
  \ and NFS (Network File System) and the Amazon Web Services Storage Gateway service Tape Gateway type.\"\n        }\n      ]\n    },\n    \"AddressId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressId\"\n        },\n        {\n          \"description\": \"The ID of the updated <a>Address</a> object.\"\n        }\n      ]\n    },\n    \"ShippingOption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShippingOption\"\n        },\n        {\n          \"description\": \"The updated shipping option value of this job's <a>ShippingDetails</a> object.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The updated description of this job's <a>JobMetadata</a> object.\"\n        }\n      ]\n    },\n    \"SnowballCapacityPreference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/SnowballCapacity\"\n        },\n        {\n          \"description\": \"<p>The updated <code>SnowballCapacityPreference</code> of this job's <a>JobMetadata</a> object. The 50 TB Snowballs are only available in the US regions.</p> <p>For more information, see \\\"https://docs.aws.amazon.com/snowball/latest/snowcone-guide/snow-device-types.html\\\" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i> or \\\"https://docs.aws.amazon.com/snowball/latest/developer-guide/snow-device-types.html\\\" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"ForwardingAddressId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressId\"\n        },\n        {\n          \"description\": \"The updated ID for the forwarding address for a job. This field is not supported in most regions.\"\n        }\n      ]\n    },\n    \"PickupDetails\": {\n      \"$ref\": \"#/components/schemas/PickupDetails\"\
  \n    }\n  },\n  \"required\": [\n    \"JobId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-update-job-request-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: UpdateJobRequest
---
