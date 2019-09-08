# stripe.com

This is a [Stacklane Connector](https://stacklane.com/docs/scripting/connectors) for [Stripe's API](https://stripe.com/docs/api).

For client side use of Stripe, specifiy additional Content-Security-Policy as:

```
<script defer src="https://js.stripe.com/v3/"
        data-frame-src="https://js.stripe.com"
        data-connect-src="https://api.stripe.com"></script>
```        
