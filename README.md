# QRTOTP: Secure Authentication & API Infrastructure

A REST-based authentication engine implementing Time-based One-Time Password (TOTP) protocols over QR mechanisms to mitigate replay attacks and credential harvesting.

## System Architecture

- **Backend API:** Django REST Framework handling secure identity management, session tokens, and dynamic TOTP payload generation.
- **Mobile Client (React Native / Expo):** Cross-platform mobile application consuming the REST endpoints to generate and scan OTP tokens. 
  - **Live Frontend Preview:** [Expo Snack Sandbox](https://snack.expo.dev/@nisaraoun514/qrtotp)

## Security Features Implemented
- **Dynamic Key Distribution:** Secure generation of TOTP secrets passed via cryptographic QR payloads.
- **Endpoint Protection:** Structured exception handling in API views to prevent error-based data disclosure.
- **Cross-Origin Security:** Strict CORS configurations regulating token exchange between mobile client and server boundaries.

## Tech Stack
- **Backend:** Python, Django, Django REST Framework
- **Frontend Client:** React Native, Expo Snack
- **Security Protocols:** TOTP / QR Authentication
