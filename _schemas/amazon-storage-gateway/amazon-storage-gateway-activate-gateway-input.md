---
description: <p>A JSON object containing one or more of the following fields:</p> <ul> <li> <p> <a>ActivateGatewayInput$ActivationKey</a> </p> </li> <li> <p> <a>ActivateGatewayInput$GatewayName</a> </p> </li> <li> <p> <a>ActivateGatewayInput$GatewayRegion</a> </p> </li> <li> <p> <a>ActivateGatewayInput$GatewayTimezone</a> </p> </li> <li> <p> <a>ActivateGatewayInput$GatewayType</a> </p> </li> <li> <p> <a>ActivateGatewayInput$MediumChangerType</a> </p> </li> <li> <p> <a>ActivateGatewayInput$TapeDriveType</a> </p> </li> </ul>
layout: schema
name: ActivateGatewayInput
properties_list:
- description: ''
  name: ActivationKey
  type: object
- description: ''
  name: GatewayName
  type: object
- description: ''
  name: GatewayTimezone
  type: object
- description: ''
  name: GatewayRegion
  type: object
- description: ''
  name: GatewayType
  type: object
- description: ''
  name: TapeDriveType
  type: object
- description: ''
  name: MediumChangerType
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-activate-gateway-input-schema.json
slug: amazon-storage-gateway-activate-gateway-input
source_filename: amazon-storage-gateway-activate-gateway-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-activate-gateway-input-schema.json\",\n  \"title\": \"ActivateGatewayInput\",\n  \"description\": \"<p>A JSON object containing one or more of the following fields:</p> <ul> <li> <p> <a>ActivateGatewayInput$ActivationKey</a> </p> </li> <li> <p> <a>ActivateGatewayInput$GatewayName</a> </p> </li> <li> <p> <a>ActivateGatewayInput$GatewayRegion</a> </p> </li> <li> <p> <a>ActivateGatewayInput$GatewayTimezone</a> </p> </li> <li> <p> <a>ActivateGatewayInput$GatewayType</a> </p> </li> <li> <p> <a>ActivateGatewayInput$MediumChangerType</a> </p> </li> <li> <p> <a>ActivateGatewayInput$TapeDriveType</a> </p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActivationKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivationKey\"\n\
  \        },\n        {\n          \"description\": \"<p>Your gateway activation key. You can obtain the activation key by sending an HTTP GET request with redirects enabled to the gateway IP address (port 80). The redirect URL returned in the response provides you the activation key for your gateway in the query string parameter <code>activationKey</code>. It may also include other activation-related parameters, however, these are merely defaults -- the arguments you pass to the <code>ActivateGateway</code> API call determine the actual configuration of your gateway.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/storagegateway/latest/userguide/get-activation-key.html\\\">Getting activation key</a> in the <i>Storage Gateway User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"GatewayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayName\"\n        },\n        {\n          \"description\": \"The name you configured\
  \ for your gateway.\"\n        }\n      ]\n    },\n    \"GatewayTimezone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayTimezone\"\n        },\n        {\n          \"description\": \"A value that indicates the time zone you want to set for the gateway. The time zone is of the format \\\"GMT-hr:mm\\\" or \\\"GMT+hr:mm\\\". For example, GMT-4:00 indicates the time is 4 hours behind GMT. GMT+2:00 indicates the time is 2 hours ahead of GMT. The time zone is used, for example, for scheduling snapshots and your gateway's maintenance schedule.\"\n        }\n      ]\n    },\n    \"GatewayRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegionId\"\n        },\n        {\n          \"description\": \"<p>A value that indicates the Amazon Web Services Region where you want to store your data. The gateway Amazon Web Services Region specified must be the same Amazon Web Services Region as the Amazon Web Services Region in\
  \ your <code>Host</code> header in the request. For more information about available Amazon Web Services Regions and endpoints for Storage Gateway, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/sg.html\\\"> Storage Gateway endpoints and quotas</a> in the <i>Amazon Web Services General Reference</i>.</p> <p>Valid Values: See <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/sg.html\\\"> Storage Gateway endpoints and quotas</a> in the <i>Amazon Web Services General Reference</i>. </p>\"\n        }\n      ]\n    },\n    \"GatewayType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayType\"\n        },\n        {\n          \"description\": \"<p>A value that defines the type of gateway to activate. The type specified is critical to all later functions of the gateway and cannot be changed after activation. The default value is <code>CACHED</code>.</p> <p>Valid Values: <code>STORED</code> | <code>CACHED</code> | <code>VTL</code> |\
  \ <code>VTL_SNOW</code> | <code>FILE_S3</code> | <code>FILE_FSX_SMB</code> </p>\"\n        }\n      ]\n    },\n    \"TapeDriveType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeDriveType\"\n        },\n        {\n          \"description\": \"<p>The value that indicates the type of tape drive to use for tape gateway. This field is optional.</p> <p>Valid Values: <code>IBM-ULT3580-TD5</code> </p>\"\n        }\n      ]\n    },\n    \"MediumChangerType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MediumChangerType\"\n        },\n        {\n          \"description\": \"<p>The value that indicates the type of medium changer to use for tape gateway. This field is optional.</p> <p>Valid Values: <code>STK-L700</code> | <code>AWS-Gateway-VTL</code> | <code>IBM-03584L32-0402</code> </p>\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n\
  \        {\n          \"description\": \"<p>A list of up to 50 tags that you can assign to the gateway. Each tag is a key-value pair.</p> <note> <p>Valid characters for key and value are letters, spaces, and numbers that can be represented in UTF-8 format, and the following special characters: + - = . _ : / @. The maximum length of a tag's key is 128 characters, and the maximum length for a tag's value is 256 characters.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ActivationKey\",\n    \"GatewayName\",\n    \"GatewayTimezone\",\n    \"GatewayRegion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-activate-gateway-input-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: ActivateGatewayInput
---
