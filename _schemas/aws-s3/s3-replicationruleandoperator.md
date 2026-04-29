---
description: <p>A container for specifying rule filters. The filters determine the subset of objects to which the rule applies. This element is required only if you specify more than one filter. </p> <p>For example:</p> <ul> <li> <p>If you specify both a <code>Prefix</code> and a <code>Tag</code> filter, wrap these filters in an <code>And</code> tag. </p> </li> <li> <p>If you specify a filter based on multiple tags, wrap the <code>Tag</code> elements in an <code>And</code> tag.</p> </li> </ul>
layout: schema
name: ReplicationRuleAndOperator
properties_list:
- description: ''
  name: Prefix
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-replicationruleandoperator-schema.json
slug: s3-replicationruleandoperator
source_filename: s3-replicationruleandoperator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReplicationRuleAndOperator\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Prefix\": {},\n    \"Tags\": {}\n  },\n  \"description\": \"<p>A container for specifying rule filters. The filters determine the subset of objects to which the rule applies. This element is required only if you specify more than one filter. </p> <p>For example:</p> <ul> <li> <p>If you specify both a <code>Prefix</code> and a <code>Tag</code> filter, wrap these filters in an <code>And</code> tag. </p> </li> <li> <p>If you specify a filter based on multiple tags, wrap the <code>Tag</code> elements in an <code>And</code> tag.</p> </li> </ul>\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-replicationruleandoperator-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: ReplicationRuleAndOperator
---
