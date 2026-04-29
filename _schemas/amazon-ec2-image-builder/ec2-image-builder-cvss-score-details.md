---
description: Details about the source of the score, and the factors that determined the adjustments to create the final score.
layout: schema
name: CvssScoreDetails
properties_list:
- description: ''
  name: scoreSource
  type: object
- description: ''
  name: cvssSource
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: score
  type: object
- description: ''
  name: scoringVector
  type: object
- description: ''
  name: adjustments
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-cvss-score-details-schema.json
slug: ec2-image-builder-cvss-score-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-cvss-score-details-schema.json\",\n  \"title\": \"CvssScoreDetails\",\n  \"description\": \"Details about the source of the score, and the factors that determined the adjustments to create the final score.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scoreSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The source for the CVSS score.\"\n        }\n      ]\n    },\n    \"cvssSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The source of the finding.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\
  \n        },\n        {\n          \"description\": \"The CVSS version that generated the score.\"\n        }\n      ]\n    },\n    \"score\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonNegativeDouble\"\n        },\n        {\n          \"description\": \"The CVSS score.\"\n        }\n      ]\n    },\n    \"scoringVector\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"A vector that measures the severity of the vulnerability.\"\n        }\n      ]\n    },\n    \"adjustments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CvssScoreAdjustmentList\"\n        },\n        {\n          \"description\": \"An object that contains details about an adjustment that Amazon Inspector made to the CVSS score for the finding.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-cvss-score-details-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: CvssScoreDetails
---
