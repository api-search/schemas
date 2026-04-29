---
description: AuthorisationNotificationAdditionalData schema from Adyen API
layout: schema
name: AuthorisationNotificationAdditionalData
properties_list:
- description: Reference of the payment account.
  name: PaymentAccountReference
  type: string
- description: The acquirer account code.
  name: acquirerAccountCode
  type: string
- description: The acquirer code.
  name: acquirerCode
  type: string
- description: The acquirer reference.
  name: acquirerReference
  type: string
- description: ACS interface. Related to 3DS.
  name: acsRenderingType.acsInterface
  type: string
- description: ACS UI template.
  name: acsRenderingType.acsUiTemplate
  type: string
- description: Alias for this card.
  name: alias
  type: string
- description: Alias type.
  name: aliasType
  type: string
- description: Acquirer Reference Number of the dispute.
  name: arn
  type: string
- description: Authcode of the scheme.
  name: authCode
  type: string
- description: 3DS authentication type
  name: authenticationType
  type: string
- description: Authorisation MID of the acquirer.
  name: authorisationMid
  type: string
- description: The currency authorised for a dynamic zero auth request.
  name: authorisedAmountCurrency
  type: string
- description: The amount authorised for a dynamic zero auth request.
  name: authorisedAmountValue
  type: string
- description: Address Verification Service result.
  name: avsResult
  type: string
- description: Address Verification Service result raw.
  name: avsResultRaw
  type: string
- description: The bank account number.
  name: bankAccountNumber
  type: string
- description: The bank location.
  name: bankLocation
  type: string
- description: The bank location ID.
  name: bankLocationId
  type: string
- description: The bank name.
  name: bankName
  type: string
- description: The bank verificaiton result.
  name: bankVerificationResult
  type: string
- description: The bank verification result raw.
  name: bankVerificationResultRaw
  type: string
- description: Business Identifier Code.
  name: bic
  type: string
- description: 'BillingAddress: county.'
  name: billingAddress.city
  type: string
- description: 'BillingAddress: house number or name.'
  name: billingAddress.houseNumberOrName
  type: string
- description: 'BillingAddress: postal code.'
  name: billingAddress.postalCode
  type: string
- description: 'BillingAddress: state or province'
  name: billingAddress.stateOrProvince
  type: string
- description: 'BillingAddress: street'
  name: billingAddress.street
  type: string
- description: Browser code.
  name: browserCode
  type: string
- description: The amount of delay after authorisation.
  name: captureDelayHours
  type: string
- description: The merchant reference of the capture.
  name: captureMerchantReference
  type: string
- description: The PSP reference of the capture.
  name: capturePspReference
  type: string
- description: Card Bank Identification number.
  name: cardBin
  type: string
- description: Card issuing bank.
  name: cardIssuingBank
  type: string
- description: Card issuing country.
  name: cardIssuingCountry
  type: string
- description: Card issuing currency.
  name: cardIssuingCurrency
  type: string
- description: Card payment method.
  name: cardPaymentMethod
  type: string
- description: Card scheme enhanced data level.
  name: cardSchemeEnhancedDataLevel
  type: string
- description: Card summary
  name: cardSummary
  type: string
- description: Secure Cardholder Authentication Verification Value.
  name: cavv
  type: string
- description: CAVV algorithm.
  name: cavvAlgorithm
  type: string
- description: Information about the 3DS challenge being canceled.
  name: challengeCancel
  type: string
- description: ID of the Checkout Session.
  name: checkoutSessionId
  type: string
- description: Card Verification Code result.
  name: cvcResult
  type: string
- description: Card Verification Code result raw.
  name: cvcResultRaw
  type: string
- description: 'Delivery address: city.'
  name: deliveryAddress.city
  type: string
- description: 'Delivery address: country.'
  name: deliveryAddress.country
  type: string
- description: 'Delivery address: house number or name.'
  name: deliveryAddress.houseNumberOrName
  type: string
- description: 'Delivery address: postal code.'
  name: deliveryAddress.postalCode
  type: string
- description: 'Delivery address: state or province.'
  name: deliveryAddress.stateOrProvince
  type: string
- description: 'Delivery address: street.'
  name: deliveryAddress.street
  type: string
- description: Type of device the request was made from.
  name: deviceType
  type: string
- description: 'Direct debit GB: date of signature.'
  name: directdebit_GB.dateOfSignature
  type: string
- description: 'Direct debit GB: mandate ID.'
  name: directdebit_GB.mandateId
  type: string
- description: 'Direct debit GB: sequence type.'
  name: directdebit_GB.sequenceType
  type: string
- description: 'Direct debit GB: service user name.'
  name: directdebit_GB.serviceUserName
  type: string
- description: 'Direct debit GB: service user number.'
  name: directdebit_GB.serviceUserNumber
  type: string
- description: '3DS: Electronic Commerce Indicator.'
  name: eci
  type: string
- description: Expiry date of the card.
  name: expiryDate
  type: string
- description: Additional cost used in [BIN or card verification](https://docs.adyen.com/payment-methods/cards/bin-data-and-card-verification).
  name: extraCostsCurrency
  type: string
- description: Related additional cost value.
  name: extraCostsValue
  type: string
- description: Gratuity related additional cost value.
  name: extraCostsValueGratuity
  type: string
- description: Surcharge related additional cost value.
  name: extraCostsValueSurcharge
  type: string
- description: Information on the fraud check in a dynamic format.
  name: fraudCheck-<check ID>-<name>
  type: string
- description: Indicates if the risk check was done manually.
  name: fraudManualReview
  type: string
- description: The fraud offset.
  name: fraudOffset
  type: string
- description: Result type of the fraud check.
  name: fraudResultType
  type: string
- description: Funding source.
  name: fundingSource
  type: string
- description: Chargeback gross currency.
  name: grossCurrency
  type: string
- description: Chargeback gross value.
  name: grossValue
  type: string
- description: Only included for iDeal payments.
  name: iDealConsumerAccountNumber
  type: string
- description: Only included for iDeal payments.
  name: iDealConsumerBIC
  type: string
- description: Only included for iDeal payments.
  name: iDealConsumerCity
  type: string
- description: Only included for iDeal payments.
  name: iDealConsumerIBAN
  type: string
- description: Only included for iDeal payments.
  name: iDealConsumerIban
  type: string
- description: Only included for iDeal payments.
  name: iDealConsumerName
  type: string
- description: Only included for iDeal payments.
  name: iDealTransactionId
  type: string
- description: International Bank Account Number.
  name: iban
  type: string
- description: 'The number of installments that the payment amount should be charged with. Example: 5 > Only relevant for card payments in countries that support installments.'
  name: installments.value
  type: string
- description: 3DS interaction counter.
  name: interactionCounter
  type: string
- description: Card holder name.
  name: issuerComments.cardholderName
  type: string
- description: Country of the card issuer.
  name: issuerCountry
  type: string
- description: 'Recurring: Latest card BIN.'
  name: latestCard.bin
  type: string
- description: 'Recurring: Latest card expiry date.'
  name: latestCard.expiryDate
  type: string
- description: 'Recurring: Latest card summary.'
  name: latestCard.summary
  type: string
- description: Risk liability shift.
  name: liabilityShift
  type: string
- description: 'A set of key-value pairs provided in the request, prefixed with ''metadata.''. For example, ''metadata.myField: myValue'''
  name: metadata
  type: object
- description: Recurring related.
  name: networkToken.available
  type: string
- description: Recurring related.
  name: networkToken.bin
  type: string
- description: Recurring related.
  name: networkToken.tokenSummary
  type: string
- description: NFC related.
  name: nfc.expire
  type: string
- description: NFC related.
  name: nfc.issue
  type: string
- description: NFC related.
  name: nfc.pin.provided
  type: string
- description: NFC related.
  name: nfc.uid
  type: string
- description: The transaction token to be used in your Oracle Opera integration.
  name: opi.transToken
  type: string
- description: Owner city.
  name: ownerCity
  type: string
- description: Owner name.
  name: ownerName
  type: string
- description: Related to PayU in LATAM.
  name: payULatamTrazabilityCode
  type: string
- description: ID of the Checkout payment link.
  name: paymentLinkId
  type: string
- description: Related to PayPal.
  name: paypalAddressStatus
  type: string
- description: Related to PayPal.
  name: paypalBillingName
  type: string
- description: 'The buyer''s PayPal account email address. Example: paypaltest@adyen.com'
  name: paypalEmail
  type: string
- description: Related to PayPal.
  name: paypalErrorCode
  type: string
- description: Related to PayPal.
  name: paypalErrorDescription
  type: string
- description: Related to PayPal.
  name: paypalPairingId
  type: string
- description: 'The buyer''s PayPal ID. Example: LF5HCWWBRV2KL'
  name: paypalPayerId
  type: string
- description: 'The buyer''s country of residence. Example: NL'
  name: paypalPayerResidenceCountry
  type: string
- description: 'The status of the buyer''s PayPal account. Example: unverified'
  name: paypalPayerStatus
  type: string
- description: Related to PayPal.
  name: paypalPhone
  type: string
- description: 'The eligibility for PayPal Seller Protection for this payment. Example: Ineligible'
  name: paypalProtectionEligibility
  type: string
- description: Related to PayPal.
  name: paypalRisk
  type: string
- description: Real time Account Update status.
  name: realtimeAccountUpdaterStatus
  type: string
- description: Recurring contract types.
  name: recurring.contractTypes
  type: string
- description: Recurring first PSP reference.
  name: recurring.firstPspReference
  type: string
- description: The [token for stored payment details](https://docs.adyen.com/online-payments/tokenization/create-and-use-tokens/) to make recurring payments.
  name: recurring.recurringDetailReference
  type: string
- description: 'If the payment is referred, this field is set to true. This field is unavailable if the payment is referred and is usually not returned with ecommerce transactions. Example: true'
  name: referred
  type: string
- description: 'Raw refusal reason received from the acquirer, where available. Example: AUTHORISED'
  name: refusalReasonRaw
  type: string
- description: Indicates if an auto rescue for a pyment is scheduled.
  name: retry.rescueScheduled
  type: string
- description: Related to Risk.
  name: riskProfile
  type: string
- description: Related to Risk.
  name: riskProfileReference
  type: string
- description: 'The transaction signature date. Format: yyyy-MM-dd'
  name: sepadirectdebit.dateOfSignature
  type: string
- description: Its value corresponds to the pspReference value of the transaction.
  name: sepadirectdebit.mandateId
  type: string
- description: 'This field can take one of the following values: * OneOff: (OOFF) Direct debit instruction to initiate exactly one direct debit transaction. * First: (FRST) Initial/first collection in a series of dir'
  name: sepadirectdebit.sequenceType
  type: string
- description: Country of the shopper.
  name: shopperCountry
  type: string
- description: Email of the shopper.
  name: shopperEmail
  type: string
- description: IP of the shopper.
  name: shopperIP
  type: string
- description: 'The shopper interaction type of the payment request. Example: Ecommerce'
  name: shopperInteraction
  type: string
- description: The locale of the shopper.
  name: shopperLocale
  type: string
- description: The social security number of the shopper.
  name: shopperSocialSecurityNumber
  type: string
- description: The text to be shown on the shopper's bank statement.
  name: shopperStatement
  type: string
- description: The telephone number of the shopper.
  name: shopperTelephone
  type: string
- description: Identifier of the store processing the transaction.
  name: store
  type: string
- description: Tender reference. For point-of-sale integrations only.
  name: tenderReference
  type: string
- description: Terminal ID. For point-of-sale integrations only.
  name: terminalId
  type: string
- description: 'A Boolean value indicating whether 3DS authentication was completed on this payment. Example: true'
  name: threeDAuthenticated
  type: string
- description: 'The raw 3DS authentication result from the card issuer. Example: N'
  name: threeDAuthenticatedResponse
  type: string
- description: 'A Boolean value indicating whether 3DS was offered for this payment. Example: true'
  name: threeDOffered
  type: string
- description: 'The raw enrollment result from the 3DS directory services of the card schemes. Example: Y'
  name: threeDOfferedResponse
  type: string
- description: The 3D Secure 2 version.
  name: threeDSVersion
  type: string
- description: Payment method variant of the token/wallet payment method.
  name: tokenTxVariant
  type: string
- description: Total fraud score from risk.
  name: totalFraudScore
  type: string
- description: Card summary without tokenization.
  name: untokenisedCardSummary
  type: string
- description: The 3DS transaction ID of the 3DS session sent in notifications. The value is Base64-encoded and is returned for transactions with directoryResponse 'N' or 'Y'. If you want to submit the xid in your 3
  name: xid
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/webhooks-authorisation-notification-additional-data-schema.json
slug: webhooks-authorisation-notification-additional-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-authorisation-notification-additional-data-schema.json\",\n  \"title\": \"AuthorisationNotificationAdditionalData\",\n  \"description\": \"AuthorisationNotificationAdditionalData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PaymentAccountReference\": {\n      \"description\": \"Reference of the payment account.\",\n      \"type\": \"string\"\n    },\n    \"acquirerAccountCode\": {\n      \"description\": \"The acquirer account code.\",\n      \"type\": \"string\"\n    },\n    \"acquirerCode\": {\n      \"description\": \"The acquirer code.\",\n      \"type\": \"string\"\n    },\n    \"acquirerReference\": {\n      \"description\": \"The acquirer reference.\",\n      \"type\": \"string\"\n    },\n    \"acsRenderingType.acsInterface\": {\n      \"description\": \"ACS interface.\
  \ Related to 3DS.\",\n      \"type\": \"string\"\n    },\n    \"acsRenderingType.acsUiTemplate\": {\n      \"description\": \"ACS UI template.\",\n      \"type\": \"string\"\n    },\n    \"alias\": {\n      \"description\": \"Alias for this card.\",\n      \"type\": \"string\"\n    },\n    \"aliasType\": {\n      \"description\": \"Alias type.\",\n      \"type\": \"string\"\n    },\n    \"arn\": {\n      \"description\": \"Acquirer Reference Number of the dispute.\",\n      \"type\": \"string\"\n    },\n    \"authCode\": {\n      \"description\": \"Authcode of the scheme.\",\n      \"type\": \"string\"\n    },\n    \"authenticationType\": {\n      \"description\": \"3DS authentication type\",\n      \"type\": \"string\"\n    },\n    \"authorisationMid\": {\n      \"description\": \"Authorisation MID of the acquirer.\",\n      \"type\": \"string\"\n    },\n    \"authorisedAmountCurrency\": {\n      \"description\": \"The currency authorised for a dynamic zero auth request.\",\n      \"\
  type\": \"string\"\n    },\n    \"authorisedAmountValue\": {\n      \"description\": \"The amount authorised for a dynamic zero auth request.\",\n      \"type\": \"string\"\n    },\n    \"avsResult\": {\n      \"description\": \"Address Verification Service result.\",\n      \"type\": \"string\"\n    },\n    \"avsResultRaw\": {\n      \"description\": \"Address Verification Service result raw.\",\n      \"type\": \"string\"\n    },\n    \"bankAccountNumber\": {\n      \"description\": \"The bank account number.\",\n      \"type\": \"string\"\n    },\n    \"bankLocation\": {\n      \"description\": \"The bank location.\",\n      \"type\": \"string\"\n    },\n    \"bankLocationId\": {\n      \"description\": \"The bank location ID.\",\n      \"type\": \"string\"\n    },\n    \"bankName\": {\n      \"description\": \"The bank name.\",\n      \"type\": \"string\"\n    },\n    \"bankVerificationResult\": {\n      \"description\": \"The bank verificaiton result.\",\n      \"type\": \"string\"\
  \n    },\n    \"bankVerificationResultRaw\": {\n      \"description\": \"The bank verification result raw.\",\n      \"type\": \"string\"\n    },\n    \"bic\": {\n      \"description\": \"Business Identifier Code.\",\n      \"type\": \"string\"\n    },\n    \"billingAddress.city\": {\n      \"description\": \"BillingAddress: county.\",\n      \"type\": \"string\"\n    },\n    \"billingAddress.houseNumberOrName\": {\n      \"description\": \"BillingAddress: house number or name.\",\n      \"type\": \"string\"\n    },\n    \"billingAddress.postalCode\": {\n      \"description\": \"BillingAddress: postal code.\",\n      \"type\": \"string\"\n    },\n    \"billingAddress.stateOrProvince\": {\n      \"description\": \"BillingAddress: state or province\",\n      \"type\": \"string\"\n    },\n    \"billingAddress.street\": {\n      \"description\": \"BillingAddress: street\",\n      \"type\": \"string\"\n    },\n    \"browserCode\": {\n      \"description\": \"Browser code.\",\n      \"type\"\
  : \"string\"\n    },\n    \"captureDelayHours\": {\n      \"description\": \"The amount of delay after authorisation.\",\n      \"type\": \"string\"\n    },\n    \"captureMerchantReference\": {\n      \"description\": \"The merchant reference of the capture.\",\n      \"type\": \"string\"\n    },\n    \"capturePspReference\": {\n      \"description\": \"The PSP reference of the capture.\",\n      \"type\": \"string\"\n    },\n    \"cardBin\": {\n      \"description\": \"Card Bank Identification number.\",\n      \"type\": \"string\"\n    },\n    \"cardIssuingBank\": {\n      \"description\": \"Card issuing bank.\",\n      \"type\": \"string\"\n    },\n    \"cardIssuingCountry\": {\n      \"description\": \"Card issuing country.\",\n      \"type\": \"string\"\n    },\n    \"cardIssuingCurrency\": {\n      \"description\": \"Card issuing currency.\",\n      \"type\": \"string\"\n    },\n    \"cardPaymentMethod\": {\n      \"description\": \"Card payment method.\",\n      \"type\": \"string\"\
  \n    },\n    \"cardSchemeEnhancedDataLevel\": {\n      \"description\": \"Card scheme enhanced data level.\",\n      \"type\": \"string\"\n    },\n    \"cardSummary\": {\n      \"description\": \"Card summary\",\n      \"type\": \"string\"\n    },\n    \"cavv\": {\n      \"description\": \"Secure Cardholder Authentication Verification Value.\",\n      \"type\": \"string\"\n    },\n    \"cavvAlgorithm\": {\n      \"description\": \"CAVV algorithm.\",\n      \"type\": \"string\"\n    },\n    \"challengeCancel\": {\n      \"description\": \"Information about the 3DS challenge being canceled.\",\n      \"type\": \"string\"\n    },\n    \"checkoutSessionId\": {\n      \"description\": \"ID of the Checkout Session.\",\n      \"type\": \"string\"\n    },\n    \"cvcResult\": {\n      \"description\": \"Card Verification Code result.\",\n      \"type\": \"string\"\n    },\n    \"cvcResultRaw\": {\n      \"description\": \"Card Verification Code result raw.\",\n      \"type\": \"string\"\n    },\n\
  \    \"deliveryAddress.city\": {\n      \"description\": \"Delivery address: city.\",\n      \"type\": \"string\"\n    },\n    \"deliveryAddress.country\": {\n      \"description\": \"Delivery address: country.\",\n      \"type\": \"string\"\n    },\n    \"deliveryAddress.houseNumberOrName\": {\n      \"description\": \"Delivery address: house number or name.\",\n      \"type\": \"string\"\n    },\n    \"deliveryAddress.postalCode\": {\n      \"description\": \"Delivery address: postal code.\",\n      \"type\": \"string\"\n    },\n    \"deliveryAddress.stateOrProvince\": {\n      \"description\": \"Delivery address: state or province.\",\n      \"type\": \"string\"\n    },\n    \"deliveryAddress.street\": {\n      \"description\": \"Delivery address: street.\",\n      \"type\": \"string\"\n    },\n    \"deviceType\": {\n      \"description\": \"Type of device the request was made from.\",\n      \"type\": \"string\"\n    },\n    \"directdebit_GB.dateOfSignature\": {\n      \"description\"\
  : \"Direct debit GB: date of signature.\",\n      \"type\": \"string\"\n    },\n    \"directdebit_GB.mandateId\": {\n      \"description\": \"Direct debit GB: mandate ID.\",\n      \"type\": \"string\"\n    },\n    \"directdebit_GB.sequenceType\": {\n      \"description\": \"Direct debit GB: sequence type.\",\n      \"type\": \"string\"\n    },\n    \"directdebit_GB.serviceUserName\": {\n      \"description\": \"Direct debit GB: service user name.\",\n      \"type\": \"string\"\n    },\n    \"directdebit_GB.serviceUserNumber\": {\n      \"description\": \"Direct debit GB: service user number.\",\n      \"type\": \"string\"\n    },\n    \"eci\": {\n      \"description\": \"3DS: Electronic Commerce Indicator.\",\n      \"type\": \"string\"\n    },\n    \"expiryDate\": {\n      \"description\": \"Expiry date of the card.\",\n      \"type\": \"string\"\n    },\n    \"extraCostsCurrency\": {\n      \"description\": \"Additional cost used in [BIN or card verification](https://docs.adyen.com/payment-methods/cards/bin-data-and-card-verification).\"\
  ,\n      \"type\": \"string\"\n    },\n    \"extraCostsValue\": {\n      \"description\": \"Related additional cost value.\",\n      \"type\": \"string\"\n    },\n    \"extraCostsValueGratuity\": {\n      \"description\": \"Gratuity related additional cost value.\",\n      \"type\": \"string\"\n    },\n    \"extraCostsValueSurcharge\": {\n      \"description\": \"Surcharge related additional cost value.\",\n      \"type\": \"string\"\n    },\n    \"fraudCheck-<check ID>-<name>\": {\n      \"description\": \"Information on the fraud check in a dynamic format.\",\n      \"type\": \"string\"\n    },\n    \"fraudManualReview\": {\n      \"description\": \"Indicates if the risk check was done manually.\",\n      \"type\": \"string\"\n    },\n    \"fraudOffset\": {\n      \"description\": \"The fraud offset.\",\n      \"type\": \"string\"\n    },\n    \"fraudResultType\": {\n      \"description\": \"Result type of the fraud check.\",\n      \"type\": \"string\"\n    },\n    \"fundingSource\"\
  : {\n      \"description\": \"Funding source.\",\n      \"type\": \"string\"\n    },\n    \"grossCurrency\": {\n      \"description\": \"Chargeback gross currency.\",\n      \"type\": \"string\"\n    },\n    \"grossValue\": {\n      \"description\": \"Chargeback gross value.\",\n      \"type\": \"string\"\n    },\n    \"iDealConsumerAccountNumber\": {\n      \"description\": \"Only included for iDeal payments.\",\n      \"type\": \"string\"\n    },\n    \"iDealConsumerBIC\": {\n      \"description\": \"Only included for iDeal payments.\",\n      \"type\": \"string\"\n    },\n    \"iDealConsumerCity\": {\n      \"description\": \"Only included for iDeal payments.\",\n      \"type\": \"string\"\n    },\n    \"iDealConsumerIBAN\": {\n      \"description\": \"Only included for iDeal payments.\",\n      \"type\": \"string\"\n    },\n    \"iDealConsumerIban\": {\n      \"description\": \"Only included for iDeal payments.\",\n      \"type\": \"string\"\n    },\n    \"iDealConsumerName\": {\n\
  \      \"description\": \"Only included for iDeal payments.\",\n      \"type\": \"string\"\n    },\n    \"iDealTransactionId\": {\n      \"description\": \"Only included for iDeal payments.\",\n      \"type\": \"string\"\n    },\n    \"iban\": {\n      \"description\": \"International Bank Account Number.\",\n      \"type\": \"string\"\n    },\n    \"installments.value\": {\n      \"description\": \"The number of installments that the payment amount should be charged with.\\n\\nExample: 5\\n> Only relevant for card payments in countries that support installments.\",\n      \"type\": \"string\"\n    },\n    \"interactionCounter\": {\n      \"description\": \"3DS interaction counter.\",\n      \"type\": \"string\"\n    },\n    \"issuerComments.cardholderName\": {\n      \"description\": \"Card holder name.\",\n      \"type\": \"string\"\n    },\n    \"issuerCountry\": {\n      \"description\": \"Country of the card issuer.\",\n      \"type\": \"string\"\n    },\n    \"latestCard.bin\": {\n\
  \      \"description\": \"Recurring: Latest card BIN.\",\n      \"type\": \"string\"\n    },\n    \"latestCard.expiryDate\": {\n      \"description\": \"Recurring: Latest card expiry date.\",\n      \"type\": \"string\"\n    },\n    \"latestCard.summary\": {\n      \"description\": \"Recurring: Latest card summary.\",\n      \"type\": \"string\"\n    },\n    \"liabilityShift\": {\n      \"description\": \"Risk liability shift.\",\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A set of key-value pairs provided in the request, prefixed with 'metadata.'. For example, 'metadata.myField: myValue'\",\n      \"type\": \"object\"\n    },\n    \"networkToken.available\": {\n      \"description\": \"Recurring related.\",\n      \"type\": \"string\"\n    },\n    \"networkToken.bin\": {\n      \"description\": \"Recurring related.\",\n      \"type\": \"string\"\n    },\n    \"networkToken.tokenSummary\"\
  : {\n      \"description\": \"Recurring related.\",\n      \"type\": \"string\"\n    },\n    \"nfc.expire\": {\n      \"description\": \"NFC related.\",\n      \"type\": \"string\"\n    },\n    \"nfc.issue\": {\n      \"description\": \"NFC related.\",\n      \"type\": \"string\"\n    },\n    \"nfc.pin.provided\": {\n      \"description\": \"NFC related.\",\n      \"type\": \"string\"\n    },\n    \"nfc.uid\": {\n      \"description\": \"NFC related.\",\n      \"type\": \"string\"\n    },\n    \"opi.transToken\": {\n      \"description\": \"The transaction token to be used in your Oracle Opera integration.\",\n      \"type\": \"string\"\n    },\n    \"ownerCity\": {\n      \"description\": \"Owner city.\",\n      \"type\": \"string\"\n    },\n    \"ownerName\": {\n      \"description\": \"Owner name.\",\n      \"type\": \"string\"\n    },\n    \"payULatamTrazabilityCode\": {\n      \"description\": \"Related to PayU in LATAM.\",\n      \"type\": \"string\"\n    },\n    \"paymentLinkId\"\
  : {\n      \"description\": \"ID of the Checkout payment link.\",\n      \"type\": \"string\"\n    },\n    \"paypalAddressStatus\": {\n      \"description\": \"Related to PayPal.\",\n      \"type\": \"string\"\n    },\n    \"paypalBillingName\": {\n      \"description\": \"Related to PayPal.\",\n      \"type\": \"string\"\n    },\n    \"paypalEmail\": {\n      \"description\": \"The buyer's PayPal account email address.\\n\\nExample: paypaltest@adyen.com\",\n      \"type\": \"string\"\n    },\n    \"paypalErrorCode\": {\n      \"description\": \"Related to PayPal.\",\n      \"type\": \"string\"\n    },\n    \"paypalErrorDescription\": {\n      \"description\": \"Related to PayPal.\",\n      \"type\": \"string\"\n    },\n    \"paypalPairingId\": {\n      \"description\": \"Related to PayPal.\",\n      \"type\": \"string\"\n    },\n    \"paypalPayerId\": {\n      \"description\": \"The buyer's PayPal ID.\\n\\nExample: LF5HCWWBRV2KL\",\n      \"type\": \"string\"\n    },\n    \"paypalPayerResidenceCountry\"\
  : {\n      \"description\": \"The buyer's country of residence.\\n\\nExample: NL\",\n      \"type\": \"string\"\n    },\n    \"paypalPayerStatus\": {\n      \"description\": \"The status of the buyer's PayPal account.\\n\\nExample: unverified\",\n      \"type\": \"string\"\n    },\n    \"paypalPhone\": {\n      \"description\": \"Related to PayPal.\",\n      \"type\": \"string\"\n    },\n    \"paypalProtectionEligibility\": {\n      \"description\": \"The eligibility for PayPal Seller Protection for this payment.\\n\\nExample: Ineligible\",\n      \"type\": \"string\"\n    },\n    \"paypalRisk\": {\n      \"description\": \"Related to PayPal.\",\n      \"type\": \"string\"\n    },\n    \"realtimeAccountUpdaterStatus\": {\n      \"description\": \"Real time Account Update status.\",\n      \"type\": \"string\"\n    },\n    \"recurring.contractTypes\": {\n      \"description\": \"Recurring contract types.\",\n      \"type\": \"string\"\n    },\n    \"recurring.firstPspReference\": {\n  \
  \    \"description\": \"Recurring first PSP reference.\",\n      \"type\": \"string\"\n    },\n    \"recurring.recurringDetailReference\": {\n      \"description\": \"The [token for stored payment details](https://docs.adyen.com/online-payments/tokenization/create-and-use-tokens/) to make recurring payments.\",\n      \"type\": \"string\"\n    },\n    \"referred\": {\n      \"description\": \"If the payment is referred, this field is set to true.\\n\\nThis field is unavailable if the payment is referred and is usually not returned with ecommerce transactions.\\n\\nExample: true\",\n      \"type\": \"string\"\n    },\n    \"refusalReasonRaw\": {\n      \"description\": \"Raw refusal reason received from the acquirer, where available.\\n\\nExample: AUTHORISED\",\n      \"type\": \"string\"\n    },\n    \"retry.rescueScheduled\": {\n      \"description\": \"Indicates if an auto rescue for a pyment is scheduled.\",\n      \"type\": \"string\"\n    },\n    \"riskProfile\": {\n      \"description\"\
  : \"Related to Risk.\",\n      \"type\": \"string\"\n    },\n    \"riskProfileReference\": {\n      \"description\": \"Related to Risk.\",\n      \"type\": \"string\"\n    },\n    \"sepadirectdebit.dateOfSignature\": {\n      \"description\": \"The transaction signature date.\\n\\nFormat: yyyy-MM-dd\",\n      \"type\": \"string\"\n    },\n    \"sepadirectdebit.mandateId\": {\n      \"description\": \"Its value corresponds to the pspReference value of the transaction.\",\n      \"type\": \"string\"\n    },\n    \"sepadirectdebit.sequenceType\": {\n      \"description\": \"This field can take one of the following values:\\n* OneOff: (OOFF) Direct debit instruction to initiate exactly one direct debit transaction.\\n\\n* First: (FRST) Initial/first collection in a series of direct debit instructions.\\n* Recurring: (RCUR) Direct debit instruction to carry out regular direct debit transactions initiated by the creditor.\\n* Final: (FNAL) Last/final collection in a series of direct debit instructions.\\\
  n\\nExample: OOFF\",\n      \"type\": \"string\"\n    },\n    \"shopperCountry\": {\n      \"description\": \"Country of the shopper.\",\n      \"type\": \"string\"\n    },\n    \"shopperEmail\": {\n      \"description\": \"Email of the shopper.\",\n      \"type\": \"string\"\n    },\n    \"shopperIP\": {\n      \"description\": \"IP of the shopper.\",\n      \"type\": \"string\"\n    },\n    \"shopperInteraction\": {\n      \"description\": \"The shopper interaction type of the payment request.\\n\\nExample: Ecommerce\",\n      \"type\": \"string\"\n    },\n    \"shopperLocale\": {\n      \"description\": \"The locale of the shopper.\",\n      \"type\": \"string\"\n    },\n    \"shopperSocialSecurityNumber\": {\n      \"description\": \"The social security number of the shopper.\",\n      \"type\": \"string\"\n    },\n    \"shopperStatement\": {\n      \"description\": \"The text to be shown on the shopper's bank statement.\",\n      \"type\": \"string\"\n    },\n    \"shopperTelephone\"\
  : {\n      \"description\": \"The telephone number of the shopper.\",\n      \"type\": \"string\"\n    },\n    \"store\": {\n      \"description\": \"Identifier of the store processing the transaction.\",\n      \"type\": \"string\"\n    },\n    \"tenderReference\": {\n      \"description\": \"Tender reference. For point-of-sale integrations only.\",\n      \"type\": \"string\"\n    },\n    \"terminalId\": {\n      \"description\": \"Terminal ID. For point-of-sale integrations only.\",\n      \"type\": \"string\"\n    },\n    \"threeDAuthenticated\": {\n      \"description\": \"A Boolean value indicating whether 3DS authentication was completed on this payment.\\n\\nExample: true\",\n      \"type\": \"string\"\n    },\n    \"threeDAuthenticatedResponse\": {\n      \"description\": \"The raw 3DS authentication result from the card issuer.\\n\\nExample: N\",\n      \"type\": \"string\"\n    },\n    \"threeDOffered\": {\n      \"description\": \"A Boolean value indicating whether 3DS was\
  \ offered for this payment.\\n\\nExample: true\",\n      \"type\": \"string\"\n    },\n    \"threeDOfferedResponse\": {\n      \"description\": \"The raw enrollment result from the 3DS directory services of the card schemes.\\n\\nExample: Y\",\n      \"type\": \"string\"\n    },\n    \"threeDSVersion\": {\n      \"description\": \"The 3D Secure 2 version.\",\n      \"type\": \"string\"\n    },\n    \"tokenTxVariant\": {\n      \"description\": \"Payment method variant of the token/wallet payment method.\",\n      \"type\": \"string\"\n    },\n    \"totalFraudScore\": {\n      \"description\": \"Total fraud score from risk.\",\n      \"type\": \"string\"\n    },\n    \"untokenisedCardSummary\": {\n      \"description\": \"Card summary without tokenization.\",\n      \"type\": \"string\"\n    },\n    \"xid\": {\n      \"description\": \"The 3DS transaction ID of the 3DS session sent in notifications. The value is Base64-encoded and is returned for transactions with directoryResponse 'N'\
  \ or 'Y'. If you want to submit the xid in your 3D Secure 1 request, use the `mpiData.xid`, field.\\n\\nExample: ODgxNDc2MDg2MDExODk5MAAAAAA=\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-authorisation-notification-additional-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AuthorisationNotificationAdditionalData
---
