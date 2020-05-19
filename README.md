# stripe.com

A [Stacklane Connector](https://stacklane.com/docs/settings/connectors) for the [Stripe API](https://stripe.com/docs/api).

As a best practice, use Stripe's [restricted API keys functionality](https://stripe.com/docs/keys#limit-access).

## Import

/🔌.yaml

```
- https://github.com/stacklane-registry/stripe.com.git#!v1.0.3
```

## Server Side Example

This example reads [active plans](https://stripe.com/docs/api/plans):

```
import {plans} from 'stripe.com';

const plans = plans.list({active:'true', limit: '100').data;
const usdPlans = plans.filter(plan=>plan.currency=='USD');

// ...
```

## Stripe.js Usage

Configures Stripe’s browser-side JavaScript library, [Stripe.js](https://stripe.com/docs/js).

After importing, use the following:

```
<head>
...
<stripe.com-v3 defer/>
...
</head>
```

This applies the correct `Content-Security-Policy` and includes the `<script>` tag.
