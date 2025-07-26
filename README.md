# Expense Tracker

A cross-platform Flutter application to manage personal expenses. It lets you log daily spending, visualize totals in a bar chart, and keep your budget on track.

![screenshot](web/preview.png)

---

## Features

* Add new expenses with a title, amount, category and date
* Real-time bar chart summarizing expenditure per category
* Responsive UI – adapts between portrait phones and wider tablets/desktop (web)
* Swipe-to-delete with SnackBar undo
* State persisted in memory (easily swappable for a database or API)
* Material 3 theming with dedicated light & dark color schemes

## Demo

Run the project on any Flutter-supported device:

```bash
flutter pub get
flutter run   # chooses a connected device or opens Chrome for web
```

---

## Getting Started

1. **Install Flutter** – Follow the [official guide](https://docs.flutter.dev/get-started/install) and ensure you have Flutter 3+.
2. **Clone the project**
   ```bash
   git clone https://github.com/your-username/expense_tracker.git
   cd expense_tracker
   ```
3. **Fetch packages**
   ```bash
   flutter pub get
   ```
4. **Launch**
   ```bash
   flutter run
   ```
   Specify `-d chrome` or a simulator ID to target a platform.

### Platform-specific builds

```bash
flutter build apk        # Android
flutter build ios        # iOS (requires macOS)
flutter build web        # Web release build in /build/web
```

---

## Project Structure

```
lib/
├── main.dart                # Entry point & theme definitions
├── expenses.dart            # Root page with navigation & state
├── models/
│   └── expense.dart         # Expense model & helpers
└── widgets/                 # Presentation layer
    ├── chart/               # Category bar chart
    └── expenses_list/       # List, item & form widgets
```

*`assets/` can be added in `pubspec.yaml` for images or JSON as needed.*

---

## Dependencies

| Package | Purpose |
| ------- | ------- |
| `uuid`  | Generates unique IDs for each expense |
| `intl`  | Date formatting across locales |
| `cupertino_icons` | iOS-style icons |

All versions are controlled in `pubspec.yaml`.

---

## Contributing

Pull requests are welcome! Please:

1. Create a feature branch (`git checkout -b feature/my-feature`).
2. Run `flutter analyze` to pass static analysis.
3. Write/adjust tests in `test/` if necessary.
4. Open a PR with a clear description of the change.

---

## License

This project is licensed under the MIT License – see `LICENSE` for details.

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
