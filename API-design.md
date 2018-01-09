# API Design
The API will be designed as follows:
```

let device = manager.getDevices()[0];
device.endpoints;

manager.onDeviceAdd((device) => {
    device.onEndpointUpdate((endpoints) => {
        my.endpoints = endpoints;
    });
});


let device = manager.getDevices()[0];
device.endpoints;

gpio.onChange((newValue) => {
    manager.getDevice(self).setBrightness(newValue);
})

while true:
    manager.tick();
```
