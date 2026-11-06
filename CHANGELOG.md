# Changelog

## Ignatius Web Server 1.0

- Fixed server shutdown so closing a public tunnel does not block stopping the local server.
- Made repeated stop requests safe while a server is already stopping.
- Kept the app on the Windows taskbar when minimized instead of hiding it in the system tray.
