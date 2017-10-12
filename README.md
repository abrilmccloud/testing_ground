
```javascript
//Define the Transaction attributes
TransactionAttributes txnAttributes = new TransactionAttributes(“<ORDER ID>”)
                .setRevenue(<Total>)
                .setTax(<Tax>)
                .setShipping(<Total Shipping Cost>)

//Define the Transaction attributes
Map<String, String> commEventAttrs = new HashMap<String, String>();
commEventAttrs.put(“Sample Purchase Attribute“, “<value>”);

//Create the Transaction event and attributes
CommerceEvent txnEvent = new CommerceEvent.Builder(Product.PURCHASE, builderProduct).products(productList).transactionAttributes(txnAttributes).currency(“<currency>”).customAttributes(commEventAttrs).build();
        
//Create the Transaction Commerce Event
MParticle.getInstance().logEvent(txnEvent);

```

```javascript
Map<String, String> eventInfo = new HashMap<String, String>();
eventInfo.put(“Custom Attribute”, <value>);
MPEvent event = new MPEvent.Builder(“Login - Success”, MParticle.EventType.Other).info(eventInfo).build(); MParticle.getInstance().logEvent(event);
//Also set User Identifiers and Attributes

```
