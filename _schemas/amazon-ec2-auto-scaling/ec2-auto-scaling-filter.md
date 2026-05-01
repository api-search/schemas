---
description: <p>Describes a filter that is used to return a more specific list of results from a describe operation.</p> <p>If you specify multiple filters, the filters are automatically logically joined with an <code>AND</code>, and the request returns only the results that match all of the specified filters. </p> <p>For more information, see <a href="https://docs.aws.amazon.com/autoscaling/ec2/userguide/ec2-auto-scaling-tagging.html">Tag Auto Scaling groups and instances</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>
layout: schema
name: Filter
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Values
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-filter-schema.json
slug: ec2-auto-scaling-filter
source_filename: ec2-auto-scaling-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-filter-schema.json\",\n  \"title\": \"Filter\",\n  \"description\": \"<p>Describes a filter that is used to return a more specific list of results from a describe operation.</p> <p>If you specify multiple filters, the filters are automatically logically joined with an <code>AND</code>, and the request returns only the results that match all of the specified filters. </p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/ec2-auto-scaling-tagging.html\\\">Tag Auto Scaling groups and instances</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"\
  description\": \"<p>The name of the filter.</p> <p>The valid values for <code>Name</code> depend on which API operation you're using with the filter (<a>DescribeAutoScalingGroups</a> or <a>DescribeTags</a>).</p> <p> <b>DescribeAutoScalingGroups</b> </p> <p>Valid values for <code>Name</code> include the following: </p> <ul> <li> <p> <code>tag-key</code> - Accepts tag keys. The results only include information about the Auto Scaling groups associated with these tag keys. </p> </li> <li> <p> <code>tag-value</code> - Accepts tag values. The results only include information about the Auto Scaling groups associated with these tag values. </p> </li> <li> <p> <code>tag:&lt;key&gt;</code> - Accepts the key/value combination of the tag. Use the tag key in the filter name and the tag value as the filter value. The results only include information about the Auto Scaling groups associated with the specified key/value combination. </p> </li> </ul> <p> <b>DescribeTags</b> </p> <p>Valid values for <code>Name</code>\
  \ include the following: </p> <ul> <li> <p> <code>auto-scaling-group</code> - Accepts the names of Auto Scaling groups. The results only include information about the tags associated with these Auto Scaling groups. </p> </li> <li> <p> <code>key</code> - Accepts tag keys. The results only include information about the tags associated with these tag keys. </p> </li> <li> <p> <code>value</code> - Accepts tag values. The results only include information about the tags associated with these tag values. </p> </li> <li> <p> <code>propagate-at-launch</code> - Accepts a Boolean value, which specifies whether tags propagate to instances at launch. The results only include information about the tags associated with the specified Boolean value. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Values\"\n        },\n        {\n          \"description\": \"<p>One or more filter values. Filter values are case-sensitive.\
  \ </p> <p>If you specify multiple values for a filter, the values are automatically logically joined with an <code>OR</code>, and the request returns all results that match any of the specified values. For example, specify \\\"tag:environment\\\" for the filter name and \\\"production,development\\\" for the filter values to find Auto Scaling groups with the tag \\\"environment=production\\\" or \\\"environment=development\\\".</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-filter-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: Filter
---
