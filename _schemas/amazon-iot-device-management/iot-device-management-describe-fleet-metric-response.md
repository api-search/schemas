---
description: DescribeFleetMetricResponse schema
layout: schema
name: DescribeFleetMetricResponse
properties_list:
- description: ''
  name: metricName
  type: object
- description: ''
  name: queryString
  type: object
- description: ''
  name: aggregationType
  type: object
- description: ''
  name: period
  type: object
- description: ''
  name: aggregationField
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: queryVersion
  type: object
- description: ''
  name: indexName
  type: object
- description: ''
  name: creationDate
  type: object
- description: ''
  name: lastModifiedDate
  type: object
- description: ''
  name: unit
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: metricArn
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-describe-fleet-metric-response-schema.json
slug: iot-device-management-describe-fleet-metric-response
source_filename: iot-device-management-describe-fleet-metric-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-fleet-metric-response-schema.json\",\n  \"title\": \"DescribeFleetMetricResponse\",\n  \"description\": \"DescribeFleetMetricResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metricName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetMetricName\"\n        },\n        {\n          \"description\": \"The name of the fleet metric to describe.\"\n        }\n      ]\n    },\n    \"queryString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryString\"\n        },\n        {\n          \"description\": \"The search query string.\"\n        }\n      ]\n    },\n    \"aggregationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregationType\"\
  \n        },\n        {\n          \"description\": \"The type of the aggregation query.\"\n        }\n      ]\n    },\n    \"period\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetMetricPeriod\"\n        },\n        {\n          \"description\": \"The time in seconds between fleet metric emissions. Range [60(1 min), 86400(1 day)] and must be multiple of 60.\"\n        }\n      ]\n    },\n    \"aggregationField\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregationField\"\n        },\n        {\n          \"description\": \"The field to aggregate.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetMetricDescription\"\n        },\n        {\n          \"description\": \"The fleet metric description.\"\n        }\n      ]\n    },\n    \"queryVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryVersion\"\
  \n        },\n        {\n          \"description\": \"The query version.\"\n        }\n      ]\n    },\n    \"indexName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IndexName\"\n        },\n        {\n          \"description\": \"The name of the index to search.\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreationDate\"\n        },\n        {\n          \"description\": \"The date when the fleet metric is created.\"\n        }\n      ]\n    },\n    \"lastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastModifiedDate\"\n        },\n        {\n          \"description\": \"The date when the fleet metric is last modified.\"\n        }\n      ]\n    },\n    \"unit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetMetricUnit\"\n        },\n        {\n          \"description\": \"Used to support\
  \ unit transformation such as milliseconds to seconds. The unit must be supported by <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_MetricDatum.html\\\">CW metric</a>.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The version of the fleet metric.\"\n        }\n      ]\n    },\n    \"metricArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetMetricArn\"\n        },\n        {\n          \"description\": \"The ARN of the fleet metric to describe.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-fleet-metric-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: DescribeFleetMetricResponse
---
