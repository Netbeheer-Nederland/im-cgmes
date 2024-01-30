# WindGenType3aIEC


_IEC type 3A generator set model._

_Reference: IEC 61400-27-1:2015, 5.6.3.2._





**URI**: [cim:WindGenType3aIEC](http://iec.ch/TC57/CIM100#WindGenType3aIEC)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindGenType3aIEC
      WindGenType3IEC <|-- WindGenType3aIEC
      
      WindGenType3aIEC : IdentifiedObject.description
        
      WindGenType3aIEC : WindGenType3IEC.dipmax
        
          WindGenType3aIEC --> PU : WindGenType3IEC.dipmax
        
      WindGenType3aIEC : WindGenType3IEC.diqmax
        
          WindGenType3aIEC --> PU : WindGenType3IEC.diqmax
        
      WindGenType3aIEC : WindGenType3aIEC.kpc
        
      WindGenType3aIEC : IdentifiedObject.mRID
        
      WindGenType3aIEC : IdentifiedObject.name
        
      WindGenType3aIEC : WindGenType3aIEC.tic
        
          WindGenType3aIEC --> Seconds : WindGenType3aIEC.tic
        
      WindGenType3aIEC : WindGenType3IEC.WindTurbineType3IEC
        
          WindGenType3aIEC --> WindTurbineType3IEC : WindGenType3IEC.WindTurbineType3IEC
        
      WindGenType3aIEC : WindGenType3aIEC.WindTurbineType4IEC
        
          WindGenType3aIEC --> WindTurbineType4IEC : WindGenType3aIEC.WindTurbineType4IEC
        
      WindGenType3aIEC : WindGenType3IEC.xs
        
          WindGenType3aIEC --> PU : WindGenType3IEC.xs
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [WindGenType3IEC](WindGenType3IEC.md)
        * **WindGenType3aIEC**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| kpc | [cim:WindGenType3aIEC.kpc](http://iec.ch/TC57/CIM100#WindGenType3aIEC.kpc) | 1..1 <br />  float  | Current PI controller proportional gain (<i>K</i><i><sub>Pc</sub></i>) | direct |
| tic | [cim:WindGenType3aIEC.tic](http://iec.ch/TC57/CIM100#WindGenType3aIEC.tic) | 1..1 <br />  [Seconds](Seconds.md)  | Current PI controller integration time constant (<i>T</i><i><sub>Ic</sub></i>... | direct |
| WindTurbineType4IEC | [cim:WindGenType3aIEC.WindTurbineType4IEC](http://iec.ch/TC57/CIM100#WindGenType3aIEC.WindTurbineType4IEC) | 0..1 <br />  [WindTurbineType4IEC](WindTurbineType4IEC.md)  | Wind turbine type 4 model with which this wind generator type 3A model is ass... | direct |
| dipmax | [cim:WindGenType3IEC.dipmax](http://iec.ch/TC57/CIM100#WindGenType3IEC.dipmax) | 1..1 <br />  [PU](PU.md)  | Maximum active current ramp rate (<i>di</i><i><sub>pmax</sub></i>) | [WindGenType3IEC](WindGenType3IEC.md) |
| diqmax | [cim:WindGenType3IEC.diqmax](http://iec.ch/TC57/CIM100#WindGenType3IEC.diqmax) | 1..1 <br />  [PU](PU.md)  | Maximum reactive current ramp rate (<i>di</i><i><sub>qmax</sub></i>) | [WindGenType3IEC](WindGenType3IEC.md) |
| xs | [cim:WindGenType3IEC.xs](http://iec.ch/TC57/CIM100#WindGenType3IEC.xs) | 1..1 <br />  [PU](PU.md)  | Electromagnetic transient reactance (<i>x</i><i><sub>S</sub></i>) | [WindGenType3IEC](WindGenType3IEC.md) |
| WindTurbineType3IEC | [cim:WindGenType3IEC.WindTurbineType3IEC](http://iec.ch/TC57/CIM100#WindGenType3IEC.WindTurbineType3IEC) | 0..1 <br />  [WindTurbineType3IEC](WindTurbineType3IEC.md)  | Wind turbine type 3 model with which this wind generator type 3 is associated | [WindGenType3IEC](WindGenType3IEC.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [WindTurbineType4aIEC](WindTurbineType4aIEC.md) | WindGenType3aIEC | range | [WindGenType3aIEC](WindGenType3aIEC.md) |
| [WindTurbineType4bIEC](WindTurbineType4bIEC.md) | WindGenType3aIEC | range | [WindGenType3aIEC](WindGenType3aIEC.md) |
| [WindTurbineType4IEC](WindTurbineType4IEC.md) | WindGenType3aIEC | range | [WindGenType3aIEC](WindGenType3aIEC.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WindGenType3aIEC |
| native | this:WindGenType3aIEC |




