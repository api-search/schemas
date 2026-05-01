---
description: JSON Schema representation of a single row in a FOCUS-conformant billing dataset. FOCUS (FinOps Open Cost and Usage Specification) is an open standard maintained under the FinOps Foundation that normalizes cost and usage data across cloud, SaaS, data center, and other technology vendors. This schema lists the normative columns defined by the FOCUS specification and reflects the column attributes (data type, nullability, requirement level) defined in the FOCUS data model. The full normative definitions live at https://focus.finops.org/ and in the FOCUS_Spec repository.
layout: schema
name: FOCUS Billing Record
properties_list:
- description: Provider-assigned identifier for an isolated location within a region.
  name: AvailabilityZone
  type:
  - string
  - 'null'
- description: Amount on the invoice for the billing period before amortization, in BillingCurrency.
  name: BilledCost
  type: number
- description: Provider-assigned identifier for the account that receives the invoice.
  name: BillingAccountId
  type: string
- description: Display name for the BillingAccountId.
  name: BillingAccountName
  type:
  - string
  - 'null'
- description: ISO 4217 currency code in which costs are denominated.
  name: BillingCurrency
  type: string
- description: Exclusive end of the billing period.
  name: BillingPeriodEnd
  type: string
- description: Inclusive start of the billing period.
  name: BillingPeriodStart
  type: string
- description: Highest-level classification of a charge.
  name: ChargeCategory
  type: string
- description: Indicates whether a charge represents a correction to a previously invoiced billing period.
  name: ChargeClass
  type:
  - string
  - 'null'
- description: Provider-supplied human-readable summary of the charge.
  name: ChargeDescription
  type:
  - string
  - 'null'
- description: Frequency at which a charge is incurred.
  name: ChargeFrequency
  type:
  - string
  - 'null'
- description: Exclusive end of the period over which the charge was incurred.
  name: ChargePeriodEnd
  type: string
- description: Inclusive start of the period over which the charge was incurred.
  name: ChargePeriodStart
  type: string
- description: Whether a commitment-based discount is denominated in spend or usage units.
  name: CommitmentDiscountCategory
  type:
  - string
  - 'null'
- description: Provider-assigned identifier for the commitment-based discount applied to the charge.
  name: CommitmentDiscountId
  type:
  - string
  - 'null'
- description: Display name for the CommitmentDiscountId.
  name: CommitmentDiscountName
  type:
  - string
  - 'null'
- description: Whether the commitment-based discount was used or unused for the charge.
  name: CommitmentDiscountStatus
  type:
  - string
  - 'null'
- description: Provider-defined type of commitment-based discount (e.g. Reserved Instance, Savings Plan).
  name: CommitmentDiscountType
  type:
  - string
  - 'null'
- description: Volume of a metered service consumed, in ConsumedUnit.
  name: ConsumedQuantity
  type:
  - number
  - 'null'
- description: Provider-defined unit of measurement for ConsumedQuantity.
  name: ConsumedUnit
  type:
  - string
  - 'null'
- description: Cost based on negotiated rates excluding negotiated discounts, in BillingCurrency.
  name: ContractedCost
  type: number
- description: Per-unit price at negotiated rates, in BillingCurrency per PricingUnit.
  name: ContractedUnitPrice
  type:
  - number
  - 'null'
- description: Amortized cost of the charge after applying upfront and recurring commitment fees, in BillingCurrency.
  name: EffectiveCost
  type: number
- description: Entity responsible for invoicing the consumer.
  name: InvoiceIssuerName
  type: string
- description: Cost based on public list prices, in BillingCurrency.
  name: ListCost
  type: number
- description: Per-unit price at public list rates, in BillingCurrency per PricingUnit.
  name: ListUnitPrice
  type:
  - number
  - 'null'
- description: Pricing model used to compute the cost of the charge.
  name: PricingCategory
  type:
  - string
  - 'null'
- description: Quantity priced for this charge, in PricingUnit.
  name: PricingQuantity
  type:
  - number
  - 'null'
- description: Provider-defined unit of measurement used for pricing.
  name: PricingUnit
  type:
  - string
  - 'null'
- description: Entity providing the resources or services.
  name: ProviderName
  type: string
- description: Entity that produced the resources or services.
  name: PublisherName
  type: string
- description: Provider-assigned identifier for an isolated geographic area.
  name: RegionId
  type:
  - string
  - 'null'
- description: Display name for the RegionId.
  name: RegionName
  type:
  - string
  - 'null'
- description: Provider-assigned identifier for a billable resource.
  name: ResourceId
  type:
  - string
  - 'null'
- description: Display name of the ResourceId.
  name: ResourceName
  type:
  - string
  - 'null'
- description: Provider-defined type of resource.
  name: ResourceType
  type:
  - string
  - 'null'
- description: FOCUS top-level service category (e.g. Compute, Storage, Networking, AI and Machine Learning).
  name: ServiceCategory
  type: string
- description: Provider-defined service name.
  name: ServiceName
  type: string
- description: FOCUS service subcategory within the parent ServiceCategory.
  name: ServiceSubcategory
  type:
  - string
  - 'null'
- description: Provider-assigned identifier for the SKU charged.
  name: SkuId
  type:
  - string
  - 'null'
- description: Provider-defined description of what is metered by the SKU.
  name: SkuMeter
  type:
  - string
  - 'null'
- description: Structured object capturing additional pricing attributes specific to the SKU.
  name: SkuPriceDetails
  type:
  - object
  - 'null'
- description: Provider-assigned identifier for the SKU's specific price.
  name: SkuPriceId
  type:
  - string
  - 'null'
- description: Provider-assigned identifier for a sub-account, project, or grouping below the BillingAccountId.
  name: SubAccountId
  type:
  - string
  - 'null'
- description: Display name for the SubAccountId.
  name: SubAccountName
  type:
  - string
  - 'null'
- description: Set of user- or provider-defined tag key/value pairs applied to the charge.
  name: Tags
  type:
  - object
  - 'null'
- description: Implementation-defined extension column. FOCUS reserves the x_ prefix for non-normative provider extensions.
  name: x_CostCategory
  type:
  - string
  - 'null'
provider_name: FOCUS (FinOps Open Cost and Usage Specification)
provider_slug: focus-spec
schema_file: json-schema/focus-billing-record-schema.json
slug: focus-billing-record
source_filename: focus-billing-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/focus-spec/refs/heads/main/json-schema/focus-billing-record-schema.json\",\n  \"title\": \"FOCUS Billing Record\",\n  \"description\": \"JSON Schema representation of a single row in a FOCUS-conformant billing dataset. FOCUS (FinOps Open Cost and Usage Specification) is an open standard maintained under the FinOps Foundation that normalizes cost and usage data across cloud, SaaS, data center, and other technology vendors. This schema lists the normative columns defined by the FOCUS specification and reflects the column attributes (data type, nullability, requirement level) defined in the FOCUS data model. The full normative definitions live at https://focus.finops.org/ and in the FOCUS_Spec repository.\",\n  \"type\": \"object\",\n  \"additionalProperties\": true,\n  \"properties\": {\n    \"AvailabilityZone\": {\n      \"type\": [\"string\", \"\
  null\"],\n      \"description\": \"Provider-assigned identifier for an isolated location within a region.\"\n    },\n    \"BilledCost\": {\n      \"type\": \"number\",\n      \"description\": \"Amount on the invoice for the billing period before amortization, in BillingCurrency.\"\n    },\n    \"BillingAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Provider-assigned identifier for the account that receives the invoice.\"\n    },\n    \"BillingAccountName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Display name for the BillingAccountId.\"\n    },\n    \"BillingCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code in which costs are denominated.\"\n    },\n    \"BillingPeriodEnd\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Exclusive end of the billing period.\"\n    },\n    \"BillingPeriodStart\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"Inclusive start of the billing period.\"\n    },\n    \"ChargeCategory\": {\n      \"type\": \"string\",\n      \"enum\": [\"Usage\", \"Purchase\", \"Tax\", \"Credit\", \"Adjustment\"],\n      \"description\": \"Highest-level classification of a charge.\"\n    },\n    \"ChargeClass\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"Correction\", null],\n      \"description\": \"Indicates whether a charge represents a correction to a previously invoiced billing period.\"\n    },\n    \"ChargeDescription\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Provider-supplied human-readable summary of the charge.\"\n    },\n    \"ChargeFrequency\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"One-Time\", \"Recurring\", \"Usage-Based\", null],\n      \"description\": \"Frequency at which a charge is incurred.\"\n    },\n    \"ChargePeriodEnd\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n \
  \     \"description\": \"Exclusive end of the period over which the charge was incurred.\"\n    },\n    \"ChargePeriodStart\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Inclusive start of the period over which the charge was incurred.\"\n    },\n    \"CommitmentDiscountCategory\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"Spend\", \"Usage\", null],\n      \"description\": \"Whether a commitment-based discount is denominated in spend or usage units.\"\n    },\n    \"CommitmentDiscountId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Provider-assigned identifier for the commitment-based discount applied to the charge.\"\n    },\n    \"CommitmentDiscountName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Display name for the CommitmentDiscountId.\"\n    },\n    \"CommitmentDiscountStatus\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"Used\", \"Unused\"\
  , null],\n      \"description\": \"Whether the commitment-based discount was used or unused for the charge.\"\n    },\n    \"CommitmentDiscountType\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Provider-defined type of commitment-based discount (e.g. Reserved Instance, Savings Plan).\"\n    },\n    \"ConsumedQuantity\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Volume of a metered service consumed, in ConsumedUnit.\"\n    },\n    \"ConsumedUnit\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Provider-defined unit of measurement for ConsumedQuantity.\"\n    },\n    \"ContractedCost\": {\n      \"type\": \"number\",\n      \"description\": \"Cost based on negotiated rates excluding negotiated discounts, in BillingCurrency.\"\n    },\n    \"ContractedUnitPrice\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Per-unit price at negotiated rates, in BillingCurrency per PricingUnit.\"\n    },\n\
  \    \"EffectiveCost\": {\n      \"type\": \"number\",\n      \"description\": \"Amortized cost of the charge after applying upfront and recurring commitment fees, in BillingCurrency.\"\n    },\n    \"InvoiceIssuerName\": {\n      \"type\": \"string\",\n      \"description\": \"Entity responsible for invoicing the consumer.\"\n    },\n    \"ListCost\": {\n      \"type\": \"number\",\n      \"description\": \"Cost based on public list prices, in BillingCurrency.\"\n    },\n    \"ListUnitPrice\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Per-unit price at public list rates, in BillingCurrency per PricingUnit.\"\n    },\n    \"PricingCategory\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"Standard\", \"Dynamic\", \"Committed\", \"Other\", null],\n      \"description\": \"Pricing model used to compute the cost of the charge.\"\n    },\n    \"PricingQuantity\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Quantity priced\
  \ for this charge, in PricingUnit.\"\n    },\n    \"PricingUnit\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Provider-defined unit of measurement used for pricing.\"\n    },\n    \"ProviderName\": {\n      \"type\": \"string\",\n      \"description\": \"Entity providing the resources or services.\"\n    },\n    \"PublisherName\": {\n      \"type\": \"string\",\n      \"description\": \"Entity that produced the resources or services.\"\n    },\n    \"RegionId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Provider-assigned identifier for an isolated geographic area.\"\n    },\n    \"RegionName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Display name for the RegionId.\"\n    },\n    \"ResourceId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Provider-assigned identifier for a billable resource.\"\n    },\n    \"ResourceName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\"\
  : \"Display name of the ResourceId.\"\n    },\n    \"ResourceType\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Provider-defined type of resource.\"\n    },\n    \"ServiceCategory\": {\n      \"type\": \"string\",\n      \"description\": \"FOCUS top-level service category (e.g. Compute, Storage, Networking, AI and Machine Learning).\"\n    },\n    \"ServiceName\": {\n      \"type\": \"string\",\n      \"description\": \"Provider-defined service name.\"\n    },\n    \"ServiceSubcategory\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"FOCUS service subcategory within the parent ServiceCategory.\"\n    },\n    \"SkuId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Provider-assigned identifier for the SKU charged.\"\n    },\n    \"SkuMeter\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Provider-defined description of what is metered by the SKU.\"\n    },\n    \"SkuPriceDetails\": {\n      \"\
  type\": [\"object\", \"null\"],\n      \"description\": \"Structured object capturing additional pricing attributes specific to the SKU.\"\n    },\n    \"SkuPriceId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Provider-assigned identifier for the SKU's specific price.\"\n    },\n    \"SubAccountId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Provider-assigned identifier for a sub-account, project, or grouping below the BillingAccountId.\"\n    },\n    \"SubAccountName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Display name for the SubAccountId.\"\n    },\n    \"Tags\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Set of user- or provider-defined tag key/value pairs applied to the charge.\",\n      \"additionalProperties\": {\n        \"type\": [\"string\", \"number\", \"boolean\", \"null\"]\n      }\n    },\n    \"x_CostCategory\": {\n      \"type\": [\"string\", \"null\"],\n    \
  \  \"description\": \"Implementation-defined extension column. FOCUS reserves the x_ prefix for non-normative provider extensions.\"\n    }\n  },\n  \"required\": [\n    \"BilledCost\",\n    \"BillingAccountId\",\n    \"BillingCurrency\",\n    \"BillingPeriodEnd\",\n    \"BillingPeriodStart\",\n    \"ChargeCategory\",\n    \"ChargePeriodEnd\",\n    \"ChargePeriodStart\",\n    \"ContractedCost\",\n    \"EffectiveCost\",\n    \"InvoiceIssuerName\",\n    \"ListCost\",\n    \"ProviderName\",\n    \"PublisherName\",\n    \"ServiceCategory\",\n    \"ServiceName\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/focus-spec/refs/heads/main/json-schema/focus-billing-record-schema.json
tags:
- Billing
- Cost and Usage
- FinOps
- Open Standard
- Specification
title: FOCUS Billing Record
---
