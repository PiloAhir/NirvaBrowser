# Nirva Browser (નિર્વા બ્રાઉઝર)

## Build APK with GitHub Actions
1. Upload/extract the project files into the root of your GitHub repository.
2. Ensure `.github/workflows/android.yml` is included.
3. Open **Actions** and run **Build Nirva Browser APK** (or push a commit).
4. Download artifact **Nirva-Browser-debug-apk**.

## Notes
- Uses Android WebView, not a new independent browser engine.
- Search providers receive searches submitted to them.
- Tracker blocking is a limited host blocklist and cannot guarantee complete protection.
- Time-range clearing applies to saved visit history. WebView cookies/cache/site storage can only be reliably cleared together using Clear all data.
- Auto-clear runs when Android backgrounds/stops the activity; force-stop may not trigger cleanup.
- The layout explicitly applies system-bar insets, so app controls start below the status bar and stay above navigation controls.
