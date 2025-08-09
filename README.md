# DTS Test Projects – Case-ID: 15374981

Two minimal versions of the Guitar Jam Track app for reproducing a crash-on-launch
seen in Apple’s review environment (iPad Air 5th Gen, iPadOS 18.6).

## Archives

- **/clean** – Project with only the necessary functionality to load `HomeViewController`.  
  Size: <50 MB. Compiles and runs locally without crash.
- **/no-content** – Full project without media/content assets.  
  Size: <50 MB. Compiles and runs locally without crash.

## Build & Run

1. Open `.xcodeproj` in Xcode 15.x.
2. Select any iPad target (arm64).
3. Run on a physical iPad device.
4. Observe that both versions launch successfully locally.

## Expected vs Actual

- **Expected:** Launches normally.
- **Actual in Review Environment:** Immediate crash at launch with `EXC_BAD_ACCESS (Address size fault)`.

## Notes

Crash logs in repo.
