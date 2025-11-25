# Weather App – Flutter

A visually appealing **Flutter weather application** that shows:

* Current weather (temperature, description, humidity, wind speed, icon)
* 7-day forecast (horizontal scroll)
* Search history (last 5 searched cities)
* Modern UI with gradient backgrounds and weather icons


## **Features**

* Search weather by city name
* Store last searched cities (clickable history)
* Display current weather info: temperature, humidity, wind speed
* 7-day forecast with weather icons
* Gradient background and attractive UI

---

## **Setup Instructions**

### **1. Clone or download the repository**

```bash
git clone <your-repo-url>
cd <your-project-folder>
```

### **2. Install Flutter dependencies**

```bash
flutter pub get
```

Make sure Flutter is installed and added to your PATH.

---

### **3. Add your OpenWeatherMap API Key**

Open `lib/main.dart`, find:

```dart
String apiKey = "Your_public_api_key";
```

Replace the value with your own **OpenWeatherMap API key**.
If you don't have one, register here: [OpenWeatherMap](https://openweathermap.org/api)

---

### **4. Add assets (images)**

Place these images inside your project:

```
assets/images/
  sun.png
  cloud.png
  rain.png
  snow.png
  humidity.png
  wind.png
  background.jpg
```

Make sure your `pubspec.yaml` includes:

```yaml
flutter:
  assets:
    - assets/images/
```

---

### **5. Run the app**

Connect a device or start an emulator, then:

```bash
flutter run
```

---

### **6. Optional**

* To reset the search history, clear app storage or uninstall/reinstall the app.
* Supports up to **5 previous cities** for quick access.

---

## **Dependencies**

* `http: ^1.0.0` – for REST API calls
* `shared_preferences: ^2.1.1` – to store search history
* `flutter` (>=2.0.0)

Add dependencies in `pubspec.yaml`:

```yaml
dependencies:
  flutter:
    sdk: flutter
  http: ^1.0.0
  shared_preferences: ^2.1.1
```

---

### **7. Notes**

* The forecast API provides **3-hour interval data**, so the app calculates **7-day forecast** by picking 8 entries per day.
* UI uses gradient and semi-transparent cards for an attractive look.

---

