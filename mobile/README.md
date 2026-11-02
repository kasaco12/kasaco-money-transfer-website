# KASACO MONEY TRANSFER — Native mobile development demo

This is an **Expo / React Native** prototype, not a payment product. It has no financial institution integration, KYC, actual identity verification, authentication, bank accounts, or real funds. Do not use real customer data.

## Start locally

Install Node.js LTS, then run:

```bash
cd mobile
npm install
npx expo start
```

Try the prototype on Expo Go where supported. This repository provides source code only. **It is not an App Store listing or signed iOS build.**

## Build for TestFlight / App Store

After enrolling a verified legal entity in the Apple Developer Program and setting up an Expo account:

```bash
npm install -g eas-cli
eas login
eas build:configure
eas build --platform ios --profile production
eas submit --platform ios
```

Set a unique bundle identifier controlled by the organization before uploading. Generate compliant app icon and splash assets, complete privacy policy, app listing, screenshots, review notes, tests, and financial compliance documents. Apple may reject a basic demo. The release decision rests with Apple.

## Demo functionality

- Native Home and Send tabs, Recipients, History, Demo Admin.
- USD -> TZS / CDF / KES sample estimates.
- Tries public USD exchange reference rates at https://open.er-api.com/v6/latest/USD; labels fallback estimates.
- Sample fee ($2.99 + 1.2%) is not a quote.
- Sample recipients and transfers exist in app local memory only and reset when the app fully restarts.

The public website remains at https://kasaco12.github.io/kasaco-money-transfer-website/.
