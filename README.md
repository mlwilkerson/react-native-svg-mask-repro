# react-native-svg-mask-repro
Reproduces error RNSVGMask does not exist error

1. `yarn`
2. `yarn start`
3. Install Expo app on an iPhone
4. Aim iPhone camera app at the QR code presented by `yarn start`
5. Open app in Expo

Expected: rendered view with text and image

Actual: red screen with error:

```
Invariant Violation: Native component for "RNSVGMask" does not exist

This error is located at:
    in RNSVGPath (at Path.js:25)
    in Path (at App.js:19)
    in RNSVGGroup (at G.js:25)
    in G (at App.js:18)
    in RNSVGGroup (at G.js:25)
    in G (at App.js:17)
    in RNSVGMask (at Mask.js:52)
    in Mask (at App.js:15)
    in RNSVGDefs (at Defs.js:8)
    in Defs (at App.js:11)
    in RNSVGSvgView (at Svg.js:92)
    in Svg (at App.js:10)
    in RCTView (at View.js:60)
    in View (at App.js:8)
    in App (at registerRootComponent.js:35)
    in RootErrorBoundary (at registerRootComponent.js:34)
    in ExpoRootComponent (at renderApplication.js:33)
    in RCTView (at View.js:60)
    in View (at AppContainer.js:102)
    in RCTView (at View.js:60)
    in View (at AppContainer.js:122)
    in AppContainer (at renderApplication.js:32)
```
