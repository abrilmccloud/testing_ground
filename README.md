
```javascript
var attributes = [String: String]()
attributes[“Custom Attribute”] = “<value>”
MParticle.sharedInstance().logEvent(“Login - Success”, eventType: .Other, eventInfo: attributes)
//Also set User Identifiers and Attributes
```

```javascript
Map<String, String> eventInfo = new HashMap<String, String>();
eventInfo.put(“Custom Attribute”, <value>);
MPEvent event = new MPEvent.Builder(“Login - Success”, MParticle.EventType.Other).info(eventInfo).build(); MParticle.getInstance().logEvent(event);
//Also set User Identifiers and Attributes

```
