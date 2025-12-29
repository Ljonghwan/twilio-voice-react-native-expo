# Twilio Voice React Native SDK


[![NPM](https://img.shields.io/npm/v/%40twilio/voice-react-native-sdk.svg?color=blue)](https://www.npmjs.com/package/%40twilio/voice-react-native-sdk) [![CircleCI](https://dl.circleci.com/status-badge/img/gh/twilio/twilio-voice-react-native/tree/main.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/twilio/twilio-voice-react-native/tree/main)

Twilio's Voice React Native SDK allows you to add real-time voice and PSTN calling to your React Native apps.

- [Documentation](https://www.twilio.com/docs/voice/sdks/react-native)
- [API Reference](https://github.com/twilio/twilio-voice-react-native/blob/latest/docs/api/voice-react-native-sdk.md)
- [Reference App](https://github.com/twilio/twilio-voice-react-native-app)

Please check out the following if you are new to Twilio's Programmable Voice or React Native.

- [Programmable Voice](https://www.twilio.com/docs/voice/sdks)
- [React Native](https://reactnative.dev/docs/getting-started)

## Installation
# Confirmed to work on expo version 53.0.25

The package is available through [npm](https://www.npmjs.com/package/@twilio/voice-react-native-sdk).

```sh
npm install github:Ljonghwan/twilio-voice-react-native-expo
```

app.json 
   ```json
   {
      "voice-react-native-sdk/expo-config-plugin/ios.js",
      [
         "voice-react-native-sdk/expo-config-plugin/android.js",
         {
            "firebaseMessagingServiceEnabled": true,
            "googleServicesJsonPath": "./google-services.json"
         }
      ]
   }
   ```

```sh
npx expo prebuild --clean
```

Then import and use it exactly like the original Twilio SDK:

```javascript
import { Voice } from '@your-username/voice-react-native-sdk';

const voice = new Voice();
// Use the SDK as normal
```

### Package Structure

The published package includes:

- **Source Code**: Original TypeScript/JavaScript source files
- **Built Libraries**: Compiled CommonJS and ES modules
- **Type Definitions**: Complete TypeScript definitions
- **Native Code**: Android (Java) and iOS (Objective-C) implementations
- **Assets**: Audio files, icons, and other resources
- **Source Maps**: For debugging compiled code

### Troubleshooting

- **Build Errors**: Run `yarn install` to ensure all dependencies are installed
- **Publish Errors**: Verify you're logged into npm with `npm whoami`
- **Permission Errors**: Ensure you have publish rights to the npm scope/organization
- **Version Conflicts**: Make sure the version number is unique and higher than the previous version

## Supporting Documentation

### Getting Started

#### iOS

Learn how to get started for the [iOS platform](/docs/getting-started-ios.md).

#### Android

Learn how to get started for the Android platform if you are using [Java](/docs/getting-started-android-java.md) or [Kotlin](/docs/getting-started-android-kotlin.md).

### Migration Guide

If you are migrating from a version of the Twilio Voice React Native SDK `< 1.0.0.beta.4` to a version `>= 1.0.0.beta.4`, please see [this](/docs/migration-guide-beta.4.md) document.

### Customizing Notifications

To customize the appearance and content of your application's notifications, please see [this](/docs/customize-notifications.md) document.

### Outgoing Call Ringback Tone

To enable your application to play a ringback tone while making an outgoing call, please see [this](/docs/play-outgoing-call-ringback-tone.md) document.

### Out-of-band PushKit Handling

To have your application implement or use its own `PushKit` delegate module, please see [this](/docs/applications-own-pushkit-handler.md) document.

### Out-of-band Firebase Messaging Service

To have your application implement or use a different `FirebaseMessagingService` (such as OneSignal or RNFirebase), please see [this](/docs/out-of-band-firebase-messaging-service.md) document.

## Issues and Support

Please check out our [common issues](/COMMON_ISSUES.md) page or file any issues you find here on Github. For general inquiries related to the Voice SDK you can file a support ticket.

Please ensure that you are not sharing any [Personally Identifiable Information(PII)](https://www.twilio.com/docs/glossary/what-is-personally-identifiable-information-pii) or sensitive account information (API keys, credentials, etc.) when reporting an issue.

Please check out our [known issues](/KNOWN_ISSUES.md) for known bugs and workarounds.

## Related

- [Reference App](https://github.com/twilio/twilio-voice-react-native-app)
- [Twilio Voice JS](https://github.com/twilio/twilio-voice.js)
- [Twilio Voice iOS](https://github.com/twilio/voice-quickstart-ios)
- [Twilio Voice Android](https://github.com/twilio/voice-quickstart-android)

## License

See [LICENSE](/LICENSE)
