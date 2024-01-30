# WindAeroTwoDimIEC


_Two-dimensional aerodynamic model.  _

_Reference: IEC 61400-27-1:2015, 5.6.1.3._





**URI**: [cim:WindAeroTwoDimIEC](http://iec.ch/TC57/CIM100#WindAeroTwoDimIEC)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindAeroTwoDimIEC
      IdentifiedObject <|-- WindAeroTwoDimIEC
      
      WindAeroTwoDimIEC : IdentifiedObject.description
        
      WindAeroTwoDimIEC : WindAeroTwoDimIEC.dpomega
        
          WindAeroTwoDimIEC --> PU : WindAeroTwoDimIEC.dpomega
        
      WindAeroTwoDimIEC : WindAeroTwoDimIEC.dptheta
        
          WindAeroTwoDimIEC --> PU : WindAeroTwoDimIEC.dptheta
        
      WindAeroTwoDimIEC : WindAeroTwoDimIEC.dpv1
        
          WindAeroTwoDimIEC --> PU : WindAeroTwoDimIEC.dpv1
        
      WindAeroTwoDimIEC : IdentifiedObject.mRID
        
      WindAeroTwoDimIEC : IdentifiedObject.name
        
      WindAeroTwoDimIEC : WindAeroTwoDimIEC.omegazero
        
          WindAeroTwoDimIEC --> PU : WindAeroTwoDimIEC.omegazero
        
      WindAeroTwoDimIEC : WindAeroTwoDimIEC.pavail
        
          WindAeroTwoDimIEC --> PU : WindAeroTwoDimIEC.pavail
        
      WindAeroTwoDimIEC : WindAeroTwoDimIEC.thetav2
        
          WindAeroTwoDimIEC --> AngleDegrees : WindAeroTwoDimIEC.thetav2
        
      WindAeroTwoDimIEC : WindAeroTwoDimIEC.thetazero
        
          WindAeroTwoDimIEC --> AngleDegrees : WindAeroTwoDimIEC.thetazero
        
      WindAeroTwoDimIEC : WindAeroTwoDimIEC.WindTurbineType3IEC
        
          WindAeroTwoDimIEC --> WindTurbineType3IEC : WindAeroTwoDimIEC.WindTurbineType3IEC
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **WindAeroTwoDimIEC**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| dpomega | [cim:WindAeroTwoDimIEC.dpomega](http://iec.ch/TC57/CIM100#WindAeroTwoDimIEC.dpomega) | 1..1 <br />  [PU](PU.md)  | Partial derivative of aerodynamic power with respect to changes in WTR speed ... | direct |
| dptheta | [cim:WindAeroTwoDimIEC.dptheta](http://iec.ch/TC57/CIM100#WindAeroTwoDimIEC.dptheta) | 1..1 <br />  [PU](PU.md)  | Partial derivative of aerodynamic power with respect to changes in pitch angl... | direct |
| dpv1 | [cim:WindAeroTwoDimIEC.dpv1](http://iec.ch/TC57/CIM100#WindAeroTwoDimIEC.dpv1) | 1..1 <br />  [PU](PU.md)  | Partial derivative (<i>dp</i><i><sub>v1</sub></i>) | direct |
| omegazero | [cim:WindAeroTwoDimIEC.omegazero](http://iec.ch/TC57/CIM100#WindAeroTwoDimIEC.omegazero) | 1..1 <br />  [PU](PU.md)  | Rotor speed if the wind turbine is not derated (<i>omega</i><i><sub>0</sub></... | direct |
| pavail | [cim:WindAeroTwoDimIEC.pavail](http://iec.ch/TC57/CIM100#WindAeroTwoDimIEC.pavail) | 1..1 <br />  [PU](PU.md)  | Available aerodynamic power (<i>p</i><i><sub>avail</sub></i><i>)</i> | direct |
| thetazero | [cim:WindAeroTwoDimIEC.thetazero](http://iec.ch/TC57/CIM100#WindAeroTwoDimIEC.thetazero) | 1..1 <br />  [AngleDegrees](AngleDegrees.md)  | Pitch angle if the wind turbine is not derated (<i>theta</i><i><sub>0</sub></... | direct |
| thetav2 | [cim:WindAeroTwoDimIEC.thetav2](http://iec.ch/TC57/CIM100#WindAeroTwoDimIEC.thetav2) | 1..1 <br />  [AngleDegrees](AngleDegrees.md)  | Blade angle at twice rated wind speed (<i>theta</i><i><sub>v2</sub></i>) | direct |
| WindTurbineType3IEC | [cim:WindAeroTwoDimIEC.WindTurbineType3IEC](http://iec.ch/TC57/CIM100#WindAeroTwoDimIEC.WindTurbineType3IEC) | 1..1 <br />  [WindTurbineType3IEC](WindTurbineType3IEC.md)  | Wind turbine type 3 model with which this wind aerodynamic model is associate... | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [WindTurbineType3IEC](WindTurbineType3IEC.md) | WindAeroTwoDimIEC | range | [WindAeroTwoDimIEC](WindAeroTwoDimIEC.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WindAeroTwoDimIEC |
| native | this:WindAeroTwoDimIEC |




