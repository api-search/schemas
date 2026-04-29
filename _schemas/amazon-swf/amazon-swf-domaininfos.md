---
description: Contains a paginated collection of DomainInfo structures.
layout: schema
name: DomainInfos
properties_list:
- description: ''
  name: domainInfos
  type: object
- description: ''
  name: nextPageToken
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-domaininfos-schema.json
slug: amazon-swf-domaininfos
source_filename: amazon-swf-domaininfos-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"domainInfos\"\n  ],\n  \"properties\": {\n    \"domainInfos\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainInfoList\"\n        },\n        {\n          \"description\": \"A list of DomainInfo structures.\"\n        }\n      ]\n    },\n    \"nextPageToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageToken\"\n        },\n        {\n          \"description\": \"<p>If a <code>NextPageToken</code> was returned by a previous call, there are more results available. To retrieve the next page of results, make the call again using the returned token in <code>nextPageToken</code>. Keep all other arguments unchanged.</p> <p>The configured <code>maximumPageSize</code> determines how many results can be returned in a single call.</p>\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Contains a paginated collection of DomainInfo structures.\",\n  \"$schema\"\
  : \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DomainInfos\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-domaininfos-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: DomainInfos
---
