# Quicksilver

Primarily model enterprise storage cost and growth over a forecast horizon. 
The model can be adapted for unique requirements such as migrating between systems or archiving a percentage of storage. 
The model can be used to model storage strategy over a forecast horizon. 

## Required Data
This is a standard set of variables that may or may not exist at the time but the model can be adapted accordingly. 

### Storage Parameters
Variable |	Definition |
--- | --- | 
Storage Category | e.g. cloud, VMAX, |
Vendor | Storage vendor |
Array | Array Name |
Connected Devices | Devices connected to the Array |
Connected Devices CPU Type | |
Model Name | Storage Device Name |
Purchase Date | To calculate depreciation |
LUN | The LUNS within the storage device |
LUN Capacity | Capacity of the LUNs for modelling|
Location | Location of the storage devices for modelling |
Mirror | The mirror device needs to be considered when modelling storage |
Business Area | To work out storage of each area|
Is Hypervisor | |

### Finance Parameters
Variable | Definition |
--- | --- |
Depreciation | Period / Percentage |
Storage Forecast Growth by Area | |
Cost per GB by Area | |
Cost Deprecation | |

## Reports

![Alt](https://raw.githubusercontent.com/klameer/blog/master/quicksilver/P1.PNG)

![Alt](https://raw.githubusercontent.com/klameer/blog/master/quicksilver/P2.PNG)
