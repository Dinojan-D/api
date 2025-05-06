# Celestial Bodies API

This API provides information about various celestial bodies in our solar system. It includes data on planets, moons, dwarf planets, asteroids, and the Sun. The data is structured in a way to support simulation and astronomical applications.

```
https://github.com/Dinojan-D/api/new/main/data/solar-system/bodies.json
```

## Properties

Each celestial body contains the following properties:

- **name** (string): The name of the celestial body (e.g., "Sun", "Earth", "Moon").
- **type** (string): The type of the celestial body, which can be one of the following:
  - "Star" (for stars like the Sun)
  - "Planet" (for planets like Earth or Mars)
  - "Moon" (for natural satellites like the Moon or Io)
  - "Dwarf Planet" (for bodies like Ceres)
  - "Asteroid" (for objects like Vesta or Pallas)
  
- **mass_kg** (number): The mass of the celestial body in kilograms (kg).
- **radius_km** (number): The radius of the celestial body in kilometers (km).
- **gravity_m_s2** (number): The gravitational acceleration on the surface of the celestial body in meters per second squared (m/s²).
- **rotation_period_hours** (number): The time it takes for the celestial body to complete one full rotation in hours (h).
- **orbital_period_days** (number, optional): The orbital period of the body in Earth days. This is relevant for planets, moons, and dwarf planets.
- **distance_from_parent_km** (number, optional): The distance from the celestial body to its parent body (e.g., the distance from the Earth to the Sun for the Earth, or from a moon to its planet). For planets and asteroids, this distance is measured from the **Sun**. For moons, this distance is from their **planet**.
- **has_rings** (boolean, optional): A flag indicating whether the celestial body has rings (relevant for planets like Saturn, Jupiter, etc.).
- **parent** (string, optional): The name of the parent celestial body (only for moons). For example, the Moon has Earth as its parent.

## Celestial Bodies

### Number of Planets:
There are **8** planets in the solar system:
- Mercury
- Venus
- Earth
- Mars
- Jupiter
- Saturn
- Uranus
- Neptune

### Number of Moons:
There are several important moons listed in the database, including:
- **Earth's Moon**
- **Jupiter's Moons** (Io, Europa, Ganymede)
- **Saturn's Moon** (Titan)
  
In total, there are **5** major moons (not counting smaller moons).

### Number of Asteroids:
The database includes the following notable asteroids:
- Ceres (Dwarf Planet, but considered an asteroid)
- Vesta
- Pallas
- Hygiea

In total, there are **4** major asteroids listed.

## Notes on Distances:
- The **distance_from_parent_km** for **planets** and **asteroids** is expressed as the distance from the **Sun**.
- The **distance_from_parent_km** for **moons** is expressed as the distance from their **parent planet**.
- All distances are in kilometers (km).

## Example Data

### Sun (Star)
```json
{
  "name": "Sun",
  "type": "Star",
  "mass_kg": 1.9885e30,
  "radius_km": 695700,
  "gravity_m_s2": 274,
  "rotation_period_hours": 609.12
}
