---
description: DescribeConfigurationAggregatorSourcesStatusRequest schema
layout: schema
name: DescribeConfigurationAggregatorSourcesStatusRequest
properties_list:
- description: ''
  name: ConfigurationAggregatorName
  type: object
- description: ''
  name: UpdateStatus
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Limit
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-describe-configuration-aggregator-sources-status-request-schema.json
slug: config-describe-configuration-aggregator-sources-status-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-configuration-aggregator-sources-status-request-schema.json\",\n  \"title\": \"DescribeConfigurationAggregatorSourcesStatusRequest\",\n  \"description\": \"DescribeConfigurationAggregatorSourcesStatusRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationAggregatorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationAggregatorName\"\n        },\n        {\n          \"description\": \"The name of the configuration aggregator.\"\n        }\n      ]\n    },\n    \"UpdateStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregatedSourceStatusTypeList\"\n        },\n        {\n          \"description\": \"<p>Filters the status type.</p> <ul> <li> <p>Valid value FAILED indicates errors\
  \ while moving data.</p> </li> <li> <p>Valid value SUCCEEDED indicates the data was successfully moved.</p> </li> <li> <p>Valid value OUTDATED indicates the data is not the most recent.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The maximum number of AggregatorSourceStatus returned on each page. The default is maximum. If you specify 0, Config uses the default.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigurationAggregatorName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-describe-configuration-aggregator-sources-status-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DescribeConfigurationAggregatorSourcesStatusRequest
---
