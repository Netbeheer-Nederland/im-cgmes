# WindMechIEC


_Two mass model._

_Reference: IEC 61400-27-1:2015, 5.6.2.1._





**URI**: [cim:WindMechIEC](http://iec.ch/TC57/CIM100#WindMechIEC)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindMechIEC
    click WindMechIEC href "../WindMechIEC"
      IdentifiedObject <|-- WindMechIEC
        click IdentifiedObject href "../IdentifiedObject"
      
      WindMechIEC : WindMechIEC.cdrt
        
          WindMechIEC --> PU : WindMechIEC.cdrt
          click PU href "../PU"
        
      WindMechIEC : IdentifiedObject.description
        
      WindMechIEC : WindMechIEC.hgen
        
          WindMechIEC --> Seconds : WindMechIEC.hgen
          click Seconds href "../Seconds"
        
      WindMechIEC : WindMechIEC.hwtr
        
          WindMechIEC --> Seconds : WindMechIEC.hwtr
          click Seconds href "../Seconds"
        
      WindMechIEC : WindMechIEC.kdrt
        
          WindMechIEC --> PU : WindMechIEC.kdrt
          click PU href "../PU"
        
      WindMechIEC : IdentifiedObject.mRID
        
      WindMechIEC : IdentifiedObject.name
        
      WindMechIEC : WindMechIEC.WindTurbineType1or2IEC
        
          WindMechIEC --> WindTurbineType1or2IEC : WindMechIEC.WindTurbineType1or2IEC
          click WindTurbineType1or2IEC href "../WindTurbineType1or2IEC"
        
      WindMechIEC : WindMechIEC.WindTurbineType3IEC
        
          WindMechIEC --> WindTurbineType3IEC : WindMechIEC.WindTurbineType3IEC
          click WindTurbineType3IEC href "../WindTurbineType3IEC"
        
      WindMechIEC : WindMechIEC.WindTurbineType4bIEC
        
          WindMechIEC --> WindTurbineType4bIEC : WindMechIEC.WindTurbineType4bIEC
          click WindTurbineType4bIEC href "../WindTurbineType4bIEC"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **WindMechIEC**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| cdrt | [cim:WindMechIEC.cdrt](http://iec.ch/TC57/CIM100#WindMechIEC.cdrt) | 1 <br />  [PU](PU.md)  | Drive train damping (<i>c</i><i><sub>drt</sub></i><i>)</i> | direct |
| hgen | [cim:WindMechIEC.hgen](http://iec.ch/TC57/CIM100#WindMechIEC.hgen) | 1 <br />  [Seconds](Seconds.md)  | Inertia constant of generator (<i>H</i><i><sub>gen</sub></i>) (&gt;= 0) | direct |
| hwtr | [cim:WindMechIEC.hwtr](http://iec.ch/TC57/CIM100#WindMechIEC.hwtr) | 1 <br />  [Seconds](Seconds.md)  | Inertia constant of wind turbine rotor (<i>H</i><i><sub>WTR</sub></i>) (&gt;=... | direct |
| kdrt | [cim:WindMechIEC.kdrt](http://iec.ch/TC57/CIM100#WindMechIEC.kdrt) | 1 <br />  [PU](PU.md)  | Drive train stiffness (<i>k</i><i><sub>drt</sub></i>) | direct |
| WindTurbineType3IEC | [cim:WindMechIEC.WindTurbineType3IEC](http://iec.ch/TC57/CIM100#WindMechIEC.WindTurbineType3IEC) | 0..1 <br />  [WindTurbineType3IEC](WindTurbineType3IEC.md)  | Wind turbine type 3 model with which this wind mechanical model is associated | direct |
| WindTurbineType1or2IEC | [cim:WindMechIEC.WindTurbineType1or2IEC](http://iec.ch/TC57/CIM100#WindMechIEC.WindTurbineType1or2IEC) | 0..1 <br />  [WindTurbineType1or2IEC](WindTurbineType1or2IEC.md)  | Wind generator type 1 or type 2 model with which this wind mechanical model i... | direct |
| WindTurbineType4bIEC | [cim:WindMechIEC.WindTurbineType4bIEC](http://iec.ch/TC57/CIM100#WindMechIEC.WindTurbineType4bIEC) | 0..1 <br />  [WindTurbineType4bIEC](WindTurbineType4bIEC.md)  | Wind turbine type 4B model with which this wind mechanical model is associate... | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [WindGenTurbineType1aIEC](WindGenTurbineType1aIEC.md) | WindMechIEC | range | [WindMechIEC](WindMechIEC.md) |
| [WindGenTurbineType1bIEC](WindGenTurbineType1bIEC.md) | WindMechIEC | range | [WindMechIEC](WindMechIEC.md) |
| [WindGenTurbineType2IEC](WindGenTurbineType2IEC.md) | WindMechIEC | range | [WindMechIEC](WindMechIEC.md) |
| [WindTurbineType1or2IEC](WindTurbineType1or2IEC.md) | WindMechIEC | range | [WindMechIEC](WindMechIEC.md) |
| [WindTurbineType3IEC](WindTurbineType3IEC.md) | WindMechIEC | range | [WindMechIEC](WindMechIEC.md) |
| [WindTurbineType4bIEC](WindTurbineType4bIEC.md) | WindMechIEC | range | [WindMechIEC](WindMechIEC.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WindMechIEC |
| native | this:WindMechIEC |




