# Yijie Liu

I'm a software engineer in Vienna. I work on clinical imaging software and study Business Informatics at FH Technikum Wien. One feature I shipped lets a radiologist scroll through one image stack while a compatible series from another study follows the corresponding slice. I also run SoloTechAI, the one-person studio where I build and operate my own apps.

## Zimple Home

I built a household inventory app for iOS, Android, and the web. Forward an order confirmation and the items arrive in a review list with their prices and purchase dates. After you save an item, anyone you share the household with can find its receipt or check when its warranty expires. [See Zimple Home](https://zimple.tech)

One production problem was deciding what an error report could safely contain. A household invitation carries a token in its URL. I use Sentry SDKs with self-hosted GlitchTip, so I added filters that remove invite tokens from browser breadcrumbs, request URLs, and API transaction names before those records leave the application. On mobile and web, crash reporting follows the user's diagnostics preference.

## Code you can read

**Mein Wohn-Ticket Checker** is a Python service that watches for matching housing listings in Vienna. The first poll establishes a baseline. Later polls notify the user when a listing appears, including when a previously removed listing comes back. The tests cover expired sessions and verify that repeated failures trigger one alert followed by a recovery notification. [Read the code](https://github.com/Dev02Liu/meinwohnticketChecker) · [Read the tests](https://github.com/Dev02Liu/meinwohnticketChecker/blob/main/tests/test_checker.py) · [English setup guide](https://github.com/Dev02Liu/meinwohnticketChecker/blob/main/README.en.md)

## Other projects I'm building

| Project | An engineering problem I worked on |
| --- | --- |
| [ClipLookout](https://cliplookout.com) | Turns streams and recordings into vertical highlights. Python workers claim jobs from a PostgreSQL queue. I wrote integration tests for two workers claiming work at once, expired leases, and jobs that exhaust their retries. |
| [Golpix](https://golpix.com) | A padel coaching app in development. Native Swift and Kotlin modules extract pose landmarks on the phone. The scoring engine checks whether enough of the player is visible to give feedback and flags measurements it can't trust. |
| [RepWake](https://repwake.app) | An exercise alarm that counts push-ups and squats on the phone. If the camera loses sight of the user halfway through a set, the counter pauses and resumes at rest, keeping the completed reps. |

[SoloTechAI](https://solotechai.com) · [LinkedIn](https://www.linkedin.com/in/yijie-liu-746556214/) · [X](https://x.com/SoloDev_AT)
