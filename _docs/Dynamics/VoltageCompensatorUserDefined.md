# VoltageCompensatorUserDefined


_Voltage compensator function block whose dynamic behaviour is described by <font color="#0f0f0f">a user-defined model.</font>_





**URI**: [cim:VoltageCompensatorUserDefined](http://iec.ch/TC57/CIM100#VoltageCompensatorUserDefined)<br />
**Type**: Class




```mermaid
 classDiagram
    class VoltageCompensatorUserDefined
      VoltageCompensatorDynamics <|-- VoltageCompensatorUserDefined
      
      VoltageCompensatorUserDefined : IdentifiedObject.description
        
      VoltageCompensatorUserDefined : DynamicsFunctionBlock.enabled
        
      VoltageCompensatorUserDefined : VoltageCompensatorDynamics.ExcitationSystemDynamics
        
          VoltageCompensatorUserDefined --> ExcitationSystemDynamics : VoltageCompensatorDynamics.ExcitationSystemDynamics
        
      VoltageCompensatorUserDefined : IdentifiedObject.mRID
        
      VoltageCompensatorUserDefined : IdentifiedObject.name
        
      VoltageCompensatorUserDefined : VoltageCompensatorUserDefined.proprietary
        
      VoltageCompensatorUserDefined : VoltageCompensatorUserDefined.ProprietaryParameterDynamics
        
          VoltageCompensatorUserDefined --> ProprietaryParameterDynamics : VoltageCompensatorUserDefined.ProprietaryParameterDynamics
        
      VoltageCompensatorUserDefined : VoltageCompensatorDynamics.RemoteInputSignal
        
          VoltageCompensatorUserDefined --> RemoteInputSignal : VoltageCompensatorDynamics.RemoteInputSignal
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md)
            * **VoltageCompensatorUserDefined**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| proprietary | [cim:VoltageCompensatorUserDefined.proprietary](http://iec.ch/TC57/CIM100#VoltageCompensatorUserDefined.proprietary) | 1..1 <br />  boolean  | Behaviour is based on a proprietary model as opposed to a detailed model | direct |
| ProprietaryParameterDynamics | [cim:VoltageCompensatorUserDefined.ProprietaryParameterDynamics](http://iec.ch/TC57/CIM100#VoltageCompensatorUserDefined.ProprietaryParameterDynamics) | 0..* <br />  [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md)  | Parameter of this proprietary user-defined model | direct |
| RemoteInputSignal | [cim:VoltageCompensatorDynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#VoltageCompensatorDynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this voltage compensator model | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| ExcitationSystemDynamics | [cim:VoltageCompensatorDynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#VoltageCompensatorDynamics.ExcitationSystemDynamics) | 1..1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this voltage compensator is associated | [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1..1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md) | VoltageCompensatorUserDefined | range | [VoltageCompensatorUserDefined](VoltageCompensatorUserDefined.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:VoltageCompensatorUserDefined |
| native | this:VoltageCompensatorUserDefined |




