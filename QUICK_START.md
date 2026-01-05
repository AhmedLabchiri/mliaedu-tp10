# Quick Start Guide - RestClient Android App

## Project Status: ✅ Code Fixed, Ready for Android Studio

All code errors have been fixed. The project is ready to build in Android Studio.

## Steps to Run:

### 1. Open in Android Studio
```bash
# Open Android Studio and select:
File → Open → /Users/ahmedlabchiri/AndroidStudioProjects/Restclient
```

### 2. Wait for Gradle Sync
- Android Studio will automatically start syncing
- This will download all dependencies (first time takes 2-5 minutes)
- Watch the bottom status bar for "Gradle Sync" progress

### 3. Build the Project
```
Build → Clean Project
Build → Rebuild Project
```

### 4. Run the App
- Start an Android emulator (API 24+) or connect a device
- Click the green "Run" button (▶️)
- Select your device/emulator
- App should launch successfully

## Before Running - Configure Backend:

Edit: `app/src/main/java/ma/projet/config/RetrofitClient.java`

Line 10:
```java
private static final String BASE_URL = "http://10.0.2.2:8082/";
```

**For Android Emulator**: Use `http://10.0.2.2:8082/` (localhost)
**For Physical Device**: Use your computer's IP, e.g., `http://192.168.1.100:8082/`

## Features:

✅ View accounts (JSON/XML format switching)
✅ Add new account
✅ Update account
✅ Delete account
✅ Material Design UI
✅ RecyclerView with adapters
✅ Retrofit REST client

## If Something Goes Wrong:

### "Cannot resolve symbol" errors persist:
```
File → Invalidate Caches / Restart → Invalidate and Restart
```

### Gradle sync fails:
1. Check internet connection
2. Delete `.gradle` folder in project root
3. Restart Android Studio
4. Let it sync again

### App crashes at runtime:
1. Check Android Studio Logcat for errors
2. Verify backend server is running
3. Test backend URL in browser first

## Backend Expected Format:

### JSON Response (GET /banque/comptes):
```json
[
  {
    "id": 1,
    "solde": 1000.0,
    "type": "COURANT",
    "dateCreation": "2024-01-01"
  }
]
```

### XML Response (GET /banque/comptes):
```xml
<List>
  <item>
    <id>1</id>
    <solde>1000.0</solde>
    <type>COURANT</type>
    <dateCreation>2024-01-01</dateCreation>
  </item>
</List>
```

## Need Help?

See `FIXES_APPLIED.md` for detailed information about all changes made.

