---
description: The risk factor is represented numerically using a range from 0 (no risk data) to 5 (high risk). Each numerical value and its associated risk representation is shown below. * `0` - Represents an unknown risk because no data on this device is available. * `1` - Represents a no or low risk request. * `2` - Represents a low risk request. * `3` - Represents a medium risk request. * `4` - Represents a high risk request. * `5` - Represents a very high risk request. The risk factor is typically used to identify scenarios where a service provider may want to introduce consumer friction on the authorization process to validate the identity of the consumer. Example usage by a service provider may be to implement controls such as multifactor authentication for calculated risk factors of `3` or `4` and request blocking for risk factors of `5`.
layout: schema
name: RiskFactor
properties_list: []
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-identity-insights-for-transactions-risk-factor-schema.json
slug: mastercard-identity-insights-for-transactions-risk-factor
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RiskFactor\",\n  \"type\": \"integer\",\n  \"description\": \"The risk factor is represented numerically using a range from 0 (no risk data) to 5 (high risk). Each numerical value and its associated risk representation is shown below.\\n* `0` - Represents an unknown risk because no data on this device is available.\\n* `1` - Represents a no or low risk request.\\n* `2` - Represents a low risk request.\\n* `3` - Represents a medium risk request.\\n* `4` - Represents a high risk request.\\n* `5` - Represents a very high risk request.\\n\\nThe risk factor is typically used to identify scenarios where a service provider may want to introduce consumer friction on the authorization process to validate the identity of the consumer. Example usage by a service provider may be to implement controls such as multifactor authentication for calculated risk factors of `3` or `4` and request blocking for risk\
  \ factors of `5`.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-identity-insights-for-transactions-risk-factor-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: RiskFactor
---
