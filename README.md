# js_interop
A Flutter project demo for JS Interop.  


## Run Flutter Web localhost
```shell
flutter run -d chrome --web-renderer html

# Run with CORS, Since Flutter 3.3.0
# Áp dụng khi chạy ở localhost nhưng lại gọi lên Staging hoặc Product.
flutter run -d chrome --web-renderer html --web-browser-flag "--disable-web-security"
```

## Build Release Flutter Web.
```shell
flutter clean
flutter build web --web-renderer html --release

# Run
cd  build/web
python3 -m http.server 8787
# Open browser with URL:
http://localhost:8787
```


## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
