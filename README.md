# QR Code Generator - Android App

A modern and user-friendly Android application for generating, saving, and sharing QR codes. Built with Kotlin and Material Design.

## 📱 Features

✅ **Generate QR Codes** - Convert text or URLs to QR codes instantly
✅ **Beautiful UI** - Material Design with smooth animations
✅ **Save QR Codes** - Save generated QR codes to device storage
✅ **Share QR Codes** - Share via Email, Messaging, Social Media, etc.
✅ **Clear Function** - Reset and start fresh
✅ **Permission Handling** - Proper Android 11+ permission management
✅ **Error Handling** - User-friendly error messages

## 🛠 Tech Stack

- **Language**: Kotlin
- **Minimum SDK**: Android 5.0 (API 21)
- **Target SDK**: Android 14 (API 34)
- **QR Library**: ZXing (com.google.zxing:core)
- **UI Framework**: Material Design Components
- **Build System**: Gradle

## 📦 Dependencies

```gradle
dependencies {
    implementation 'com.google.zxing:core:3.5.3'
    implementation 'com.journeyapps:zxing-android-embedded:4.3.0'
    implementation 'androidx.appcompat:appcompat:1.6.1'
    implementation 'com.google.android.material:material:1.11.0'
}
```

## 🚀 Getting Started

### Prerequisites
- Android Studio (latest version)
- JDK 1.8 or higher
- Android SDK (API 21+)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/241b286-Vijay/Qr-generator-2.git
   cd Qr-generator-2
   ```

2. **Open in Android Studio**
   - Open Android Studio
   - Click "Open an Existing Project"
   - Select the project folder
   - Wait for Gradle sync to complete

3. **Build and Run**
   - Click "Run" or press `Shift + F10`
   - Select your emulator or connected device
   - The app will install and launch

## 📖 Usage

### Generating a QR Code
1. **Enter Text/URL**: Type any text or URL in the input field
2. **Click Generate**: Press the "Generate QR Code" button
3. **View QR Code**: The QR code will appear in the display area

### Saving QR Code
1. Generate a QR code first
2. Click the **Save** button
3. QR code is saved to your device's Pictures folder
4. You'll receive a confirmation message

### Sharing QR Code
1. Generate a QR code first
2. Click the **Share** button
3. Select an app to share with (Email, WhatsApp, Telegram, etc.)
4. The QR code image will be shared

### Clearing
1. Click the **Clear** button to reset the app
2. Input field and QR code display will be cleared

## 📁 Project Structure

```
Qr-generator-2/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── kotlin/
│   │   │   │   └── com/example/qrgenerator/
│   │   │   │       ├── MainActivity.kt
│   │   │   │       └── QRCodeGenerator.kt
│   │   │   ├── res/
│   │   │   │   ├── layout/
│   │   │   │   │   └── activity_main.xml
│   │   │   │   ├── drawable/
│   │   │   │   ├── values/
│   │   │   │   │   ├── strings.xml
│   │   │   │   │   ├── colors.xml
│   │   │   │   │   └── themes.xml
│   │   │   │   └── xml/
│   │   │   │       └── file_paths.xml
│   │   │   └── AndroidManifest.xml
│   │   └── test/
│   └── build.gradle
└── README.md
```

## 🔐 Permissions

The app requests the following permissions:
- `READ_EXTERNAL_STORAGE` - To access device storage (Android 12 and below)
- `WRITE_EXTERNAL_STORAGE` - To save QR codes (Android 12 and below)
- `READ_MEDIA_IMAGES` - To access images (Android 13+)
- `INTERNET` - For potential future features
- `CAMERA` - For potential QR scanning features

## 🎨 UI Components

### Main Activity Layout
- **EditText** - Input field for text/URL
- **ImageView** - Display area for generated QR code
- **Buttons**:
  - Generate (Primary - Purple)
  - Save (Success - Green)
  - Share (Info - Blue)
  - Clear (Danger - Red)

## 🔧 Customization

### Change Colors
Edit `app/src/main/res/values/colors.xml`:
```xml
<color name="primary">#FF6200EE</color>
<color name="success">#FF4CAF50</color>
```

### Change QR Code Size
In `MainActivity.kt`, modify:
```kotlin
currentQRBitmap = QRCodeGenerator.generateQRCode(inputText, 500)
// Change 500 to your desired size
```

## 📝 License

This project is open source and available under the MIT License.

## 👨‍💻 Author

**Vijay** - 241b286-Vijay

## 📧 Contact

For queries or suggestions, feel free to open an issue in the repository.

## 🤝 Contributing

Contributions are welcome! Feel free to submit pull requests.

## 🐛 Bug Reports

If you find any bugs, please create an issue with details.

---

**Happy QR Code Generating! 🎉**
