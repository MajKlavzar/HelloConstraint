# HelloConstraint

**HelloConstraint** is an Android application developed as part of a coursework project focusing on UI layouts using `ConstraintLayout`. The app demonstrates vertical chains, click event handling, dynamic button background color changes, and layout adaptation for different screen orientations and device sizes.

---

## Features

- **Toast Button (`Toast`)**:
  - Displays a short notification (*Toast message*) with the text `"Hello Toast!"`.

- **Count Button (`Count`)**:
  - Increments the counter value shown in `show_count` by `1` with each click.
  - **Dynamic Background Color (Even/Odd)**:
    - Changes its background color to green (`Color.GREEN`) when the count is **even**.
    - Changes its background color to cyan (`Color.CYAN`) when the count is **odd**.
  - **Zero Button Activation**:
    - Updates the background color of the `Zero` button to magenta (`Color.MAGENTA`) when count is incremented, indicating that the reset action is active.

- **Zero Button (`Zero`)**:
  - Resets the counter value back to `0`.
  - Restores its own background color back to the default gray (`Color.GRAY`).

- **Responsive Layout Variations**:
  - **Portrait Orientation** (`res/layout/activity_main.xml`): Vertically chained buttons aligned on the left side of the count display.
  - **Landscape Orientation** (`res/layout-land/activity_main.xml`): Optimized layout for horizontal device orientation.
  - **Large Screens / Tablets** (`res/layout-xlarge/activity_main.xml`): Adapted layout with larger margins and font sizes for tablet screens.

---

## Project Structure

```
HelloConstraint/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/helloconstraint/
│   │   │   │   └── MainActivity.java          # Main activity logic & click handlers
│   │   │   ├── res/
│   │   │   │   ├── layout/
│   │   │   │   │   └── activity_main.xml      # Default (portrait) layout
│   │   │   │   ├── layout-land/
│   │   │   │   │   └── activity_main.xml      # Landscape orientation layout
│   │   │   │   ├── layout-xlarge/
│   │   │   │   │   └── activity_main.xml      # Large screens / tablets layout
│   │   │   │   └── values/
│   │   │   │       ├── colors.xml             # Color resources
│   │   │   │       └── strings.xml            # String resources
│   │   └── test/                              # Unit tests
│   └── build.gradle.kts                       # Module-level Gradle configuration
└── README.md
```

---

## Requirements & Setup

### Requirements
- **Language**: Java
- **Min SDK**: API 24 (Android 7.0)
- **Target / Compile SDK**: API 35
- **UI Libraries**: `androidx.constraintlayout:constraintlayout` & `com.google.android.material:material`

### How to Run
1. Clone or open the project in **Android Studio**.
2. Wait for the **Gradle Sync** to finish.
3. Launch the app on an Android emulator or physical device by clicking **Run** (`Shift + F10`).
