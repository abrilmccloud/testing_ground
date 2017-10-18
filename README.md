
```swift
github "mparticle/mparticle-apple-sdk" ~> 6.0
```

```javascript
target ‘<Your Target>’ do
    pod ‘mParticle-Appboy’, ‘~> 6’
    pod ‘mParticle-BranchMetrics’, ‘~> 6’
    pod ‘mParticle-Localytics’, ‘~> 6’
end
```
```javascript
//Set User First Name, Last Name, and a Custom Attribute example
MParticle.sharedInstance().setUserAttribute("$FirstName", value: "<user first name>")
MParticle.sharedInstance().setUserAttribute("$LastName", value: "<user last name>")
MParticle.sharedInstance().setUserAttribute("[CUSTOMATTR]", value: "<VALUE>")
```
```javascript
//Set User First Name, Last Name, and a Custom Attribute example
MParticle.getInstance().setUserAttribute(MParticle.UserAttributes.FIRSTNAME,“<user's first name>”)
MParticle.getInstance().setUserAttribute(MParticle.UserAttributes.LASTNAME, “<user's last name>”)
MParticle.getInstance().setUserAttribute("[CUSTOMATTR]", "<value>")
```

