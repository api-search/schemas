---
description: Contains details for a gateway that runs on IoT Greengrass. To create a gateway that runs on IoT Greengrass, you must add the IoT SiteWise connector to a Greengrass group and deploy it. Your Greengrass group must also have permissions to upload data to IoT SiteWise. For more information, see <a href="https://docs.aws.amazon.com/iot-sitewise/latest/userguide/gateway-connector.html">Ingesting data using a gateway</a> in the <i>IoT SiteWise User Guide</i>.
layout: schema
name: Greengrass
properties_list:
- description: ''
  name: groupArn
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-greengrass-schema.json
slug: iot-sitewise-greengrass
source_filename: iot-sitewise-greengrass-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-greengrass-schema.json\",\n  \"title\": \"Greengrass\",\n  \"description\": \"Contains details for a gateway that runs on IoT Greengrass. To create a gateway that runs on IoT Greengrass, you must add the IoT SiteWise connector to a Greengrass group and deploy it. Your Greengrass group must also have permissions to upload data to IoT SiteWise. For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/userguide/gateway-connector.html\\\">Ingesting data using a gateway</a> in the <i>IoT SiteWise User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"groupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\
  \">ARN</a> of the Greengrass group. For more information about how to find a group's ARN, see <a href=\\\"https://docs.aws.amazon.com/greengrass/latest/apireference/listgroups-get.html\\\">ListGroups</a> and <a href=\\\"https://docs.aws.amazon.com/greengrass/latest/apireference/getgroup-get.html\\\">GetGroup</a> in the <i>IoT Greengrass API Reference</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"groupArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-greengrass-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: Greengrass
---
