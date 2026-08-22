# TASKVN — GitHub APK Build

Đây là project Android WebView tối giản, không dùng Kotlin nên tránh lỗi duplicate Kotlin stdlib.

## Cấu trúc

- `app/` — mã Android
- `build.gradle` — Android Gradle Plugin 8.6.1
- `gradle.properties` — cấu hình Gradle
- `settings.gradle` — cấu hình project
- `.github/workflows/main.yml` — build APK bằng GitHub Actions

## Build APK trên GitHub

1. Upload toàn bộ nội dung ZIP vào repository.
2. Vào **Actions**.
3. Chọn **Build TASKVN APK**.
4. Bấm **Run workflow**.
5. Khi chạy xong, vào phần **Artifacts** và tải `TASKVN-debug-apk`.

## URL WebView

URL hiện tại nằm trong:

`app/src/main/java/com/taskvn/app/MainActivity.java`

Biến:

`HOME_URL`

Đang trỏ tới:

`https://webmmo-vn.netlify.app/`

Nếu muốn đổi web, chỉ cần sửa URL đó.

## Lưu ý

Project này không chứa Firebase key, API key, mật khẩu hoặc token.
