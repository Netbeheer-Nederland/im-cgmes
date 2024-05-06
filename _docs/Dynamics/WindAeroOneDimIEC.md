# WindAeroOneDimIEC


_One-dimensional aerodynamic model.  _

_Reference: IEC 61400-27-1:2015, 5.6.1.2._





**URI**: [cim:WindAeroOneDimIEC](http://iec.ch/TC57/CIM100#WindAeroOneDimIEC)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindAeroOneDimIEC
    click WindAeroOneDimIEC href "../WindAeroOneDimIEC"
      IdentifiedObject <|-- WindAeroOneDimIEC
        click IdentifiedObject href "../IdentifiedObject"
      
      WindAeroOneDimIEC : IdentifiedObject.description
        
      WindAeroOneDimIEC : WindAeroOneDimIEC.ka
        
      WindAeroOneDimIEC : IdentifiedObject.mRID
        
      WindAeroOneDimIEC : IdentifiedObject.name
        
      WindAeroOneDimIEC : WindAeroOneDimIEC.thetaomega
        
          WindAeroOneDimIEC --> AngleDegrees : WindAeroOneDimIEC.thetaomega
          click AngleDegrees href "../AngleDegrees"
        
      WindAeroOneDimIEC : WindAeroOneDimIEC.WindTurbineType3IEC
        
          WindAeroOneDimIEC --> WindTurbineType3IEC : WindAeroOneDimIEC.WindTurbineType3IEC
          click WindTurbineType3IEC href "../WindTurbineType3IEC"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **WindAeroOneDimIEC**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ka | [cim:WindAeroOneDimIEC.ka](http://iec.ch/TC57/CIM100#WindAeroOneDimIEC.ka) | 1 <br />  float  | Aerodynamic gain (<i>k</i><i><sub>a</sub></i>) | direct |
| thetaomega | [cim:WindAeroOneDimIEC.thetaomega](http://iec.ch/TC57/CIM100#WindAeroOneDimIEC.thetaomega) | 1 <br />  [AngleDegrees](AngleDegrees.md)  | Initial pitch angle (<i>theta</i><i><sub>omega0</sub></i>) | direct |
| WindTurbineType3IEC | [cim:WindAeroOneDimIEC.WindTurbineType3IEC](http://iec.ch/TC57/CIM100#WindAeroOneDimIEC.WindTurbineType3IEC) | 1 <br />  [WindTurbineType3IEC](WindTurbineType3IEC.md)  | Wind turbine type 3 model with which this wind aerodynamic model is associate... | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [WindTurbineType3IEC](WindTurbineType3IEC.md) | WindAeroOneDimIEC | range | [WindAeroOneDimIEC](WindAeroOneDimIEC.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WindAeroOneDimIEC |
| native | this:WindAeroOneDimIEC |




