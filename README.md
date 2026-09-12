# hns-bridge-auth

Telegram Mini App page used by a private Telegram bot bridge for biometric (Face ID / Touch ID) approval.

- Static, single `index.html`; no secrets, no backend, no analytics.
- The secret token is generated on the phone and stored in Telegram's biometric-protected storage
  (`Telegram.WebApp.BiometricManager`); the page only relays it back to the bot via `sendData`.
- Source of truth: `Tools/telegram-bridge/webapp/index.html` in the project repository.
