# GPS Drivers

This repository contains user-space gps drivers, used as a submodule in
[PX4-Autopilot](https://github.com/PX4/PX4-Autopilot) and
[QGroundControl](https://github.com/mavlink/qgroundcontrol).

All platform-specific stuff is done via a callback function and a
`definitions.h` header file.

In order for the project to build, `definitions.h` must include definitions for `sensor_gnss_relative_s`, `sensor_gps_s` and `satellite_info_s`.

## Parser tests

To test parsers, build and run the cmake project:

```
cmake -Bbuild -H.
cmake --build build && build/gps-parser-test
```

👨‍💻 Maintainer
```bash
Udit Ray
Email: udit.ray@indowings.com
Org: Indo Wings Private Limited
Website: https://www.indowings.com
