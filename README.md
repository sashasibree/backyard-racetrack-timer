# Backyard Race Timer

The main page is now the two-device version (Race Timer Duo). The original single-camera version lives at single.html.

A hands-free timer for a backyard RC car track. An iPhone on a steady mount watches the track through its camera. You tap two rocks on screen to draw a START line and a FINISH line, and the app times the car from one to the other.

**Current version: gate test.** It checks that the camera reliably sees the car cross each gate (beeps at each gate and announces a test time). The race flow (Ready, Racing, Returning, Staging) and the top-five leaderboard come next.

Open it at https://sashasibree.github.io/backyard-racetrack-timer/single.html in Safari, then use Share > Add to Home Screen.

Settings and times are stored only on the phone.

## Two-device race version (Race Timer Duo)

`duo.html` splits the job across two devices: the iPhone watches the start gate up close and the iPad watches the finish gate and does the timing. The phone sends the exact moment the car crossed, converted to the iPad's clock (the devices compare clocks over Wi-Fi before racing), so Wi-Fi delay does not affect the time.

Open https://sashasibree.github.io/backyard-racetrack-timer/ on both devices (any iPhone, iPad or Android phone). The old duo.html link forwards there. Pairing uses the free public PeerJS service.

Race flow: the phone arms itself once the start line has been clear for 2 seconds (it beeps and the iPad says "Ready"). The next start crossing starts the run; the iPad's finish crossing ends it and announces the time and its place on the board. Stop timer on either device cancels a run; a run with no finish in 60 seconds cancels itself.

Top 5: kept on the iPad with dates. Remove any entry, clear the board, or switch off "Save times" for practice runs.
