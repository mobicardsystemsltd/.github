# MobiCard Systems – APIs & SDKs

Welcome to our developer platform 👋  

MobiCard offers a unified collection of APIs designed to simplify payment card handling, reduce PCI scope, enhance fraud controls, and enable global financial integrations.

All API calls require an initial JWT Token API request.

Each SDK lives in its **own repository** with full documentation, installation guides, and examples.  

This page serves as a **central index** to all available APIs and SDKs.

---
---

## 🔐 Payment Card Scan API
### MobiCard ScanAPI

Transform user checkout experiences with our intelligent card scanning technology. Let users scan or upload payment cards to automatically extract and validate card data.

Use Cases:

**E-commerce checkout:** Allow users to use their device camera to scan their card instead of manually typing card numbers.

**Mobile apps:** A smooth payment card entry experience for apps selling goods or services.

**Back-office onboarding:** Enterprises ingest card details faster and more reliably when adding payment methods to user profiles.

Use this multi-platform API to enhance your end-user's card checkout experience by letting them scan (or upload) their payment cards. Extract the card number, expiry date, brand information, EXIF data, Risk information and perform validation checks and card tokenization automatically. Code samples are provided.

With two implementation methods to select from depending on your use case.

#### Method 1
    Use method 1 with our scan card UI template (HTML/CSS/JS WebStack) to quickly get started or method 2 below.

#### Method 2
    Incase you need to have more control over your UI or when developing mobile applications (by securely passing the card image base64 string). This method is Best For: 
    Mobile apps (iOS/Android), custom UI implementations, or when you already have image data in base64 format.
    
    Note:
    
        The value for the "status" response parameter is always either "SUCCESS" or "FAILED" for this API. Use this to determine subsequent actions. 

### Technical Difference: 
Method 1 accepts the actual image file ('mobicard_scan_card_photo') as multipart form-data while Method 2 accepts the card image's base64 string ('mobicard_scan_card_photo_base64_string') within the initial request access token call. Method 1 is a 2-step API call process while Method 2 involves a single API call.

    
##### Method 1
| SDK Repository | Description |
|---------------|-------------|
| [Scan Card API PHP SDK](https://github.com/mobicardsystemsltd/scanapi-method1-php) | PHP SDK for Scan API using device Camera |
| [Scan Card API Python SDK](https://github.com/mobicardsystemsltd/scanapi-method1-python) | Python client for Scan API |
| [Scan Card API Java SDK](https://github.com/mobicardsystemsltd/scanapi-method1-java) | Java client library for Scan API |
| [Scan Card API Nodejs SDK](https://github.com/mobicardsystemsltd/scanapi-method1-nodejs) | Nodejs SDK for Scan API |
| [Scan Card API Curl SDK](https://github.com/mobicardsystemsltd/scanapi-method1-curl) | Curl client for Scan API|


Mobile & Hybrid App Integration

| SDK Repository | Description |
|---------------|-------------|
| [React Native / Expo Implementation](https://github.com/mobicardsystemsltd/scanapi-method1-php) | PHP SDK for Scan API using device Camera |
| [Flutter Implementation](https://github.com/mobicardsystemsltd/scanapi-method1-python) | Python client for Scan API |
| [Ionic Implementation](https://github.com/mobicardsystemsltd/scanapi-method1-java) | Java client library for Scan API |
| [PWA Implementation](https://github.com/mobicardsystemsltd/scanapi-method1-nodejs) | Nodejs SDK for Scan API |





##### Method 2
| SDK Repository | Description |
|---------------|-------------|
| [Scan Card API Base64 PHP SDK](https://github.com/mobicardsystemsltd/scanapi-method2-php) | PHP SDK for developers who want full control over their UI/UX.  |
| [Scan Card API Base64 Python SDK](https://github.com/mobicardsystemsltd/scanapi-method2-python) | Python client for Scan API |
| [Scan Card API Base64 Java SDK](https://github.com/mobicardsystemsltd/scanapi-method2-java) | Java client library for Scan API |
| [Scan Card API Base64 Nodejs SDK](https://github.com/mobicardsystemsltd/scanapi-method2-nodejs) | Nodejs SDK for Scan API |
| [Scan Card API Base64 Curl SDK](https://github.com/mobicardsystemsltd/scanapi-method2-curl) | Curl client for Scan API|


---
---

## 💳 Tokenization API
### MobiToken API

Dramatically reduce your PCI DSS compliance scope by replacing sensitive card data with secure cryptographic tokens that can't be reverse-engineered.

| SDK Repository | Description |
|---------------|-------------|
| [Tokenization API PHP SDK](https://github.com/mobicardsystemsltd/mobitoken-php) | PHP client for MobiToken API |
| [Tokenization API Python SDK](https://github.com/mobicardsystemsltd/mobitoken-python) | Python SDK for MobiToken API |
| [Tokenization API Java SDK](https://github.com/mobicardsystemsltd/mobitoken-java) | Java SDK for MobiToken API |
| [Tokenization API Nodejs SDK](https://github.com/mobicardsystemsltd/mobitoken-nodejs) | NodeJS SDK for MobiToken API |
| [Tokenization API Curl SDK](https://github.com/mobicardsystemsltd/mobitoken-curl) | Curl client for MobiToken API |

---
---

## 👤 BIIN / BIN Lookup API
### MobiBiin API

Make intelligent payment decisions with real-time card issuer data. Identify card schemes, issuer banks, and risk factors instantly for every transaction.

| SDK Repository | Description |
|---------------|-------------|
| [Tokenization API PHP SDK](https://github.com/mobicardsystemsltd/mobi-biin-php) | PHP SDK for MobiBiin API |
| [Tokenization API Python SDK](https://github.com/mobicardsystemsltd/mobi-biin-python) | Python client for MobiBiin API|
| [Tokenization API Java SDK](https://github.com/mobicardsystemsltd/mobi-biin-java) | Java client for MobiBiin API |
| [Tokenization API Nodejs SDK](https://github.com/mobicardsystemsltd/mobi-biin-nodejs) | Nodejs SDK for MobiBiin API |
| [Tokenization API Curl SDK](https://github.com/mobicardsystemsltd/mobi-biin-curl) | Curl client for MobiBiin API |

---
---

## 📊 Forex Rates API
### MobiRates API

Access real‑time foreign exchange rates for global financial applications, e‑commerce platforms, and international payment systems.

| SDK Repository | Description |
|---------------|-------------|
| [Tokenization API PHP SDK](https://github.com/mobicardsystemsltd/mobirates-php) | PHP client for MobiRates API|
| [Tokenization API Python SDK](https://github.com/mobicardsystemsltd/mobirates-python) | Python SDK for MobiRates API |
| [Tokenization API Java SDK](https://github.com/mobicardsystemsltd/mobirates-java) | Java SDK for MobiRates API |
| [Tokenization API Nodejs SDK](https://github.com/mobicardsystemsltd/mobirates-nodejs) | Nodejs SDK for MobiRates API |
| [Tokenization API Curl SDK](https://github.com/mobicardsystemsltd/mobirates-curl) | Curl client for MobiRates API |

---

## 📚 Documentation & Standards

- SDKs follow consistent naming and versioning conventions
- Backward compatibility is maintained where possible

---

## 🤝 Contributions & Support

- Please open issues in the **relevant SDK repository**
- Pull requests are welcome
- For security issues, contact us privately via support@mobicardsystems.com

---

## 🚀 Getting Started

1. Choose the API you want to integrate
2. Select your preferred SDK
3. Follow the README in the SDK repository
4. Start building

Happy coding! 🎉
