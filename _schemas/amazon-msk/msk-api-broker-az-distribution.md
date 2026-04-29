---
description: <p>The distribution of broker nodes across Availability Zones. This is an optional parameter. If you don't specify it, Amazon MSK gives it the value DEFAULT. You can also explicitly set this parameter to the value DEFAULT. No other values are currently allowed.</p> <p>Amazon MSK distributes the broker nodes evenly across the Availability Zones that correspond to the subnets you provide when you create the cluster.</p>
layout: schema
name: BrokerAZDistribution
properties_list: []
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-broker-az-distribution-schema.json
slug: msk-api-broker-az-distribution
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-broker-az-distribution-schema.json\",\n  \"title\": \"BrokerAZDistribution\",\n  \"description\": \"\\n            <p>The distribution of broker nodes across Availability Zones. This is an optional parameter. If you don't specify it, Amazon MSK gives it the value DEFAULT. You can also explicitly set this parameter to the value DEFAULT. No other values are currently allowed.</p>\\n         <p>Amazon MSK distributes the broker nodes evenly across the Availability Zones that correspond to the subnets you provide when you create the cluster.</p>\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"DEFAULT\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-broker-az-distribution-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BrokerAZDistribution
---
