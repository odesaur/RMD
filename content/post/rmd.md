+++
title = 'RMD Final'
date = '2025-11-30'
author = 'Naut'
+++
# Essential Links:

App APK here: [rmd.apk](/RMD/documents/rmd.apk)

[Presentation Video](https://www.youtube.com/watch?v=7PpBZFhZMvE) 

[The Original Pitch](/RMD/documents/RMD_Pitch.pdf)

[RMD Final Presentation](/RMD/documents/RMD_Final.pdf)

[Diagram](/RMD/documents/diagram.pdf)

> Direct file is too big to be served on Github, if the download link is
broken please contact
[RMD Code Zip](https://1sfu-my.sharepoint.com/:u:/g/personal/yja78_sfu_ca/EQcIo-_dXiJFjnk5oMGGuVcB7XsKwcOlJ7Q7MtNFWqHLgQ?e=Bds1Fr)

# Team Effort Breakdown

### **Naut**
- Built and maintained the self-hosted Go RMD server, including:
  - Command endpoints: ring, locate, camera capture/upload, lock, help, stats, allowed contacts.
  - Push handling, UnifiedPush registration, token refresh, login/logout persistence.
  - Web portal with grouped UI, themed layout, and server-side session management.
- Completed full command coverage:
  - Remote ring with max-volume fallback.
  - Remote device lock with optional lock-screen message.
  - Remote location via GPS/cell, including OSM map rendering and OpenCellID integration.
  - Remote camera capture and upload.
  - DND/ringer-mode controls, SMS/mesh transport, analytics, logs, in-app triggers.
- Implemented the RMD Lock subsystem using device-admin:
  - Secure lock workflow and ring service.
- Created and improved the web portal:
  - Trigger actions from the browser, show push status and session info.
- Added server authentication and registration flows:
  - Secure password storage, automatic session refresh, in-app server onboarding.
- Added OSM map UI, off-grid Meshtastic support, log export/clear, and response-path handling.
- Improved settings and UX:
  - Custom PINs, command keyword customization, backup/restore (settings, allowed contacts), themes/dynamic colors, notification-permission flows, transport channel setup.
- Added CI/server extras:
  - Photo capture endpoint, UnifiedPush support, self-hosting guidance.

### **Dixon Snider**
- Created initial settings pages and early UI wiring.
- Implemented OpenStreetMap functionality, demo controls, and map integration.
- Added revoke-permission flows and improved permission handling.
- Refactored `MainActivity` and reorganized project structure.
- Added base settings pages: About, Allowed Contacts, Logs.
- Managed early project merges and structural updates.

### **Nam Nguyen**
- Implemented persisted settings storage.
- Added the test-ring feature for validating ring behavior.

### **philakagujones**
- Built the initial General, Find My Device, and Appearance settings screens.
