---
description: UpdatePublishingDestinationRequest schema from Amazon GuardDuty API
layout: schema
name: UpdatePublishingDestinationRequest
properties_list:
- description: ''
  name: DestinationProperties
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-update-publishing-destination-request-schema.json
slug: guardduty-update-publishing-destination-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-update-publishing-destination-request-schema.json\",\n  \"title\": \"UpdatePublishingDestinationRequest\",\n  \"description\": \"UpdatePublishingDestinationRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DestinationProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationProperties\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationProperties\"\n          },\n          \"description\": \"A <code>DestinationProperties</code> object that includes the <code>DestinationArn</code> and <code>KmsKeyArn</code> of the publishing destination.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-update-publishing-destination-request-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: UpdatePublishingDestinationRequest
---
