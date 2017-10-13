
```javascript
<?xml version=”1.0” encoding=”utf-8” ?>
<!-- ex. src/main/res/values/mparticle.xml -->
<resources>
    <string name=”mp_key”>APP KEY</string>
    <string name=”mp_secret”>APP SECRET</string>
</resources>
```

```javascript
target ‘<Your Target>’ do
    pod ‘mParticle-Appboy’, ‘~> 6’
    pod ‘mParticle-BranchMetrics’, ‘~> 6’
    pod ‘mParticle-Localytics’, ‘~> 6’
end
```
```javascript
dependencies {
    compile (
        ‘com.mparticle:android-example-kit:4.16.2’,
        ‘com.mparticle:android-another-kit:4.16.2’
    )
}
```
```swift
#Uncomment the line below if you're using Swift or would like to use dynamic frameworks
(recommended but not required)
#use_frameworks!
target '<Your Target>'
    pod 'mParticle-Apple-SDK', '~> 6'
End
```
