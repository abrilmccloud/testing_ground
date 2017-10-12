
```javascript
//Set User Customer ID 
MParticle.sharedInstance().setUserIdentity(""<CustomerID>"",identityType: .CustomerId)
//Set User Email Address
MParticle.sharedInstance().setUserIdentity("<user's email>", identityType: .Email)

```

```javascript
//Set User Customer ID 
MParticle.getInstance().setUserIdentity("<CustomerID>", MParticle.IdentityType.CustomerId); 
//Set User Email Address
MParticle.getInstance().setUserIdentity("<user's email address>", MParticle.IdentityType.Email);

```
