# **React Native** | _**PayAnsh**_ | _**50854**_

## **Catalog ProjectId: 45025** | **Catalog BuildId: 1820**

## NOTE FOR DEVELOPERS:
Clone the code-engine branch into your working branch. The contents of the branch may get overwritten.
## Author:
Code-Engine
## Keywords:
 - PayAnsh
 - mobile
## Assembled Features To Block Status

| **Feature-Name**        | **Block-Name**        | **Path**  | **Status**  |
|:-------------|:-------------|:-------------|:-------------|
| PhoneLogin      | social-media-account-login<br>social-media-account<br>mobile-account-registration<br>country-code-selector<br>otp-input-confirmation<br>mobile-account-login<br>forgot-password<br>      | {+packages/blocks/social-media-account-login+}<br>{+packages/blocks/social-media-account+}<br>{+packages/blocks/mobile-account-registration+}<br>{+packages/blocks/country-code-selector+}<br>{+packages/blocks/otp-input-confirmation+}<br>{+packages/blocks/mobile-account-login+}<br>{+packages/blocks/forgot-password+}<br> | {+Non-Empty+} |
| GoogleLogin      | social-media-account-registration<br>      | {+packages/blocks/social-media-account-registration+}<br> | {+Non-Empty+} |
| AccountCreation      | email-account-registration<br>      | {+packages/blocks/email-account-registration+}<br> | {+Non-Empty+} |
| Dashboard      | dashboard<br>      | {+packages/blocks/dashboard+}<br> | {+Non-Empty+} |
| Catalogue      | catalogue<br>      | {+packages/blocks/catalogue+}<br> | {+Non-Empty+} |
| CouponCodeGenerator      | couponcodegenerator<br>      | {+packages/blocks/couponcodegenerator+}<br> | {+Non-Empty+} |
| CategoriessubCategories      | categoriessubcategories<br>      | {+packages/blocks/categoriessubcategories+}<br> | {+Non-Empty+} |
| ContactUs      | contactus<br>      | {+packages/blocks/contactus+}<br> | {+Non-Empty+} |
| ApiIntegration      | ApiIntegration      | {-packages/blocks/ApiIntegration-} | {-Empty-} |
| AdminConsole      | AdminConsole      | {-packages/blocks/AdminConsole-} | {-Empty-} |
| AppleLogin      | AppleLogin      | {-packages/blocks/AppleLogin-} | {-Empty-} |
| CustomForm      | CustomForm      | {-packages/blocks/CustomForm-} | {-Empty-} |
| PaymentAdmin      | PaymentAdmin      | {-packages/blocks/PaymentAdmin-} | {-Empty-} |
| AccountVerificationApi      | AccountVerificationApi      | {-packages/blocks/AccountVerificationApi-} | {-Empty-} |
| Payments      | Payments      | {-packages/blocks/Payments-} | {-Empty-} |
| CashfreeIntegration      | CashfreeIntegration      | {-packages/blocks/CashfreeIntegration-} | {-Empty-} |
| OrderDetailView      | OrderDetailView      | {-packages/blocks/OrderDetailView-} | {-Empty-} |
| PayoutApi      | PayoutApi      | {-packages/blocks/PayoutApi-} | {-Empty-} |
| FileAttachment      | FileAttachment      | {-packages/blocks/FileAttachment-} | {-Empty-} |
| RequestManagement      | RequestManagement      | {-packages/blocks/RequestManagement-} | {-Empty-} |
| PushNotifications      | PushNotifications      | {-packages/blocks/PushNotifications-} | {-Empty-} |
| EmailNotifications      | EmailNotifications      | {-packages/blocks/EmailNotifications-} | {-Empty-} |
| Notifications      | Notifications      | {-packages/blocks/Notifications-} | {-Empty-} |
| Sms      | Sms      | {-packages/blocks/Sms-} | {-Empty-} |
| Settings      | Settings      | {-packages/blocks/Settings-} | {-Empty-} |
| AdHocReporting      | AdHocReporting      | {-packages/blocks/AdHocReporting-} | {-Empty-} |
| TransactionLimit      | TransactionLimit      | {-packages/blocks/TransactionLimit-} | {-Empty-} |
| InvoiceBilling      | InvoiceBilling      | {-packages/blocks/InvoiceBilling-} | {-Empty-} |
| AdvancedSearch      | AdvancedSearch      | {-packages/blocks/AdvancedSearch-} | {-Empty-} |
| BharatbillpayIntegration      | BharatbillpayIntegration      | {-packages/blocks/BharatbillpayIntegration-} | {-Empty-} |

## AWS BACKEND DEPLOYMENT URL
 - BaseURL exported as: "https://payansh-50854-ruby.b50854.dev.us-east-1.aws.svc.builder.cafe"
## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 

See docs folder for additional information.

### Prerequisites

What things you need to install the software and how to install them

* React Native (last tested on react-native0.61.3)
  - https://facebook.github.io/react-native/docs/getting-started

* IFF brew is installed and user doesn't have permisions.
```
  $ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/uninstall)"
  $ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

* XCode 11 or greater

* XCode Command Line Tools
```
  $ xcode-select --install
```

* Android SDK
```
  $ brew cask install android-sdk
```

* JDK 11
```
  $ brew tap homebrew/cask-versions
  $ brew cask install java
  $ brew cask install java11
```

### Installing

A step by step series of examples that tell you how to get a development env running

Install yarn
```
  $ brew install yarn
```

Install node

```
  $ brew install node
```

Web
```
  $ yarn
  $ yarn workspace web start 
  (Note: After udpating depencies run again if no cocde erros. )
```

iOS
```
  $ yarn
  $ cd packages/mobile/ios && pod install && cd ../../../ && cp node-runners/RCTUIImageViewAnimated.m node_modules/react-native/Libraries/Image/RCTUIImageViewAnimated.m && npx react-native bundle --entry-file ./packages/mobile/index.js --platform ios --dev true --bundle-output ./packages/mobile/ios/main.jsbundle && yarn ios
```

Android - https://docs.expo.io/versions/latest/workflow/android-studio-emulator/
```
  $ yarn
  $ export JAVA_HOME=`/usr/libexec/java_home -v 11`; java -version; export ANDROID_HOME=${HOME}/Library/Android/sdk; export PATH=${PATH}:${ANDROID_HOME}/emulator && yarn android
```

## Running the tests

```
  $ yarn test
```


## CI/CD Details

We use GitlabCI for our deployment/Build pipelines

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags).



