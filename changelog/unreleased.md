# Unreleased Changes

## Updates

- Added new python library for validations
- Consistency updates to the Spec and Examples
- Updated Buyer object fields on checkout
- Updated PaymentProvider fields on checkout

## Checkout API Spec

### Changed

- **Buyer fields**: Removed `Buyer` field `first_name` and field `last_name`.

  - Updated in: `spec/openapi/openapi.agentic_checkout.yaml`
  - Updated in: `spec/json-schema/schema.agentic_checkout.json`
  - Updated in: `rfcs/rfc.agentic_checkout.md`

- **Buyer fields**: Added `Buyer` field `name`.

  - Updated in: `spec/openapi/openapi.agentic_checkout.yaml`
  - Updated in: `spec/json-schema/schema.agentic_checkout.json`
  - Updated in: `rfcs/rfc.agentic_checkout.md`

  - **Buyer fields**: Added `PaymentProvider` field `merchant_id`.

  - Updated in: `spec/openapi/openapi.agentic_checkout.yaml`
  - Updated in: `spec/json-schema/schema.agentic_checkout.json`
  - Updated in: `rfcs/rfc.agentic_checkout.md`

- **Examples**:
  - Added missing "Express" fulfillment option (`fulfillment_option_456`) to `cancel_checkout_session_response` in `examples/examples.agentic_checkout.json` for consistency with other responses.

## Delegate Payment API Spec

### Changed

- **IIN field length**: Updated `iin` field `maxLength` from 6 to 8 characters in `PaymentMethodCard` schema to support extended IIN ranges.
  - Updated in: `spec/openapi/openapi.delegate_payment.yaml`
  - Updated in: `spec/json-schema/schema.delegate_payment.json`
  - Updated in: `rfcs/rfc.delegate_payment.md`
