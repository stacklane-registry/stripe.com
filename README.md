# stripe.com

A [Stacklane Connector](https://stacklane.com/docs/scripting/connectors) for the [Stripe API](https://stripe.com/docs/api).

## Client Side

The client side JavaScript for Stripe requires additional content security policies.

Specify additional policies as follows:

```
<script defer src="https://js.stripe.com/v3/"
        data-frame-src="https://js.stripe.com"
        data-connect-src="https://api.stripe.com"></script>
```        
