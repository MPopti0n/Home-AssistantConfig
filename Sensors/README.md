# SENEYE sensor

Seneye is an aquarium water multi-sensor that decline in 3 versions (at the moment of writing this!).
The readings can include (depending on the model):

- Temperature
- pH
- NH3
- NH4 (ammonia)
- Dissolved O2 potential
- LUX, PAR, Kelvin
- Day/Night cycle
- In/Out water

Documentation on the Seneye api can be found here : https://api.seneye.com/


### 1. Get your device ID

Type this in your browser : https://api.seneye.com/v1/devices?user=***&pwd=***

*Replace the "* * *" by the username and password you are using to login at https://www.seneye.me/*

You should get something like this :
```
<response>
  <device>
    <id>YOUR_DEVICE_ID</id>                                <--- THIS IS THE NUMBER WE NEED!
    <description>YOUR_DEVICE_FRIENDLY_NAME</description>
    <type>3</type>
    <time_diff>0</time_diff>
  </device>
</response>
```

### 2. Create the sensors

Copy and past the code from :
- Seneye.yalm
  - Basic

OR

- SeneyeWithTemplate
  - Basic + Icons changing on min/max/critical values