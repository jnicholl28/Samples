# cybersource-unifiedCheckout-samples-node

Unified Checkout Sample integration for Node

Unified Checkout is a CyberSource-hosted HTML/JavaScript component that allows for the acceptance of digital payments within your checkout page. This simple example integration demonstrates using the Unified Checkout SDK to embed this PCI SAQ A level component in your form. Unified Checkout is integrated with Click to Pay.

## Prerequisites

- Node.js 10.15.1 or later
- Express web application framework
- NPM

## Setup Instructions

1. Clone or download this repo.

2. Modify app.js & RequestCaptureContext.js with the CyberSource REST credentials created through [EBC Portal](https://ebc2test.cybersource.com/).

  ```javascript
  const MerchantId = 'YOUR MERCHANT ID';
  const MerchantKeyId = 'YOUR KEY ID (SHARED SECRET SERIAL NUMBER)';
  const MerchantSecretKey = 'YOUR SHARED SECRET';
  ```

3. Pull down the package dependencies
  ```bash
  npm install
  ```

4. Run the web server
```bash
DEBUG=cybersource-unifiedpayments-samples-node:* npm start
```

5. Navigate to https://localhost:3000/checkout to try the sample application

## Tips
NOTE:  This sample uses a self signed certificate for HTTPS for demonstration purposes.  Please ensure that your browsers will accept self signed certificates for local host.

For Chrome set the chrome://flags/#allow-insecure-localhost to Enabled to support this functionality

