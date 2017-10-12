
```javascript
//Create Custom Attributes to add to Purchase event
var attributes = [String: String]()
attributes[“Sample Purchase Attribute“] = “<value>”
commerceEvent.setCustomAttributes(attributes)

//Define the Transaction attributes
var txnattributes = MPTransactionAttributes()
txnattributes.transactionId = “<Order Number>”
txnattributes.revenue = “<Total>”
txnattributes.tax = “<Tax>”
txnattributes.shipping = “<Shipping>”

//Create the Transaction event and attributes
txnEvent.transactionAttributes = txnattributes
txnEvent.currency = “<currency>”
MParticle.sharedInstance().logCommerceEvent(txnEvent)

//Create the Transaction Commerce Event
var txnEvent = MPCommerceEvent(action: MPCommerceEventAction.purchase, 
```

```javascript
Map<String, String> eventInfo = new HashMap<String, String>();
eventInfo.put(“Custom Attribute”, <value>);
MPEvent event = new MPEvent.Builder(“Login - Success”, MParticle.EventType.Other).info(eventInfo).build(); MParticle.getInstance().logEvent(event);
//Also set User Identifiers and Attributes

```
