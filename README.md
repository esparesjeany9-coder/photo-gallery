# Ionic Photo Gallery

A mobile photo gallery application built with Ionic, Vue 3, and Capacitor.

## Features

- 📸 Capture photos using device camera
- 🖼️ Browse and display photos in a gallery
- 💾 Save photos locally
- 📱 Cross-platform support (iOS/Android)
- ⚡ Built with Vue 3 + TypeScript

## Installation

### Prerequisites
- Node.js v26.8.1 or higher
- npm v11.19.0 or higher
- Ionic CLI v7.2.1 or higher

### Steps

1. Clone the repository:
```bash
git clone https://github.com/esparesjeany9-coder/photo-gallery.git
cd photo-gallery
```

2. Install dependencies:
```bash
npm install
```

3. Install Ionic PWA Elements:
```bash
npm install @ionic/pwa-elements
```

## Development

### Run in browser:
```bash
ionic serve
```

### Build for Android:
```bash
ionic build
npx cap sync android
cd android
./gradlew assembleDebug
```

### Build for iOS:
```bash
ionic build
npx cap sync ios
```

## Project Structure

```
photo-gallery/
├── src/
│   ├── components/
│   │   ├── CameraComponent.vue
│   │   └── PhotoGalleryComponent.vue
│   ├── views/
│   │   └── HomePage.vue
│   └── App.vue
├── android/              # Capacitor Android native project
├── .github/
│   └── workflows/
│       └── build-apk.yml # GitHub Actions for APK builds
├── public/
├── tests/
└── package.json
```

## GitHub Actions

Automatic APK builds are configured in `.github/workflows/build-apk.yml`. Every push to the `main` branch will trigger an Android build.

## License

MIT

## Author

MALOU ADAY
