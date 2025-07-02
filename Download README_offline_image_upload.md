
# Offline Image Upload with In-Memory Storage in Flutter

## ✅ Objective
This Flutter app allows users to select and upload an image, even when offline. The image is stored in memory (RAM) and automatically uploaded when internet connectivity is restored.

## 🚀 How to Run

1. Clone the repo or extract the ZIP.
2. Run `flutter pub get`
3. Connect a device/emulator
4. Run: `flutter run`

## 🛠️ Packages Used

| Package             | Purpose                         |
|---------------------|----------------------------------|
| `image_picker`      | To select image from gallery     |
| `connectivity_plus` | Monitor internet connectivity    |
| `provider`          | Manage in-memory image state     |
| `http`              | Upload to mock endpoint          |

## ✨ Features

- Pick image from gallery
- Detect internet status in real time
- Save image temporarily in memory if offline
- Upload automatically once internet is back
- Show upload status: Pending, Uploading, Success, Failed
- Retry option for failed uploads

## 🌐 Upload Endpoint

Using `https://httpbin.org/post` as mock server for `multipart/form-data` image upload.

## ⚠️ Limitations

- Only single image upload supported (multi-image is optional)
- No local file or DB storage
- No persistent memory across app restarts

## 📹 Submission Instructions

- Record your screen:
  - Show image selection while offline
  - Reconnect internet and show auto-upload
  - Walkthrough code
- Upload video to Google Drive
- Rename like: `yourname_flutter_assignment.mp4`

Example Drive links:
```
project-features : https://drive.google.com/yourname_flutter_assignment_1.mp4
project-technical : https://drive.google.com/yourname_flutter_assignment_2.mp4
```

## 🏆 Optional Improvements

- Multiple image queue (FIFO)
- Local notifications via `flutter_local_notifications`
