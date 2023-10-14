# Hubitat-InfluxDB-Logger

## Installation

### HPM Installation

This app can now be installed with [HPM](https://hubitatpackagemanager.hubitatcommunity.com/). HPM will detect updates and offer to apply them.

Click 'Install', 'From URL', and enter `https://raw.githubusercontent.com/aerickson/Hubitat-InfluxDB-Logger/master/influxdb-logger.groovy`.

### Manual Installation

See https://docs2.hubitat.com/how-to/install-custom-apps for a general overview.

## Common Errors

### Null Pointer Exception: Cannot invoke method getDisplayName()

```java
app:5282023-10-13 12:14:14.857 AMerrorjava.lang.NullPointerException: Cannot invoke method getDisplayName() on null object on line 367 (method updated)
```

This is due to deleting a device that was in use by the app.

To fix, in the app's config try updating the device group where the deleted device was.

## History

most recent at end

- Forked from: https://github.com/codersaur/SmartThings/tree/master/smartapps/influxdb-logger
  - Original Author: David Lomas (codersaur)
- Forked from https://github.com/HubitatCommunity/InfluxDB-Logger
