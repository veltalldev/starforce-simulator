# MapleStory StarForce Simulator

## Overview

This project is a WIP **Dart/Flutter** application that simulates the upgrading process of equipment in an MMORPG called MapleStory. The simulator models various features such as upgrade success rates, failure consequences, destruction events, safeguard options, and event-driven modifications (like Star Catching, pity system, and cost discounts).

You can input equipment properties like the level, initial stars, target stars, and the number of trials, and the simulator will run those trials, providing detailed statistics including success rates, destruction rates, and resource costs, etc.

## Features

- Simulates equipment upgrades with various outcomes (success, failure, destruction)
- Handles special event features like Star Catching, 5/10/15 guaranteed success events, and a 30% discount event
- Support for safeguard options during high-risk upgrade stages
- Outputs statistics on success, failure, destruction, and total resource cost for visualization
- Configurable input parameters: equipment level, initial stars, target stars, number of trials

## Directory Structure
```
/equipment_upgrade_simulator/
│
├── /lib/
│   ├── /models/                     # Data models (equipment, upgrade logic)
│   ├── /services/                   # Core simulator logic
│   ├── /utils/                      # Helper functions (probability, costs)
│   ├── /widgets/                    # UI components (if building a Flutter UI)
│   └── main.dart                    # Main Flutter app file
│
├── /test/                           # Unit tests for the simulator
│   └── upgrade_simulator_test.dart
│
├── /assets/                         # Assets (if needed)
├── /data/                           # Data storage (optional)
├── pubspec.yaml                     # Project dependencies
└── README.md                        # Project documentation (this file)
```
## Getting Started

### Prerequisites

To run this project, you will need:

- [Dart SDK](https://dart.dev/get-dart) installed on your machine.
- [Flutter SDK](https://flutter.dev/docs/get-started/install) if you're building a UI.
- A code editor like [VSCode](https://code.visualstudio.com/) or [Android Studio](https://developer.android.com/studio).

### Setup

1. Clone this repository:
   git clone https://github.com/yourusername/equipment_upgrade_simulator.git
   cd equipment_upgrade_simulator

2. Install dependencies:
   flutter pub get  # For Flutter

### Running the Simulator

To run the core simulation logic:

1. Open **lib/simulation/run_simulation.dart** and adjust the input parameters (e.g., `equipmentLevel`, `trialSize`, `initialStar`, `targetStar`).

2. Run the Dart file:
   dart lib/simulation/run_simulation.dart

### Running Unit Tests

To run unit tests:

1. Write your tests in the **test/** directory.
2. Run the tests with:
   dart test

## Future Plans

- Integrate UI components using Flutter for easy visualization of the results.
- Add graphing functionality to display statistics in charts (success rates, failure events, etc.).
- Improve customization options for event toggles and simulator settings.

## Contributing

Feel free to contribute by submitting issues or pull requests. Make sure to run the unit tests before making any changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
