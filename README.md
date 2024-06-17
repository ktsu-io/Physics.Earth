# ktsu.io.Physics.Earth

The `ktsu.io.Physics.Earth` library provides a set of classes and methods to work with Earth's physical properties and calculations, including gravity, radius, mass, and volume. It also offers methods for computing gravity at different altitudes and related geophysical quantities.

## Features

- **Gravity at Sea Level**: `Earth.GravityAtSeaLevel`
- **Earth's Radius, Diameter, and Circumference**: `Earth.Radius`, `Earth.Diameter`, `Earth.Circumference`
- **Earth's Mass and Volume**: `Earth.Mass`, `Earth.Volume`
- **Earth's Average Density**: `Earth.Density`
- **Geophysical Calculations**:
  - Gravity at Geometric and Geopotential Altitudes: `Earth.GravityAtAltitude`, `Earth.GravityAtGeopotentialAltitude`
  - Geopotential Altitude Calculation: `Earth.GeopotentialAltitude`
  - Reciprocal Relative Altitude Calculation: `Earth.ReciprocalRelativeAltitude`

## Installation

To install the `ktsu.io.Physics.Earth` library, use the following command:

```sh
dotnet add package ktsu.io.Physics.Earth
```

## Usage

### Basic Properties

```csharp
using ktsu.io.Physics.Earth;
using ktsu.io.PhysicalQuantity.Length;

var gravityAtSeaLevel = Earth.GravityAtSeaLevel;
var earthRadius = Earth.Radius;
var earthDiameter = Earth.Diameter;
var earthMass = Earth.Mass;
var earthVolume = Earth.Volume;
var earthDensity = Earth.Density;
```

### Geophysical Calculations

#### Gravity at Altitude

```csharp
var altitude = 1000.Meters();
var gravityAtAltitude = Earth.GravityAtAltitude(altitude);
```

#### Gravity at Geopotential Altitude

```csharp
var geopotentialAltitude = 1000.Meters();
var gravityAtGeopotentialAltitude = Earth.GravityAtGeopotentialAltitude(geopotentialAltitude);
```

#### Geopotential Altitude Calculation

```csharp
var geometricAltitude = 1000.Meters();
var geopotentialAltitude = Earth.GeopotentialAltitude(geometricAltitude);
```

#### Reciprocal Relative Altitude Calculation

```csharp
var altitude = 1000.Meters();
var reciprocalRelativeAltitude = Earth.ReciprocalRelativeAltitude(altitude);
```

## Contributing

Contributions are welcome! Please fork the repository and submit pull requests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
