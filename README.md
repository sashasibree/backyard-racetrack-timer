# Backyard Race Timer

A hands-free timer for a backyard RC car track. An iPhone on a steady mount watches the track through its camera. You tap two rocks on screen to draw a START line and a FINISH line, and the app times the car from one to the other.

**Current version: gate test.** It checks that the camera reliably sees the car cross each gate (beeps at each gate and announces a test time). The race flow (Ready, Racing, Returning, Staging) and the top-five leaderboard come next.

Open it at https://sashasibree.github.io/backyard-racetrack-timer/ in Safari, then use Share > Add to Home Screen.

Settings and times are stored only on the phone.

## Two-device version (connection test)

`duo.html` splits the job across two devices: the iPhone watches the start gate up close and the iPad watches the finish gate and does the timing. The phone sends the exact moment the car crossed, converted to the iPad's clock (the devices compare clocks over Wi-Fi before racing), so Wi-Fi delay does not affect the time.

Open https://sashasibree.github.io/backyard-racetrack-timer/duo.html on both devices. Pairing uses the free public PeerJS service.
