# custom_component to get info about next launches.
  
![Version](https://img.shields.io/badge/version-1.0.1-green.svg?style=for-the-badge) ![mantained](https://img.shields.io/maintenance/yes/2018.svg?style=for-the-badge) A platform which allows you to get information from alerts.weather.gov. 
  
To get started put `/custom_components/sensor/launchlibrary.py` here:  
`<config directory>/custom_components/sensor/launchlibrary.py`  
  
**Example configuration.yaml:**
```yaml
sensor:
  platform: launchlibrary
  sameid: 2190400
```
**Configuration variables:**  
  
key | description  
:--- | :---  
**platform (Required)** | The platform name.  
  
#### Sample overview
![Sample overview](overview.png)
  
[Home-Assistant demo site.](https://ha-test-launchlibrary.halfdecent.io)
  
  
This platform is using the [launchlibrary.net](http://launchlibrary.net/) API to get the information.  
Due to how `custom_componentes` are importerd, it is normal to see a `ModuleNotFoundError` error on first boot after adding this, to resolve it, restart Home-Assistant.