# trace_ads

A Flutter project integrating AdMob, Appodeal, Unity Ads, and Start.io.  
Supports all major ad types: Banner, Interstitial, Rewarded, Rewarded Interstitial, Native.

## 1. Where to put your Ad Unit IDs

Edit `lib/ads_config.dart`:

- **AdMob**: Replace the strings for `admobBannerId`, `admobInterstitialId`, `admobRewardedId`, `admobRewardedInterstitialId`, `admobNativeId`
- **Appodeal**: Replace `appodealAppKey`
- **Unity**: Replace `unityGameId`, `unityBannerPlacementId`, `unityInterstitialPlacementId`, `unityRewardedPlacementId`
- **Start.io**: Replace `startAppAppId`

## 2. How to build

- Run `flutter pub get`
- Build with Codemagic or locally:  
  - `flutter build apk --release`
  - `flutter build appbundle --release`
  - `flutter build ios --release --no-codesign`

## 3. Notes for production

- Check each ad network’s documentation for advanced integration and required dashboard settings.
- Some formats (especially Native) require custom UI and registration of ad factories.
- Test your ad units with test IDs before using live ones.

## 4. Codemagic

This repo includes a `codemagic.yaml` for CI/CD.

---

**For more, see the source files and official package documentation.**
