
```swift
//Create Custom Attributes to add to Purchase event
var attributes = [String: String]()
attributes[“Sample Purchase Attribute“] = "<value>"
commerceEvent.setCustomAttributes(attributes)

//Define the Transaction attributes
var txnattributes = MPTransactionAttributes()
txnattributes.transactionId = "<Order Number>"
txnattributes.revenue = "<Total>"
txnattributes.tax = "<Tax>"
txnattributes.shipping = "<Shipping>"

//Create the Transaction event and attributes
txnEvent.transactionAttributes = txnattributes
txnEvent.currency = "<currency>"
MParticle.sharedInstance().logCommerceEvent(txnEvent)

//Create the Transaction Commerce Event
var txnEvent = MPCommerceEvent(action: MPCommerceEventAction.purchase, product: nil)

```

```javascript
target ‘<Your Target>’ do
    pod ‘mParticle-Appboy’, ‘~> 6’
    pod ‘mParticle-BranchMetrics’, ‘~> 6’
    pod ‘mParticle-Localytics’, ‘~> 6’
end
```
```javascript
//Set User Customer ID 
MParticle.sharedInstance().setUserIdentity(‘<CustomerID>’,identityType: .CustomerId)
//Set User Email Address
MParticle.sharedInstance().setUserIdentity("<user's email>", identityType: .Email)
```
```javascript
//Set User Customer ID 
MParticle.getInstance().setUserIdentity(‘<CustomerID>’, MParticle.IdentityType.CustomerId); 
//Set User Email Address
```

