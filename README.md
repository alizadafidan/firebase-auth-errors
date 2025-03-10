# Firebase Auth Error Codes in English

## Usage

```js
const firebaseErrors = require('./error_codes.json'); 

export function localizeErrorMap(e?: Error & { code?: string }) {
  if (typeof e === 'object' && typeof e.code === 'string' && e.code in firebaseErrors)
    e.message = (firebaseErrors as any)[e.code];
}
```


## All Error Codes

```json
{
    "auth/app-deleted": "The database was not found",
    "auth/expired-action-code": "The action code or link has expired",
    "auth/invalid-action-code": "The action code is invalid. This can happen if the code is malformed or has already been used",
    "auth/user-disabled": "The user corresponding to the provided credential has been disabled",
    "auth/user-not-found": "User does not match any credentials",
    "auth/weak-password": "The password is too weak",
    "auth/email-already-in-use": "I already had an account with the provided email address",
    "auth/invalid-email": "The email address is invalid",
    "auth/operation-not-allowed": "The account type corresponding to this credential is not yet activated",
    "auth/account-exists-with-different-credential": "Email already associated with another account",
    "auth/auth-domain-config-required": "Configuration for authentication has not been provided",
    "auth/credential-already-in-use": "An account already exists for this credential",
    "auth/operation-not-supported-in-this-environment": "This operation is not supported in the environment being performed. Make sure it must be http or https",
    "auth/timeout": "Response time exceeded. The domain may not be authorized to perform operations",
    "auth/missing-android-pkg-name": "A package name must be provided to install the Android application",
    "auth/missing-continue-uri": "The following URL must be provided in the request",
    "auth/missing-ios-bundle-id": "A bundle name must be provided to install the iOS application",
    "auth/invalid-continue-uri": "The following URL provided in the request is not valid",
    "auth/unauthorized-continue-uri": "The domain of the following URL is not whitelisted",
    "auth/invalid-dynamic-link-domain": "The provided dynamic link domain is not authorized or configured in the current project",
    "auth/argument-error": "Check the binding settings for the application",
    "auth/invalid-persistence-type": "The type specified for data persistence is invalid",
    "auth/unsupported-persistence-type": "The current environment does not support the specified type for data persistence",
    "auth/invalid-credential": "The credential has expired or is malformed",
    "auth/wrong-password": "Incorrect password",
    "auth/invalid-verification-code": "The credential verification code is invalid",
    "auth/invalid-verification-id": "The credential verification ID is invalid",
    "auth/custom-token-mismatch": "The token is different from the requested standard",
    "auth/invalid-custom-token": "The supplied token is invalid",
    "auth/captcha-check-failed": "The reCAPTCHA response token is invalid, expired, or the domain is not allowed",
    "auth/invalid-phone-number": "The phone number is in an invalid format (E.164 standard)",
    "auth/missing-phone-number": "The phone number is required",
    "auth/quota-exceeded": "The SMS quota has been exceeded",
    "auth/canceled-popup-request": "Only one popup request is allowed at a time",
    "auth/popup-blocked": "The browser has blocked the popup",
    "auth/popup-closed-by-user": "The user closed the popup without completing the provider login",
    "auth/unauthorized-domain": "The application domain is not authorized to perform operations",
    "auth/invalid-user-token": "The current user was not identified",
    "auth/user-token-expired": "The current user’s token has expired",
    "auth/null-user": "The current user is null",
    "auth/app-not-authorized": "Application not authorized to authenticate with the given key",
    "auth/invalid-api-key": "The provided API key is invalid",
    "auth/network-request-failed": "Error connecting to network",
    "auth/requires-recent-login": "The user’s last access time does not meet the security limit",
    "auth/too-many-requests": "Requests were blocked due to unusual activity. Please try again after a while",
    "auth/web-storage-unsupported": "The browser does not support storage or if the user has disabled this function",
    "auth/invalid-claims": "The custom registry attributes are not valid",
    "auth/claims-too-large": "The size of the request exceeds the maximum allowed size of 1 Megabyte",
    "auth/id-token-expired": "The reported token has expired",
    "auth/id-token-revoked": "The reported token has expired",
    "auth/invalid-argument": "An invalid argument was supplied to a method",
    "auth/invalid-creation-time": "The creation time must be a valid UTC date",
    "auth/invalid-disabled-field": "Property for disabled user is invalid",
    "auth/invalid-display-name": "The username is not valid",
    "auth/invalid-email-verified": "The email is not valid",
    "auth/invalid-hash-algorithm": "The HASH algorithm does not support cryptography",
    "auth/invalid-hash-block-size": "The HASH block size is invalid",
    "auth/invalid-hash-derived-key-length": "The size of the HASH derived key is invalid",
    "auth/invalid-hash-key": "The HASH key must have a valid byte buffer",
    "auth/invalid-hash-memory-cost": "HASH memory cost is not valid",
    "auth/invalid-hash-parallelization": "HASH parallel loading is invalid",
    "auth/invalid-hash-rounds": "HASH rounding is not valid",
    "auth/invalid-hash-salt-separator": "The SALT separator field of the HASH generation algorithm must be a valid byte buffer",
    "auth/invalid-id-token": "The entered token code is invalid",
    "auth/invalid-last-sign-in-time": "The last login time must be a valid UTC date",
    "auth/invalid-page-token": "The following URL provided in the request is not valid",
    "auth/invalid-password": "The password is not valid, it must be at least 6 characters long",
    "auth/invalid-password-hash": "The HASH password is invalid",
    "auth/invalid-password-salt": "SALT password is invalid",
    "auth/invalid-photo-url": "The URL of the user’s photo is not valid",
    "auth/invalid-provider-id": "The provider identifier is not supported",
    "auth/invalid-session-cookie-duration": "The duration of the session COOKIE must be a valid number in milliseconds, between 5 minutes and 2 weeks",
    "auth/invalid-uid": "The identifier provided must have a maximum of 128 characters",
    "auth/invalid-user-import": "The user record to import is invalid",
    "auth/invalid-provider-data": "The data provider is invalid",
    "auth/maximum-user-count-exceeded": "The maximum number of users allowed to import has been exceeded",
    "auth/missing-hash-algorithm": "It is necessary to provide the HASH generation algorithm and its parameters to import users",
    "auth/missing-uid": "An identifier is required for the current operation",
    "auth/reserved-claims": "One or more custom properties provided reserved words used",
    "auth/session-cookie-revoked": "The COOKIE session has expired",
    "auth/uid-adic-exists": "The provided identifier is already in use",
    "auth/email-already-exists": "The email provided is already in use",
    "auth/phone-number-already-exists": "The provided phone is already in use",
    "auth/project-not-found": "No projects found",
    "auth/insufficient-permission": "The credential used does not have access to the requested resource",
    "auth/internal-error": "The authentication server encountered an unexpected error while trying to process the request"
  }
```
