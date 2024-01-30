# DiscontinuousExcitationControlUserDefined


_Discontinuous excitation control function block whose dynamic behaviour is described by <font color="#0f0f0f">a user-defined model.</font>_





**URI**: [cim:DiscontinuousExcitationControlUserDefined](http://iec.ch/TC57/CIM100#DiscontinuousExcitationControlUserDefined)<br />
**Type**: Class




```mermaid
 classDiagram
    class DiscontinuousExcitationControlUserDefined
      DiscontinuousExcitationControlDynamics <|-- DiscontinuousExcitationControlUserDefined
      
      DiscontinuousExcitationControlUserDefined : IdentifiedObject.description
        
      DiscontinuousExcitationControlUserDefined : DynamicsFunctionBlock.enabled
        
      DiscontinuousExcitationControlUserDefined : DiscontinuousExcitationControlDynamics.ExcitationSystemDynamics
        
          DiscontinuousExcitationControlUserDefined --> ExcitationSystemDynamics : DiscontinuousExcitationControlDynamics.ExcitationSystemDynamics
        
      DiscontinuousExcitationControlUserDefined : IdentifiedObject.mRID
        
      DiscontinuousExcitationControlUserDefined : IdentifiedObject.name
        
      DiscontinuousExcitationControlUserDefined : DiscontinuousExcitationControlUserDefined.proprietary
        
      DiscontinuousExcitationControlUserDefined : DiscontinuousExcitationControlUserDefined.ProprietaryParameterDynamics
        
          DiscontinuousExcitationControlUserDefined --> ProprietaryParameterDynamics : DiscontinuousExcitationControlUserDefined.ProprietaryParameterDynamics
        
      DiscontinuousExcitationControlUserDefined : DiscontinuousExcitationControlDynamics.RemoteInputSignal
        
          DiscontinuousExcitationControlUserDefined --> RemoteInputSignal : DiscontinuousExcitationControlDynamics.RemoteInputSignal
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md)
            * **DiscontinuousExcitationControlUserDefined**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| proprietary | [cim:DiscontinuousExcitationControlUserDefined.proprietary](http://iec.ch/TC57/CIM100#DiscontinuousExcitationControlUserDefined.proprietary) | 1..1 <br />  boolean  | Behaviour is based on a proprietary model as opposed to a detailed model | direct |
| ProprietaryParameterDynamics | [cim:DiscontinuousExcitationControlUserDefined.ProprietaryParameterDynamics](http://iec.ch/TC57/CIM100#DiscontinuousExcitationControlUserDefined.ProprietaryParameterDynamics) | 0..* <br />  [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md)  | Parameter of this proprietary user-defined model | direct |
| RemoteInputSignal | [cim:DiscontinuousExcitationControlDynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#DiscontinuousExcitationControlDynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this discontinuous excitation control system mode... | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| ExcitationSystemDynamics | [cim:DiscontinuousExcitationControlDynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#DiscontinuousExcitationControlDynamics.ExcitationSystemDynamics) | 1..1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this discontinuous excitation control mode... | [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1..1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md) | DiscontinuousExcitationControlUserDefined | range | [DiscontinuousExcitationControlUserDefined](DiscontinuousExcitationControlUserDefined.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:DiscontinuousExcitationControlUserDefined |
| native | this:DiscontinuousExcitationControlUserDefined |




