# HVDCDynamics


_HVDC whose behaviour is described by reference to a standard model <font color="#0f0f0f">or by definition of a user-defined model.</font>_





**URI**: [cim:HVDCDynamics](http://iec.ch/TC57/CIM100#HVDCDynamics)<br />
**Type**: Class




```mermaid
 classDiagram
    class HVDCDynamics
      DynamicsFunctionBlock <|-- HVDCDynamics
      

      HVDCDynamics <|-- CSCDynamics
      HVDCDynamics <|-- VSCDynamics
      
      
      HVDCDynamics : IdentifiedObject.description
        
      HVDCDynamics : DynamicsFunctionBlock.enabled
        
      HVDCDynamics : IdentifiedObject.mRID
        
      HVDCDynamics : IdentifiedObject.name
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * **HVDCDynamics**
            * [CSCDynamics](CSCDynamics.md)
            * [VSCDynamics](VSCDynamics.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1..1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:HVDCDynamics |
| native | this:HVDCDynamics |




