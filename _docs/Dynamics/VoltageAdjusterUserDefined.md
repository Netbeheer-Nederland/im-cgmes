# VoltageAdjusterUserDefined


_<font color="#0f0f0f">Voltage adjuster</font> function block whose dynamic behaviour is described by <font color="#0f0f0f">a user-defined model.</font>_





**URI**: [cim:VoltageAdjusterUserDefined](http://iec.ch/TC57/CIM100#VoltageAdjusterUserDefined)<br />
**Type**: Class




```mermaid
 classDiagram
    class VoltageAdjusterUserDefined
    click VoltageAdjusterUserDefined href "../VoltageAdjusterUserDefined"
      VoltageAdjusterDynamics <|-- VoltageAdjusterUserDefined
        click VoltageAdjusterDynamics href "../VoltageAdjusterDynamics"
      
      VoltageAdjusterUserDefined : IdentifiedObject.description
        
      VoltageAdjusterUserDefined : DynamicsFunctionBlock.enabled
        
      VoltageAdjusterUserDefined : IdentifiedObject.mRID
        
      VoltageAdjusterUserDefined : IdentifiedObject.name
        
      VoltageAdjusterUserDefined : VoltageAdjusterDynamics.PFVArControllerType1Dynamics
        
          VoltageAdjusterUserDefined --> PFVArControllerType1Dynamics : VoltageAdjusterDynamics.PFVArControllerType1Dynamics
          click PFVArControllerType1Dynamics href "../PFVArControllerType1Dynamics"
        
      VoltageAdjusterUserDefined : VoltageAdjusterUserDefined.proprietary
        
      VoltageAdjusterUserDefined : VoltageAdjusterUserDefined.ProprietaryParameterDynamics
        
          VoltageAdjusterUserDefined --> ProprietaryParameterDynamics : VoltageAdjusterUserDefined.ProprietaryParameterDynamics
          click ProprietaryParameterDynamics href "../ProprietaryParameterDynamics"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [VoltageAdjusterDynamics](VoltageAdjusterDynamics.md)
            * **VoltageAdjusterUserDefined**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| proprietary | [cim:VoltageAdjusterUserDefined.proprietary](http://iec.ch/TC57/CIM100#VoltageAdjusterUserDefined.proprietary) | 1 <br />  boolean  | Behaviour is based on a proprietary model as opposed to a detailed model | direct |
| ProprietaryParameterDynamics | [cim:VoltageAdjusterUserDefined.ProprietaryParameterDynamics](http://iec.ch/TC57/CIM100#VoltageAdjusterUserDefined.ProprietaryParameterDynamics) | * <br />  [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md)  | Parameter of this proprietary user-defined model | direct |
| PFVArControllerType1Dynamics | [cim:VoltageAdjusterDynamics.PFVArControllerType1Dynamics](http://iec.ch/TC57/CIM100#VoltageAdjusterDynamics.PFVArControllerType1Dynamics) | 1 <br />  [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md)  | Power factor or VAr controller type 1 model with which this voltage adjuster ... | [VoltageAdjusterDynamics](VoltageAdjusterDynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md) | VoltageAdjusterUserDefined | range | [VoltageAdjusterUserDefined](VoltageAdjusterUserDefined.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:VoltageAdjusterUserDefined |
| native | this:VoltageAdjusterUserDefined |




