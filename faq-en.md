---
title: FAQ (Apple Watch & iPhone)
---

# FAQ — MaxRecover Timer for Apple Watch & iPhone

**Last updated / 最終更新:** 2026-06-11
**Contact / 連絡先:** maxsaunatimer@gmail.com

> 🌐 言語 / Language: **English** / [🇯🇵 日本語](faq-ja.html)

> 🐛 Report bugs & suggestions: **[Feedback form](feedback.html)**

---

### 1. Subscription & Billing

**Q. How much is Premium?**
See the Premium tab in the app for current pricing in your region. A yearly
plan is also available at roughly **20% off** vs paying monthly. New
subscribers get a 30-day free trial.

**Q. What does Premium unlock?**
Advanced analytics (recovery slope, recovery curves, HRR trends), an A4 PDF
report, sharing with a heart-rate chart image, CSV export, a dedicated
Premium app icon, and no banner ads.

**Q. iCloud sync — is it Premium?**
No. iCloud sync is free for everyone. Data protection is infrastructure, not a
paid feature.

**Q. What happens when the free trial ends?**
Your subscription auto-renews at the regular price. You can cancel at any time
during the trial — if you cancel at least 24 hours before the trial ends, you
are not charged.

**Q. How do I cancel?**
On your iPhone: Settings → tap your Apple ID at the top → Subscriptions →
MaxRecover Premium → Cancel Subscription. After canceling, you keep Premium
features until the current billing period ends.

**Q. Does canceling delete my data?**
No. Your sessions, history, settings, and iCloud sync all stay. Only the
Premium features (advanced analytics, PDF report, chart-image sharing, CSV
export, Premium app icon, ad-free) revert to the free tier.

**Q. I paid but Premium isn't active on a new device.**
Make sure the new device is signed in to the App Store with the **same Apple
ID** you used to purchase. Then open the **Premium tab** in the app and tap
**Restore purchases** to re-verify your entitlement with the App Store.

**Q. Refunds?**
Apple handles all refund requests. Use
[reportaproblem.apple.com](https://reportaproblem.apple.com).

### 2. Data and Privacy

**Q. What data do you collect?**
The developer does not collect, receive, or store any of your data. There is no
server. All session data, health data, and locations stay on your device, and
if iCloud is enabled, in your own private iCloud account.

**Q. Where is my data stored?**
On your iPhone (SwiftData) and Apple Watch (a local JSON file). With iCloud
enabled, sessions sync through your private CloudKit database — accessible
only by you.

**Q. What if I delete the app?**
With iCloud sync enabled, your data is restored automatically when you
reinstall. Without iCloud, local data is lost — Premium users can use CSV
export as a manual backup.

**Q. Does the app use Apple Health?**
Yes. With your permission, the app reads heart rate during a session and
writes the session as a HealthKit workout, visible in the Apple Health app.

**Q. Does the free version share my data with advertisers?**
The free version shows AdMob banner ads in the History, Analytics, and Session
Detail screens. Ad network data handling follows Google's policies and your
device's privacy settings (ATT / Limit Ad Tracking). See the Privacy Policy
for details.

### 3. Usage & Features

**Q. What is the Afterglow Score?**
A 0–100 score estimating how quickly your parasympathetic nervous system
("rest mode") engages after a hot-bath session, derived from your heart-rate
recovery (HRR1 / HRR3 / HRR5). It puts a number on what Japanese sauna culture
calls "totonou". Reference value only — not a medical metric.

**Q. Can I use the app without an Apple Watch?**
The timer works on iPhone alone, but heart-rate measurement and the Afterglow
Score require an Apple Watch.

**Q. Do I need to touch the screen during a hot-bath session session?**
No. Once you start a session, measurement continues hands-free — useful with
wet hands or a towel.

**Q. What's the difference between Standard and Simple mode?**
Standard mode tracks distinct phases (sauna → cold plunge → cool-down) per
set. Simple mode runs as one continuous session and detects sets afterwards
from heart-rate peaks.

**Q. What is HRR (HRR1 / HRR3 / HRR5)?**
HRR = Heart Rate Recovery. HRR1 is your heart-rate drop 1 minute after the
peak, HRR3 at 3 minutes, HRR5 at 5 minutes. Higher means faster recovery,
which is the basis for the Afterglow Score.

**Q. What is the recovery slope?**
A Premium analytics metric (bpm/min) — the slope of the linear-fitted central
portion of your recovery curve. Steeper means faster recovery.

**Q. How can I zoom in on the heart rate chart?**
The heart rate chart at the top of the session detail screen is interactive.
Tap any point to display a value card (bpm / elapsed time / phase). Pinch with
two fingers to zoom in (up to 20×) around the tapped position. Double-tap to
reset to full view.

**Q. Can I overlay moving averages on the heart rate chart?**
Yes. Open Settings → Display and toggle on:
- **"60s moving average on HR chart"** — overlays a blue trailing 60-second
  mean. Useful for seeing set-level recovery dynamics without the small
  sample-to-sample noise.
- **"10min moving average on HR chart"** — overlays a red trailing 10-minute
  mean. Useful for the session-wide drift / fatigue baseline.
Both default OFF. Toggle either or both independently. When enabled, the
chart shows a legend at the top.

**Q. Can I hide the preparation phase from the heart rate chart?**
Yes. Settings → Display → **"Hide preparation phase from HR chart"** (default
OFF). When ON, preparation-phase samples (clothes change, body wash, etc.)
are removed from the chart and the X axis re-bases to sauna entry as 0:00,
making the actual sauna portion easier to read. Sessions without a
preparation phase are unaffected.

**Q. What is the Movement Quality score?**
A score (0–100, Excellent / Good / Average / Needs work) that measures how
many heart-rate spikes occur after each hot-phase peak. Long walking distances
between sauna → cold plunge → cool-down area cause HR rebounds; fewer spikes =
better facility flow. The per-session score is shown in session detail (free).
The period-average is also included in the Premium PDF report.

**Q. What is the Sleep Score (reference)?**
A nightly sleep quality score (0–100) computed in-app following Apple's
published watchOS formula (Duration 50 + Bedtime 30 + Interruptions 20). Note:
Apple has not exposed a Sleep Score API in HealthKit, so this is approximated
from sleepAnalysis data and labeled "(reference)" to indicate it is not the
exact value shown in the Apple Health app.

**Q. What is "Exclude walking from recovery" in Settings?**
A Premium toggle, off by default. Apple Watch's distance-based walking
detection sometimes misfires during hot-bath sessions (e.g. flagging sitting or
the cold plunge as "walking"). With the toggle off, recovery slope
calculations use all heart-rate samples. Turning it on excludes samples
flagged as walking — useful only when the Watch's walking detection is
reliable for that session.

**Q. How do I generate a PDF report?**
Premium feature. Tap **Generate PDF report (Premium)** at the top of the
Analytics tab, choose a date range and print background color (light / dark),
then tap "Generate and share". A 3-page A4 portrait report is produced with:
- **Page 1**: sessions summary, Afterglow trend, heart-rate trend (max / min
  / resting), and recovery data (HRR1 / HRR3 / HRR5, peak amplitude,
  movement quality)
- **Page 2**: recovery curve grid (up to 11 sessions, with per-set slope /
  R² / lag annotations) plus a period-average overlay
- **Page 3**: Best Sessions TOP 5, **Recent 11 sessions table** (date / day
  / venue / time / sets / Max HR / HRR1 / HRR3 / HRR5 / rating / score),
  and a calendar visit-frequency heatmap

Share via AirDrop / Mail / Files / Print.

**Q. How does the venue suggestion work?**
When you open a session's detail and the venue field is empty, the app shows
nearby candidates based on the session's GPS location:
- **Past visits** (orange clock icon): venues you previously entered within
  500 m, prioritized at the top.
- **Bath facilities** (blue map-pin icon): nearby spa / sauna / public bath
  found via Apple Maps keyword search (within 500 m).
Tap a suggestion to populate the venue field instantly.

### 4. Troubleshooting

**Q. Watch session data isn't reaching my iPhone.**
Open the MaxRecover app on both devices, keep them nearby with Bluetooth on, and
relaunch both apps. The Watch resends pending data automatically. You can also
trigger a manual resend in iPhone Settings → Apple Watch sync status.

**Q. Heart rate isn't showing on the Watch.**
Make sure the Watch is worn snugly and wrist detection is enabled. Confirm
that you granted Health permissions when first launching the app
(iPhone Settings → Health → Data Access & Devices).

**Q. "Save to Photos" fails after I tap save.**
Check iPhone Settings → MaxRecover → Photos → set to "Add Only" or higher. If
the issue persists, rebuild the app from the App Store update or restart your
iPhone.

**Q. Watch battery drains quickly.**
A 60-minute hot-bath session uses about 10–15% of an Apple Watch Series 7+
battery in our testing. Disable Always-On Display in the Watch system settings
if you need more headroom. The app also auto-ends after 60 minutes of
inactivity to protect the battery.

**Q. Double Tap doesn't respond when the screen is dim.**
This is the standard Apple Watch behavior: while Always-On Display is in its
**dim state**, touch and gesture inputs (including Double Tap) are disabled to
save battery and prevent accidental input. Lift your wrist, lightly turn the
Digital Crown, or wave your other hand over the screen to wake it to full
brightness — then Double Tap will respond. In a real hot-bath session you usually
move when transitioning phases (sauna → plunge, plunge → cool-down chair),
so the screen wakes naturally, but be aware of this if you sit still and try
to tap after a long pause.

**Q. The Afterglow Score didn't appear after my session.**
The score needs valid heart-rate data after the peak. If you ended the session
within 1 minute of the hot-phase peak, or the watch lost contact (dropouts), the
score may be missing. Sessions with too few samples are marked as unscored.

**Q. The app switches away when water hits the Watch screen.**
This is an Apple Watch system behavior — water on the touchscreen registers as
multi-touch input, which can trigger OS-level gestures (Control Center, app
switching, returning to the watch face). The app's own "no screen tap" policy
only blocks taps within the app, not the OS-level gestures. The fix is to enable
**Apple Watch's Water Lock**:

- **In-app setting (recommended)**: iPhone MaxRecover → Settings → Session →
  toggle on "Auto Water Lock in Pre-sauna" and/or "Auto Water Lock in
  Cool-down". The Watch turns on Water Lock automatically when those phases
  start.
- **Manual**: On the Watch, swipe up to open Control Center → tap the 💧
  droplet icon.

To unlock, rotate the Digital Crown (this also ejects water from the speaker
via sound waves — Apple's standard behavior).

### 5. Plank exercise (optional)

**Q. What is the Plank exercise feature?**
A built-in plank timer that you can enable in **Settings → Add-ons → Enable
plank exercise**. When on, a "Plank" tab appears between Analytics and
Settings. Two modes:
- **Countdown**: pick a target between 1 and 30 minutes (1-minute steps).
  After a 3-2-1 pre-countdown, the timer counts down to 0:00. When the
  target is reached, a strong haptic fires and the display switches to
  **bonus time** (count-up) so you can keep going. Double-tap the bottom
  button to stop.
- **Count-up**: starts at 0:00 and runs until you double-tap. Used to
  measure your endurance.

**Q. Does the Apple Watch measure heart rate during a plank?**
Yes. Open MaxRecover on your Watch before starting a plank on iPhone. The
Watch starts an `HKWorkoutSession` (`Core Training`) and streams heart
rate to the iPhone for the whole plank. Each session is also written to
Apple Health as a Core Training workout. If MaxRecover is not running on the
Watch, the iPhone timer still works but no HR is recorded.

**Q. What does the result screen show after a plank?**
- Calories burned (estimated using a 3.8 MET assumption × 65 kg default
  weight × duration in hours)
- Current streak days (consecutive days with at least one plank)
- Personal best seconds
- Total seconds (across all sessions)
- Total days (distinct calendar days with at least one plank)
- Max heart rate observed during the session (if Watch was connected)

**Q. How is the plank trend chart organized?**
1 day = 1 bar showing the **cumulative plank duration** for that day. Color
rules:
- Green: at least one countdown session on that day reached the target
- Blue: all sessions on that day were count-up
- Orange: countdown only, target not reached on any session

A period picker (1 week / 1 month / 3 months / All) lets you focus on a
range. Within a window of 14 days, every day gets a label; for longer
ranges the label stride widens automatically.

**Q. How do I delete an old plank record?**
Swipe a row in the history list to the left and tap the red trash button —
same gesture as sauna history.

**Q. Is Plank a Premium-only feature?**
No, it's a free add-on. The toggle to enable it is in the Settings tab. The
plank tab is invisible unless you turn it on, so it does not crowd the UI
for sauna-only users.

### 5. Other

**Q. Can I use this for medical purposes?**
No. The Afterglow Score, heart-rate values, HRR, and all other figures are
reference information only. They are not medical metrics and must not be used
for diagnosis or treatment decisions. Consult a physician if you have
concerns.

**Q. What is the Recommended use?**
Personal wellness tracking. Use saunas at your own risk and follow your local
sauna's rules. Avoid alcohol before and during sauna use.

**Q. How do I contact support?**
Email **maxsaunatimer@gmail.com**. Please include your iOS / watchOS versions
and a brief description of the issue.

**Q. Where can I find the Privacy Policy and Terms of Use?**
[Privacy Policy](privacy-policy.html) / [Terms of Use](terms-of-use.html).
