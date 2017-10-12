# # Uncomment the line below if you’re using Swift or would like to use dynamic frameworks (recommended but not required)
# use_frameworks!
```javascript
//Set User Customer ID 
MParticle.sharedInstance().setUserIdentity(""<CustomerID>"",identityType: .CustomerId)
//Set User Email Address
MParticle.sharedInstance().setUserIdentity("<user's email>", identityType: .Email)

```
```javascript
github “mparticle/mparticle-apple-sdk” ~> 6.0
```

```javascript
application:didFinishLaunchingWithOptions: delegate call.
```

```javascript
application:didFinishLaunchingWithOptions:
```

```javascript
import mParticle_Apple_SDK
func application(application: UIApplication, didFinishLaunchingWithOptions launchOptions:
[NSObject: AnyObject]?) -> Bool {
    // Other code goes here, prior to initializing the mParticle SDK
    MParticle.sharedInstance().startWithKey("<<<App Key Here>>>", 
    secret:"<<<App Secret Here>>>")
    return true
}
```

```javascript
You can access the Core SDK via Maven Central.
dependencies {
    compile 'com.mparticle:android-core:4.16.1'
}
```
