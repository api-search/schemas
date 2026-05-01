---
description: 'The frequency with which Amazon Macie publishes updates to policy findings for an account. This includes publishing updates to Security Hub and Amazon EventBridge (formerly Amazon CloudWatch Events). For more information, see <a href="https://docs.aws.amazon.com/macie/latest/user/findings-monitor.html">Monitoring and processing findings</a> in the <i>Amazon Macie User Guide</i>. Valid values are:'
layout: schema
name: FindingPublishingFrequency
properties_list: []
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-finding-publishing-frequency-schema.json
slug: amazon-macie-finding-publishing-frequency
source_filename: amazon-macie-finding-publishing-frequency-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-finding-publishing-frequency-schema.json\",\n  \"title\": \"FindingPublishingFrequency\",\n  \"description\": \"The frequency with which Amazon Macie publishes updates to policy findings for an account. This includes publishing updates to Security Hub and Amazon EventBridge (formerly Amazon CloudWatch Events). For more information, see <a href=\\\"https://docs.aws.amazon.com/macie/latest/user/findings-monitor.html\\\">Monitoring and processing findings</a> in the <i>Amazon Macie User Guide</i>. Valid values are:\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"FIFTEEN_MINUTES\",\n    \"ONE_HOUR\",\n    \"SIX_HOURS\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-finding-publishing-frequency-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: FindingPublishingFrequency
---
