---
description: <p>The IAM resource that enables Amazon Web Services IoT FleetWise edge agent software to send data to Amazon Timestream. </p> <p>For more information, see <a href="https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html">IAM roles</a> in the <i>Identity and Access Management User Guide</i>.</p>
layout: schema
name: IamResources
properties_list:
- description: ''
  name: roleArn
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-iam-resources-schema.json
slug: iot-fleetwise-iam-resources
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-iam-resources-schema.json\",\n  \"title\": \"IamResources\",\n  \"description\": \"<p>The IAM resource that enables Amazon Web Services IoT FleetWise edge agent software to send data to Amazon Timestream. </p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html\\\">IAM roles</a> in the <i>Identity and Access Management User Guide</i>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IAMRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM resource that allows Amazon Web Services IoT FleetWise to send data to Amazon Timestream. For example, <code>arn:aws:iam::123456789012:role/SERVICE-ROLE-ARN</code>.\
  \ \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"roleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-iam-resources-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: IamResources
---
