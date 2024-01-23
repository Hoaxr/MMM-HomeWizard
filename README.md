# MMM-HomeWizard

This is a module for the [MagicMirror²](https://github.com/MichMich/MagicMirror/).

Module to get information out of the P1 Meter (https://www.homewizard.com/p1-meter/)

## Using the module

To use this module, add the following configuration block to the modules array in the `config/config.js` file:
```js
var config = {
    modules: [
        // Home Wizard
        {
                module: "MMM-HomeWizard",
                position: "right",
                header: "Electricity & Gas",
                config: {
                        url: "http://{P1_METER_IP}/api/v1/data",
                        updateInterval: 2000
                }
        },
    ]
}
```

## Configuration options

| Option           | Description
|----------------- |-----------
| `url`        | *Required* Change to the IP of the P1 Meter
| `updateInterval`        | *Optional* DESCRIPTION HERE TOO <br><br>**Type:** `int`(milliseconds) <br>Default 2000 milliseconds (2 seconds)
