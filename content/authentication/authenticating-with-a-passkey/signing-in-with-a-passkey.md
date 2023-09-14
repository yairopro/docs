---
title: Signing in with a passkey
intro: 'You can use a passkey to sign in safely and easily to {% data variables.product.prodname_dotcom_the_website %}, without requiring a password and two-factor authentication. You can also sign in using a passkey on a nearby device.'
permissions: 'Personal account owners who manage their own credentials can authenticate to {% data variables.product.prodname_dotcom_the_website %} using passkeys.'
versions:
  feature: passkeys
type: how_to
shortTitle: Sign in with a passkey
---
{% note %}

{% data reusables.passkeys.beta-note %}

{% endnote %}

## About signing in with a passkey

You must first add a passkey to your account before you can use the passkey to sign in to {% data variables.product.prodname_dotcom_the_website %}. For more information, see "[AUTOTITLE](/authentication/authenticating-with-a-passkey/managing-your-passkeys)."

Once you have added a passkey to your account, you can use the passkey to sign in safely and securely to {% data variables.product.prodname_dotcom_the_website %} without having to enter your password or perform two-factor authentication (2FA). Once you have added a synced passkey on one device, the passkey is available to use across multiple devices. These devices must use the same passkey provider (such as iCloud).

Some authenticators allow passkeys to be used with nearby devices. For example, perhaps you want to sign in to {% data variables.product.prodname_dotcom_the_website %} using a bluetooth-enabled laptop that's not set up with a passkey. If you have registered a passkey on your phone, you might opt to scan a QR code, or trigger a push notification to your phone, in order to complete the sign in securely. For more information, see "[Signing in with a passkey using a nearby device](#signing-in-with-a-passkey-using-a-nearby-device)."

## Signing in with a passkey linked to your primary device

1. Navigate to the login page for {% data variables.product.prodname_dotcom_the_website %} at [https://github.com/login?passkey=true](https://github.com/login?passkey=true).
1. Click **{% octicon "passkey-fill" aria-hidden="true" %} Sign in with a passkey**.
1. Follow the prompts on your browser or platform to select a passkey that is accessible from the device you are using, and complete the authentication process. For example, when prompted, you might touch a fingerprint sensor or enter your PIN.

## Signing in with a passkey using a nearby device

1. Navigate to the login page for {% data variables.product.prodname_dotcom_the_website %} at [https://github.com/login?passkey=true](https://github.com/login?passkey=true).
1. Click **{% octicon "passkey-fill" aria-hidden="true" %} Sign in with a passkey**.
1. Follow the prompts on your browser or platform to select a passkey that's accessible as a nearby device (such as a phone or a tablet).
1. Continue to follow the prompts to start the authentication process. For example, you might choose to scan a QR code, or trigger a push notification to the nearby device.
1. On your nearby device, follow the prompts to complete the authentication process. For example, if you are using an iPhone, you might perform FaceID or enter your passcode.

## Further reading
- [AUTOTITLE](/authentication/authenticating-with-a-passkey/about-passkeys)
- [AUTOTITLE](/authentication/authenticating-with-a-passkey/managing-your-passkeys)
