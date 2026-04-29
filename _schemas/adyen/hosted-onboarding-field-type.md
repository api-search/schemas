---
description: FieldType schema from Adyen API
layout: schema
name: FieldType
properties_list:
- description: The full name of the property.
  name: field
  type: string
- description: The type of the field.
  name: fieldName
  type: string
- description: The code of the shareholder that the field belongs to. If empty, the field belongs to an account holder.
  name: shareholderCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/hosted-onboarding-field-type-schema.json
slug: hosted-onboarding-field-type
source_filename: hosted-onboarding-field-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/hosted-onboarding-field-type-schema.json\",\n  \"title\": \"FieldType\",\n  \"description\": \"FieldType schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"field\": {\n      \"description\": \"The full name of the property.\",\n      \"type\": \"string\"\n    },\n    \"fieldName\": {\n      \"description\": \"The type of the field.\",\n      \"enum\": [\n        \"accountCode\",\n        \"accountHolderCode\",\n        \"accountHolderDetails\",\n        \"accountNumber\",\n        \"accountStateType\",\n        \"accountStatus\",\n        \"accountType\",\n        \"address\",\n        \"balanceAccount\",\n        \"balanceAccountActive\",\n        \"balanceAccountCode\",\n        \"balanceAccountId\",\n        \"bankAccount\",\n        \"bankAccountCode\",\n        \"bankAccountName\"\
  ,\n        \"bankAccountUUID\",\n        \"bankBicSwift\",\n        \"bankCity\",\n        \"bankCode\",\n        \"bankName\",\n        \"bankStatement\",\n        \"branchCode\",\n        \"businessContact\",\n        \"cardToken\",\n        \"checkCode\",\n        \"city\",\n        \"companyRegistration\",\n        \"constitutionalDocument\",\n        \"controller\",\n        \"country\",\n        \"countryCode\",\n        \"currency\",\n        \"currencyCode\",\n        \"dateOfBirth\",\n        \"description\",\n        \"destinationAccountCode\",\n        \"document\",\n        \"documentContent\",\n        \"documentExpirationDate\",\n        \"documentIssuerCountry\",\n        \"documentIssuerState\",\n        \"documentName\",\n        \"documentNumber\",\n        \"documentType\",\n        \"doingBusinessAs\",\n        \"drivingLicence\",\n        \"drivingLicenceBack\",\n        \"drivingLicenceFront\",\n        \"drivingLicense\",\n        \"email\",\n        \"firstName\"\
  ,\n        \"formType\",\n        \"fullPhoneNumber\",\n        \"gender\",\n        \"hopWebserviceUser\",\n        \"houseNumberOrName\",\n        \"iban\",\n        \"idCard\",\n        \"idCardBack\",\n        \"idCardFront\",\n        \"idNumber\",\n        \"identityDocument\",\n        \"individualDetails\",\n        \"infix\",\n        \"jobTitle\",\n        \"lastName\",\n        \"lastReviewDate\",\n        \"legalArrangement\",\n        \"legalArrangementCode\",\n        \"legalArrangementEntity\",\n        \"legalArrangementEntityCode\",\n        \"legalArrangementLegalForm\",\n        \"legalArrangementMember\",\n        \"legalArrangementMembers\",\n        \"legalArrangementName\",\n        \"legalArrangementReference\",\n        \"legalArrangementRegistrationNumber\",\n        \"legalArrangementTaxNumber\",\n        \"legalArrangementType\",\n        \"legalBusinessName\",\n        \"legalEntity\",\n        \"legalEntityType\",\n        \"logo\",\n        \"merchantAccount\"\
  ,\n        \"merchantCategoryCode\",\n        \"merchantHouseNumber\",\n        \"merchantReference\",\n        \"microDeposit\",\n        \"name\",\n        \"nationality\",\n        \"originalReference\",\n        \"ownerCity\",\n        \"ownerCountryCode\",\n        \"ownerDateOfBirth\",\n        \"ownerHouseNumberOrName\",\n        \"ownerName\",\n        \"ownerPostalCode\",\n        \"ownerState\",\n        \"ownerStreet\",\n        \"passport\",\n        \"passportNumber\",\n        \"payoutMethod\",\n        \"payoutMethodCode\",\n        \"payoutSchedule\",\n        \"pciSelfAssessment\",\n        \"personalData\",\n        \"phoneCountryCode\",\n        \"phoneNumber\",\n        \"postalCode\",\n        \"primaryCurrency\",\n        \"reason\",\n        \"registrationNumber\",\n        \"returnUrl\",\n        \"schedule\",\n        \"shareholder\",\n        \"shareholderCode\",\n        \"shareholderCodeAndSignatoryCode\",\n        \"shareholderCodeOrSignatoryCode\",\n     \
  \   \"shareholderType\",\n        \"shareholderTypes\",\n        \"shopperInteraction\",\n        \"signatory\",\n        \"signatoryCode\",\n        \"socialSecurityNumber\",\n        \"sourceAccountCode\",\n        \"splitAccount\",\n        \"splitConfigurationUUID\",\n        \"splitCurrency\",\n        \"splitValue\",\n        \"splits\",\n        \"stateOrProvince\",\n        \"status\",\n        \"stockExchange\",\n        \"stockNumber\",\n        \"stockTicker\",\n        \"store\",\n        \"storeDetail\",\n        \"storeName\",\n        \"storeReference\",\n        \"street\",\n        \"taxId\",\n        \"tier\",\n        \"tierNumber\",\n        \"transferCode\",\n        \"ultimateParentCompany\",\n        \"ultimateParentCompanyAddressDetails\",\n        \"ultimateParentCompanyAddressDetailsCountry\",\n        \"ultimateParentCompanyBusinessDetails\",\n        \"ultimateParentCompanyBusinessDetailsLegalBusinessName\",\n        \"ultimateParentCompanyBusinessDetailsRegistrationNumber\"\
  ,\n        \"ultimateParentCompanyCode\",\n        \"ultimateParentCompanyStockExchange\",\n        \"ultimateParentCompanyStockNumber\",\n        \"ultimateParentCompanyStockNumberOrStockTicker\",\n        \"ultimateParentCompanyStockTicker\",\n        \"unknown\",\n        \"value\",\n        \"verificationType\",\n        \"virtualAccount\",\n        \"visaNumber\",\n        \"webAddress\",\n        \"year\"\n      ],\n      \"type\": \"string\"\n    },\n    \"shareholderCode\": {\n      \"description\": \"The code of the shareholder that the field belongs to. If empty, the field belongs to an account holder.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/hosted-onboarding-field-type-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: FieldType
---
