# UnderexcitationLimiterUserDefined


_Underexcitation limiter function block whose dynamic behaviour is described by <font color="#0f0f0f">a user-defined model.</font>_





**URI**: [cim:UnderexcitationLimiterUserDefined](http://iec.ch/TC57/CIM100#UnderexcitationLimiterUserDefined)<br />
**Type**: Class




```mermaid
 classDiagram
    class UnderexcitationLimiterUserDefined
      UnderexcitationLimiterDynamics <|-- UnderexcitationLimiterUserDefined
      
      UnderexcitationLimiterUserDefined : IdentifiedObject.description
        
      UnderexcitationLimiterUserDefined : DynamicsFunctionBlock.enabled
        
      UnderexcitationLimiterUserDefined : UnderexcitationLimiterDynamics.ExcitationSystemDynamics
        
          UnderexcitationLimiterUserDefined --> ExcitationSystemDynamics : UnderexcitationLimiterDynamics.ExcitationSystemDynamics
        
      UnderexcitationLimiterUserDefined : IdentifiedObject.mRID
        
      UnderexcitationLimiterUserDefined : IdentifiedObject.name
        
      UnderexcitationLimiterUserDefined : UnderexcitationLimiterUserDefined.proprietary
        
      UnderexcitationLimiterUserDefined : UnderexcitationLimiterUserDefined.ProprietaryParameterDynamics
        
          UnderexcitationLimiterUserDefined --> ProprietaryParameterDynamics : UnderexcitationLimiterUserDefined.ProprietaryParameterDynamics
        
      UnderexcitationLimiterUserDefined : UnderexcitationLimiterDynamics.RemoteInputSignal
        
          UnderexcitationLimiterUserDefined --> RemoteInputSignal : UnderexcitationLimiterDynamics.RemoteInputSignal
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md)
            * **UnderexcitationLimiterUserDefined**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| proprietary | [cim:UnderexcitationLimiterUserDefined.proprietary](http://iec.ch/TC57/CIM100#UnderexcitationLimiterUserDefined.proprietary) | 1..1 <br />  boolean  | Behaviour is based on a proprietary model as opposed to a detailed model | direct |
| ProprietaryParameterDynamics | [cim:UnderexcitationLimiterUserDefined.ProprietaryParameterDynamics](http://iec.ch/TC57/CIM100#UnderexcitationLimiterUserDefined.ProprietaryParameterDynamics) | 0..* <br />  [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md)  | Parameter of this proprietary user-defined model | direct |
| RemoteInputSignal | [cim:UnderexcitationLimiterDynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#UnderexcitationLimiterDynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this underexcitation limiter model | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| ExcitationSystemDynamics | [cim:UnderexcitationLimiterDynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#UnderexcitationLimiterDynamics.ExcitationSystemDynamics) | 1..1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this underexcitation limiter model is asso... | [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1..1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md) | UnderexcitationLimiterUserDefined | range | [UnderexcitationLimiterUserDefined](UnderexcitationLimiterUserDefined.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:UnderexcitationLimiterUserDefined |
| native | this:UnderexcitationLimiterUserDefined |




