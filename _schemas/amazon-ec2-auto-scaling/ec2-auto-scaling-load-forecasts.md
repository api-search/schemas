---
description: LoadForecasts schema from Auto Scaling
layout: schema
name: LoadForecasts
properties_list: []
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-load-forecasts-schema.json
slug: ec2-auto-scaling-load-forecasts
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-load-forecasts-schema.json\",\n  \"title\": \"LoadForecasts\",\n  \"description\": \"LoadForecasts schema from Auto Scaling\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/LoadForecast\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-load-forecasts-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: LoadForecasts
---
