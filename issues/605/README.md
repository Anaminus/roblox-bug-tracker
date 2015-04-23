Steps:

1. Open file into studio.
2. Publish as a new place.
3. Play the place online.
4. Observe the displayed messages.

Expected results:

- In ServerStorage.rbxl, the last displayed message should say that the Parent
  of ServerStorage is nil, and that the test is done.
- In TestService.rbxl, the last displayed message should say that the
  TestService is being destroyed, with no messages afterward. This indicates
  that something happened as the object was destroyed, to the effect that the
  server script was no longer able to proceed. Pressing Shift+f3, which shows
  network stats, reveals that the client is no longer connected to the server,
  suggesting that the server has crashed.
