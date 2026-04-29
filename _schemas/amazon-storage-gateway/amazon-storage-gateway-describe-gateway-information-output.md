---
description: 'A JSON object containing the following fields:'
layout: schema
name: DescribeGatewayInformationOutput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: GatewayId
  type: object
- description: ''
  name: GatewayName
  type: object
- description: ''
  name: GatewayTimezone
  type: object
- description: ''
  name: GatewayState
  type: object
- description: ''
  name: GatewayNetworkInterfaces
  type: object
- description: ''
  name: GatewayType
  type: object
- description: ''
  name: NextUpdateAvailabilityDate
  type: object
- description: ''
  name: LastSoftwareUpdate
  type: object
- description: ''
  name: Ec2InstanceId
  type: object
- description: ''
  name: Ec2InstanceRegion
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: VPCEndpoint
  type: object
- description: ''
  name: CloudWatchLogGroupARN
  type: object
- description: ''
  name: HostEnvironment
  type: object
- description: ''
  name: EndpointType
  type: object
- description: ''
  name: SoftwareUpdatesEndDate
  type: object
- description: ''
  name: DeprecationDate
  type: object
- description: ''
  name: GatewayCapacity
  type: object
- description: ''
  name: SupportedGatewayCapacities
  type: object
- description: ''
  name: HostEnvironmentId
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-gateway-information-output-schema.json
slug: amazon-storage-gateway-describe-gateway-information-output
source_filename: amazon-storage-gateway-describe-gateway-information-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-gateway-information-output-schema.json\",\n  \"title\": \"DescribeGatewayInformationOutput\",\n  \"description\": \"A JSON object containing the following fields:\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"GatewayId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayId\"\n        },\n        {\n          \"description\": \"The unique identifier assigned to your gateway during activation. This ID becomes part of the gateway Amazon Resource Name (ARN), which you use as input for other operations.\"\n        }\n      ]\n    },\n    \"GatewayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n \
  \       },\n        {\n          \"description\": \"The name you configured for your gateway.\"\n        }\n      ]\n    },\n    \"GatewayTimezone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayTimezone\"\n        },\n        {\n          \"description\": \"A value that indicates the time zone configured for the gateway.\"\n        }\n      ]\n    },\n    \"GatewayState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayState\"\n        },\n        {\n          \"description\": \"A value that indicates the operating state of the gateway.\"\n        }\n      ]\n    },\n    \"GatewayNetworkInterfaces\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayNetworkInterfaces\"\n        },\n        {\n          \"description\": \"A <a>NetworkInterface</a> array that contains descriptions of the gateway network interfaces.\"\n        }\n      ]\n    },\n    \"GatewayType\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayType\"\n        },\n        {\n          \"description\": \"The type of the gateway.\"\n        }\n      ]\n    },\n    \"NextUpdateAvailabilityDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextUpdateAvailabilityDate\"\n        },\n        {\n          \"description\": \"The date on which an update to the gateway is available. This date is in the time zone of the gateway. If the gateway is not available for an update this field is not returned in the response.\"\n        }\n      ]\n    },\n    \"LastSoftwareUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastSoftwareUpdate\"\n        },\n        {\n          \"description\": \"The date on which the last software update was applied to the gateway. If the gateway has never been updated, this field does not return a value in the response. This only only exist and returns once it have been\
  \ chosen and set by the SGW service, based on the OS version of the gateway VM\"\n        }\n      ]\n    },\n    \"Ec2InstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ec2InstanceId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon EC2 instance that was used to launch the gateway.\"\n        }\n      ]\n    },\n    \"Ec2InstanceRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ec2InstanceRegion\"\n        },\n        {\n          \"description\": \"The Amazon Web Services Region where the Amazon EC2 instance is located.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"A list of up to 50 tags assigned to the gateway, sorted alphabetically by key name. Each tag is a key-value pair. For a gateway with more than 10 tags assigned, you can view all tags using\
  \ the <code>ListTagsForResource</code> API operation.\"\n        }\n      ]\n    },\n    \"VPCEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The configuration settings for the virtual private cloud (VPC) endpoint for your gateway.\"\n        }\n      ]\n    },\n    \"CloudWatchLogGroupARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudWatchLogGroupARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Amazon CloudWatch log group that is used to monitor events in the gateway. This field only only exist and returns once it have been chosen and set by the SGW service, based on the OS version of the gateway VM\"\n        }\n      ]\n    },\n    \"HostEnvironment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HostEnvironment\"\n        },\n        {\n          \"description\":\
  \ \"The type of hardware or software platform on which the gateway is running.\"\n        }\n      ]\n    },\n    \"EndpointType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointType\"\n        },\n        {\n          \"description\": \"<p>The type of endpoint for your gateway.</p> <p>Valid Values: <code>STANDARD</code> | <code>FIPS</code> </p>\"\n        }\n      ]\n    },\n    \"SoftwareUpdatesEndDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SoftwareUpdatesEndDate\"\n        },\n        {\n          \"description\": \"Date after which this gateway will not receive software updates for new features.\"\n        }\n      ]\n    },\n    \"DeprecationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeprecationDate\"\n        },\n        {\n          \"description\": \"Date after which this gateway will not receive software updates for new features and bug fixes.\"\n        }\n\
  \      ]\n    },\n    \"GatewayCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayCapacity\"\n        },\n        {\n          \"description\": \"Specifies the size of the gateway's metadata cache.\"\n        }\n      ]\n    },\n    \"SupportedGatewayCapacities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SupportedGatewayCapacities\"\n        },\n        {\n          \"description\": \"A list of the metadata cache sizes that the gateway can support based on its current hardware specifications.\"\n        }\n      ]\n    },\n    \"HostEnvironmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HostEnvironmentId\"\n        },\n        {\n          \"description\": \"A unique identifier for the specific instance of the host platform running the gateway. This value is only available for certain host environments, and its format depends on the host environment type.\"\n        }\n\
  \      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-gateway-information-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeGatewayInformationOutput
---
