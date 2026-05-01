---
description: A single cost and usage record conforming to the FinOps Open Cost and Usage Specification (FOCUS) v1.3. Contains dimensions (qualitative values for categorization and filtering) and metrics (quantitative values for measurement).
layout: schema
name: FOCUS Cost and Usage Record
properties_list:
- description: A provider-assigned identifier for a physically separated and isolated area within a region that provides high availability and fault tolerance.
  name: AvailabilityZone
  type:
  - string
  - 'null'
- description: A charge serving as the basis for invoicing, inclusive of the impacts of all reduced rates and discounts while excluding the amortization of relevant purchases.
  name: BilledCost
  type: number
- description: The unique identifier for a billing account.
  name: BillingAccountId
  type: string
- description: The display name assigned to a billing account.
  name: BillingAccountName
  type:
  - string
  - 'null'
- description: The currency that a charge was billed in. Represented as a three-letter ISO 4217 currency code.
  name: BillingCurrency
  type: string
- description: The exclusive end date and time of the billing period.
  name: BillingPeriodEnd
  type: string
- description: The inclusive start date and time of the billing period.
  name: BillingPeriodStart
  type: string
- description: The identifier assigned to a capacity reservation by the provider. Introduced in FOCUS v1.3.
  name: CapacityReservationId
  type:
  - string
  - 'null'
- description: The highest-level classification of a charge based on the nature of how it is billed.
  name: ChargeCategory
  type: string
- description: Indicates whether the row represents a correction to one or more charges invoiced in a previous billing period.
  name: ChargeClass
  type:
  - string
  - 'null'
- description: A self-contained summary of the charge's purpose and price.
  name: ChargeDescription
  type:
  - string
  - 'null'
- description: Indicates how often a charge will occur.
  name: ChargeFrequency
  type: string
- description: The exclusive end date and time of a charge period.
  name: ChargePeriodEnd
  type: string
- description: The inclusive start date and time of a charge period.
  name: ChargePeriodStart
  type: string
- description: Indicates whether the commitment discount is based on usage quantity or cost.
  name: CommitmentDiscountCategory
  type:
  - string
  - 'null'
- description: The identifier assigned to a commitment discount by the provider.
  name: CommitmentDiscountId
  type:
  - string
  - 'null'
- description: The display name assigned to a commitment discount.
  name: CommitmentDiscountName
  type:
  - string
  - 'null'
- description: The amount of a commitment discount purchased or accounted for in commitment discount-related rows.
  name: CommitmentDiscountQuantity
  type:
  - number
  - 'null'
- description: Indicates whether the charge corresponds to the consumption of a commitment discount or the unused portion.
  name: CommitmentDiscountStatus
  type:
  - string
  - 'null'
- description: A provider-assigned label describing the type of commitment discount (e.g., Reserved Instance, Savings Plan).
  name: CommitmentDiscountType
  type:
  - string
  - 'null'
- description: The provider-specified measurement unit for the commitment discount quantity.
  name: CommitmentDiscountUnit
  type:
  - string
  - 'null'
- description: The volume of a given resource or service used, based on the consumed unit.
  name: ConsumedQuantity
  type:
  - number
  - 'null'
- description: The provider-specified measurement unit indicating how a resource or service was consumed.
  name: ConsumedUnit
  type:
  - string
  - 'null'
- description: The cost calculated by multiplying contracted unit price and the corresponding pricing quantity.
  name: ContractedCost
  type: number
- description: The agreed-upon unit price for a single pricing unit of the associated resource or service.
  name: ContractedUnitPrice
  type:
  - number
  - 'null'
- description: The amortized cost of the charge after applying all reduced rates, discounts, and the applicable portion of relevant prepaid purchases.
  name: EffectiveCost
  type: number
- description: The name of the entity responsible for invoicing for the resources or services consumed.
  name: InvoiceIssuerName
  type: string
- description: The cost calculated by multiplying list unit price and the corresponding pricing quantity.
  name: ListCost
  type: number
- description: The suggested provider-published unit price for a single pricing unit of the associated resource or service.
  name: ListUnitPrice
  type:
  - number
  - 'null'
- description: Describes the pricing model used for a charge at the time of use or purchase.
  name: PricingCategory
  type:
  - string
  - 'null'
- description: The volume of a given resource or service used or purchased, based on the pricing unit.
  name: PricingQuantity
  type:
  - number
  - 'null'
- description: The provider-specified measurement unit for determining unit prices and pricing quantities.
  name: PricingUnit
  type:
  - string
  - 'null'
- description: The name of the entity that made the resource or service available for purchase.
  name: ProviderName
  type: string
- description: The name of the entity that produced the resource or service that was purchased.
  name: PublisherName
  type:
  - string
  - 'null'
- description: An isolated geographic area where a resource is provisioned in or a service is provided from.
  name: Region
  type:
  - string
  - 'null'
- description: The unique identifier assigned to a resource by the provider.
  name: ResourceId
  type:
  - string
  - 'null'
- description: The display name assigned to a resource.
  name: ResourceName
  type:
  - string
  - 'null'
- description: The type of resource the charge applies to.
  name: ResourceType
  type:
  - string
  - 'null'
- description: The highest-level classification of a service based on the core function of the service (e.g., Compute, Storage, Networking, Database).
  name: ServiceCategory
  type: string
- description: The display name of the service that was purchased.
  name: ServiceName
  type: string
- description: A secondary classification of a service, providing further detail beyond ServiceCategory.
  name: ServiceSubcategory
  type:
  - string
  - 'null'
- description: The unique identifier for the SKU that was used or purchased.
  name: SkuId
  type:
  - string
  - 'null'
- description: The unique identifier for the SKU inclusive of all pricing variations such as tiering and discounts.
  name: SkuPriceId
  type:
  - string
  - 'null'
- description: The identifier assigned to a grouping of resources or services, often used to manage access and/or cost.
  name: SubAccountId
  type:
  - string
  - 'null'
- description: The display name assigned to a sub account.
  name: SubAccountName
  type:
  - string
  - 'null'
- description: A set of key-value pairs applied to a resource. Tags are commonly used for cost allocation, access control, and automation.
  name: Tags
  type:
  - object
  - 'null'
- description: The method used by the data generator for split cost allocation across workloads. Introduced in FOCUS v1.3.
  name: x_SplitCostAllocationMethod
  type:
  - string
  - 'null'
- description: The percentage of the cost allocated to this record via split cost allocation. Introduced in FOCUS v1.3.
  name: x_SplitCostAllocationPercentage
  type:
  - number
  - 'null'
provider_name: FinOps Foundation
provider_slug: finops-foundation
schema_file: json-schema/finops-foundation-cost-and-usage-record-schema.json
slug: finops-foundation-cost-and-usage-record
source_filename: finops-foundation-cost-and-usage-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/finops-foundation/refs/heads/main/json-schema/finops-foundation-cost-and-usage-record-schema.json\",\n  \"title\": \"FOCUS Cost and Usage Record\",\n  \"description\": \"A single cost and usage record conforming to the FinOps Open Cost and Usage Specification (FOCUS) v1.3. Contains dimensions (qualitative values for categorization and filtering) and metrics (quantitative values for measurement).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AvailabilityZone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A provider-assigned identifier for a physically separated and isolated area within a region that provides high availability and fault tolerance.\"\n    },\n    \"BilledCost\": {\n      \"type\": \"number\",\n      \"description\": \"A charge serving as the basis for invoicing, inclusive of the impacts of all reduced\
  \ rates and discounts while excluding the amortization of relevant purchases.\"\n    },\n    \"BillingAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for a billing account.\"\n    },\n    \"BillingAccountName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The display name assigned to a billing account.\"\n    },\n    \"BillingCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"The currency that a charge was billed in. Represented as a three-letter ISO 4217 currency code.\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"BillingPeriodEnd\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The exclusive end date and time of the billing period.\"\n    },\n    \"BillingPeriodStart\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The inclusive start date and time of the billing period.\"\n    },\n    \"CapacityReservationId\"\
  : {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The identifier assigned to a capacity reservation by the provider. Introduced in FOCUS v1.3.\"\n    },\n    \"ChargeCategory\": {\n      \"type\": \"string\",\n      \"enum\": [\"Usage\", \"Purchase\", \"Tax\", \"Credit\", \"Adjustment\"],\n      \"description\": \"The highest-level classification of a charge based on the nature of how it is billed.\"\n    },\n    \"ChargeClass\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"Correction\", null],\n      \"description\": \"Indicates whether the row represents a correction to one or more charges invoiced in a previous billing period.\"\n    },\n    \"ChargeDescription\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A self-contained summary of the charge's purpose and price.\"\n    },\n    \"ChargeFrequency\": {\n      \"type\": \"string\",\n      \"enum\": [\"One-Time\", \"Recurring\", \"Usage-Based\"],\n      \"description\":\
  \ \"Indicates how often a charge will occur.\"\n    },\n    \"ChargePeriodEnd\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The exclusive end date and time of a charge period.\"\n    },\n    \"ChargePeriodStart\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The inclusive start date and time of a charge period.\"\n    },\n    \"CommitmentDiscountCategory\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"Spend\", \"Usage\", null],\n      \"description\": \"Indicates whether the commitment discount is based on usage quantity or cost.\"\n    },\n    \"CommitmentDiscountId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The identifier assigned to a commitment discount by the provider.\"\n    },\n    \"CommitmentDiscountName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The display name assigned to a commitment discount.\"\n    },\n\
  \    \"CommitmentDiscountQuantity\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"The amount of a commitment discount purchased or accounted for in commitment discount-related rows.\"\n    },\n    \"CommitmentDiscountStatus\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"Used\", \"Unused\", null],\n      \"description\": \"Indicates whether the charge corresponds to the consumption of a commitment discount or the unused portion.\"\n    },\n    \"CommitmentDiscountType\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A provider-assigned label describing the type of commitment discount (e.g., Reserved Instance, Savings Plan).\"\n    },\n    \"CommitmentDiscountUnit\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The provider-specified measurement unit for the commitment discount quantity.\"\n    },\n    \"ConsumedQuantity\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"The volume\
  \ of a given resource or service used, based on the consumed unit.\"\n    },\n    \"ConsumedUnit\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The provider-specified measurement unit indicating how a resource or service was consumed.\"\n    },\n    \"ContractedCost\": {\n      \"type\": \"number\",\n      \"description\": \"The cost calculated by multiplying contracted unit price and the corresponding pricing quantity.\"\n    },\n    \"ContractedUnitPrice\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"The agreed-upon unit price for a single pricing unit of the associated resource or service.\"\n    },\n    \"EffectiveCost\": {\n      \"type\": \"number\",\n      \"description\": \"The amortized cost of the charge after applying all reduced rates, discounts, and the applicable portion of relevant prepaid purchases.\"\n    },\n    \"InvoiceIssuerName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the entity responsible\
  \ for invoicing for the resources or services consumed.\"\n    },\n    \"ListCost\": {\n      \"type\": \"number\",\n      \"description\": \"The cost calculated by multiplying list unit price and the corresponding pricing quantity.\"\n    },\n    \"ListUnitPrice\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"The suggested provider-published unit price for a single pricing unit of the associated resource or service.\"\n    },\n    \"PricingCategory\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"On-Demand\", \"Commitment-Based\", \"Dynamic\", \"Other\", null],\n      \"description\": \"Describes the pricing model used for a charge at the time of use or purchase.\"\n    },\n    \"PricingQuantity\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"The volume of a given resource or service used or purchased, based on the pricing unit.\"\n    },\n    \"PricingUnit\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\"\
  : \"The provider-specified measurement unit for determining unit prices and pricing quantities.\"\n    },\n    \"ProviderName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the entity that made the resource or service available for purchase.\"\n    },\n    \"PublisherName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The name of the entity that produced the resource or service that was purchased.\"\n    },\n    \"Region\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"An isolated geographic area where a resource is provisioned in or a service is provided from.\"\n    },\n    \"ResourceId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The unique identifier assigned to a resource by the provider.\"\n    },\n    \"ResourceName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The display name assigned to a resource.\"\n    },\n    \"ResourceType\": {\n      \"type\": [\"\
  string\", \"null\"],\n      \"description\": \"The type of resource the charge applies to.\"\n    },\n    \"ServiceCategory\": {\n      \"type\": \"string\",\n      \"description\": \"The highest-level classification of a service based on the core function of the service (e.g., Compute, Storage, Networking, Database).\"\n    },\n    \"ServiceName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the service that was purchased.\"\n    },\n    \"ServiceSubcategory\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A secondary classification of a service, providing further detail beyond ServiceCategory.\"\n    },\n    \"SkuId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The unique identifier for the SKU that was used or purchased.\"\n    },\n    \"SkuPriceId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The unique identifier for the SKU inclusive of all pricing variations such as tiering\
  \ and discounts.\"\n    },\n    \"SubAccountId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The identifier assigned to a grouping of resources or services, often used to manage access and/or cost.\"\n    },\n    \"SubAccountName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The display name assigned to a sub account.\"\n    },\n    \"Tags\": {\n      \"type\": [\"object\", \"null\"],\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A set of key-value pairs applied to a resource. Tags are commonly used for cost allocation, access control, and automation.\"\n    },\n    \"x_SplitCostAllocationMethod\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The method used by the data generator for split cost allocation across workloads. Introduced in FOCUS v1.3.\"\n    },\n    \"x_SplitCostAllocationPercentage\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\"\
  : \"The percentage of the cost allocated to this record via split cost allocation. Introduced in FOCUS v1.3.\"\n    }\n  },\n  \"required\": [\n    \"BilledCost\",\n    \"BillingAccountId\",\n    \"BillingCurrency\",\n    \"BillingPeriodEnd\",\n    \"BillingPeriodStart\",\n    \"ChargeCategory\",\n    \"ChargeFrequency\",\n    \"ChargePeriodEnd\",\n    \"ChargePeriodStart\",\n    \"ContractedCost\",\n    \"EffectiveCost\",\n    \"InvoiceIssuerName\",\n    \"ListCost\",\n    \"ProviderName\",\n    \"ServiceCategory\",\n    \"ServiceName\"\n  ],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/finops-foundation/refs/heads/main/json-schema/finops-foundation-cost-and-usage-record-schema.json
tags:
- Budgets
- Costs
- FinOps
title: FOCUS Cost and Usage Record
---
