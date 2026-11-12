# Changelog

## Ignatius Web Server 1.0

- Fixed servers remaining stuck on "Stopping..." by waiting for normal shutdown and adding a five-second fallback that closes tracked connections; tunnel unshare timeouts and repeated Stop requests now settle cleanly.
- Made repeated stop requests safe while a server is already stopping.
- Fixed server shutdown so closing a public tunnel does not block stopping the local server.
- Fixed shutdown so closed sockets cannot corrupt the active connection list and the HTTP server's close callback finalizes the stop.
- Fixed the server action overlay so a fast start or stop completion cannot leave a stale "Starting..." or "Stopping..." message on screen.
- Kept the app on the Windows taskbar when minimized instead of hiding it in the system tray.
