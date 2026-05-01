---
description: '<p>The severity to assign to findings that the custom data identifier produces, based on the number of occurrences of text that matches the custom data identifier''s detection criteria. You can specify as many as three SeverityLevel objects in this array, one for each severity: LOW, MEDIUM, or HIGH. If you specify more than one, the occurrences thresholds must be in ascending order by severity, moving from LOW to HIGH. For example, 1 for LOW, 50 for MEDIUM, and 100 for HIGH. If an S3 object contains fewer occurrences than the lowest specified threshold, Amazon Macie doesn''t create a finding.</p> <p>If you don''t specify any values for this array, Macie creates findings for S3 objects that contain at least one occurrence of text that matches the detection criteria, and Macie automatically assigns the MEDIUM severity to those findings.</p>'
layout: schema
name: SeverityLevelList
properties_list: []
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-severity-level-list-schema.json
slug: amazon-macie-severity-level-list
source_filename: amazon-macie-severity-level-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-severity-level-list-schema.json\",\n  \"title\": \"SeverityLevelList\",\n  \"description\": \"<p>The severity to assign to findings that the custom data identifier produces, based on the number of occurrences of text that matches the custom data identifier's detection criteria. You can specify as many as three SeverityLevel objects in this array, one for each severity: LOW, MEDIUM, or HIGH. If you specify more than one, the occurrences thresholds must be in ascending order by severity, moving from LOW to HIGH. For example, 1 for LOW, 50 for MEDIUM, and 100 for HIGH. If an S3 object contains fewer occurrences than the lowest specified threshold, Amazon Macie doesn't create a finding.</p> <p>If you don't specify any values for this array, Macie creates findings for S3 objects that contain at least\
  \ one occurrence of text that matches the detection criteria, and Macie automatically assigns the MEDIUM severity to those findings.</p>\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/SeverityLevel\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-severity-level-list-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SeverityLevelList
---
