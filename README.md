# Flutter Simple Map

Flutter plugin to display animated points on world map in real time mode.
It could be also helpful as a presentation of some online users, devices, etc.

![1.gif](screens/1.gif)
![2.gif](screens/2.gif)

## Getting Started

* Add this to pubspec.yaml file
  ```
  dependencies:
  world_map: ^1.0.0
  ```
* Get the package from Pub:
  ```
  flutter packages get
  ```
* Import it in your file
  ```
  import 'package:world_map/world_map.dart';
  ```

## Features

* Render simple customizable flat map
* Render points with animation effect
* Customize every point
* Create points
* Clear map

## Usage

* Change Map Options - map, map color, points color
```dart
final mapOptions = SimpleMapOptions(
    mapAsset: 'assets/map.png',
    mapColor: Colors.grey,
    bgColor: Colors.black,
);
```

* Using SimpleMapController
```dart
final SimpleMapController mapController = SimpleMapController();

mapController.addPoint(SimpleMapPoint());
mapController.points = [SimpleMapPoint()];
mapController.clear();

SimpleMap(
  controller: mapController,
  options: mapOptions,
),
```

* Check out the complete example in github


## License

* MIT License Daniil Shilintsev