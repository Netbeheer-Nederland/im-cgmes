# VoltageAdjusterDynamics


_Voltage adjuster function block whose behaviour is described by reference to a standard model <font color="#0f0f0f">or by definition of a user-defined model.</font>_





**URI**: [cim:VoltageAdjusterDynamics](http://iec.ch/TC57/CIM100#VoltageAdjusterDynamics)<br />
**Type**: Class




```mermaid
 classDiagram
    class VoltageAdjusterDynamics
      DynamicsFunctionBlock <|-- VoltageAdjusterDynamics
      

      VoltageAdjusterDynamics <|-- VoltageAdjusterUserDefined
      VoltageAdjusterDynamics <|-- VAdjIEEE
      
      
      VoltageAdjusterDynamics : IdentifiedObject.description
        
      VoltageAdjusterDynamics : DynamicsFunctionBlock.enabled
        
      VoltageAdjusterDynamics : IdentifiedObject.mRID
        
      VoltageAdjusterDynamics : IdentifiedObject.name
        
      VoltageAdjusterDynamics : VoltageAdjusterDynamics.PFVArControllerType1Dynamics
        
          VoltageAdjusterDynamics --> PFVArControllerType1Dynamics : VoltageAdjusterDynamics.PFVArControllerType1Dynamics
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * **VoltageAdjusterDynamics**
            * [VoltageAdjusterUserDefined](VoltageAdjusterUserDefined.md)
            * [VAdjIEEE](VAdjIEEE.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| PFVArControllerType1Dynamics | [cim:VoltageAdjusterDynamics.PFVArControllerType1Dynamics](http://iec.ch/TC57/CIM100#VoltageAdjusterDynamics.PFVArControllerType1Dynamics) | 1..1 <br />  [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md)  | Power factor or VAr controller type 1 model with which this voltage adjuster ... | direct |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1..1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [PFVArControllerType1UserDefined](PFVArControllerType1UserDefined.md) | VoltageAdjusterDynamics | range | [VoltageAdjusterDynamics](VoltageAdjusterDynamics.md) |
| [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) | VoltageAdjusterDynamics | range | [VoltageAdjusterDynamics](VoltageAdjusterDynamics.md) |
| [PFVArType1IEEEPFController](PFVArType1IEEEPFController.md) | VoltageAdjusterDynamics | range | [VoltageAdjusterDynamics](VoltageAdjusterDynamics.md) |
| [PFVArType1IEEEVArController](PFVArType1IEEEVArController.md) | VoltageAdjusterDynamics | range | [VoltageAdjusterDynamics](VoltageAdjusterDynamics.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:VoltageAdjusterDynamics |
| native | this:VoltageAdjusterDynamics |




