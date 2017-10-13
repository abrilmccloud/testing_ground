
```javascript

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

