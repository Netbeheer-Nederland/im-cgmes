# OverexcitationLimiterUserDefined


_Overexcitation limiter system function block whose dynamic behaviour is described by <font color="#0f0f0f">a user-defined model.</font>_





**URI**: [cim:OverexcitationLimiterUserDefined](http://iec.ch/TC57/CIM100#OverexcitationLimiterUserDefined)<br />
**Type**: Class




```mermaid
 classDiagram
    class OverexcitationLimiterUserDefined
    click OverexcitationLimiterUserDefined href "../OverexcitationLimiterUserDefined"
      OverexcitationLimiterDynamics <|-- OverexcitationLimiterUserDefined
        click OverexcitationLimiterDynamics href "../OverexcitationLimiterDynamics"
      
      OverexcitationLimiterUserDefined : IdentifiedObject.description
        
      OverexcitationLimiterUserDefined : DynamicsFunctionBlock.enabled
        
      OverexcitationLimiterUserDefined : OverexcitationLimiterDynamics.ExcitationSystemDynamics
        
          OverexcitationLimiterUserDefined --> ExcitationSystemDynamics : OverexcitationLimiterDynamics.ExcitationSystemDynamics
          click ExcitationSystemDynamics href "../ExcitationSystemDynamics"
        
      OverexcitationLimiterUserDefined : IdentifiedObject.mRID
        
      OverexcitationLimiterUserDefined : IdentifiedObject.name
        
      OverexcitationLimiterUserDefined : OverexcitationLimiterUserDefined.proprietary
        
      OverexcitationLimiterUserDefined : OverexcitationLimiterUserDefined.ProprietaryParameterDynamics
        
          OverexcitationLimiterUserDefined --> ProprietaryParameterDynamics : OverexcitationLimiterUserDefined.ProprietaryParameterDynamics
          click ProprietaryParameterDynamics href "../ProprietaryParameterDynamics"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md)
            * **OverexcitationLimiterUserDefined**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| proprietary | [cim:OverexcitationLimiterUserDefined.proprietary](http://iec.ch/TC57/CIM100#OverexcitationLimiterUserDefined.proprietary) | 1 <br />  boolean  | Behaviour is based on a proprietary model as opposed to a detailed model | direct |
| ProprietaryParameterDynamics | [cim:OverexcitationLimiterUserDefined.ProprietaryParameterDynamics](http://iec.ch/TC57/CIM100#OverexcitationLimiterUserDefined.ProprietaryParameterDynamics) | * <br />  [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md)  | Parameter of this proprietary user-defined model | direct |
| ExcitationSystemDynamics | [cim:OverexcitationLimiterDynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#OverexcitationLimiterDynamics.ExcitationSystemDynamics) | 1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this overexcitation limiter model is assoc... | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md) | OverexcitationLimiterUserDefined | range | [OverexcitationLimiterUserDefined](OverexcitationLimiterUserDefined.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:OverexcitationLimiterUserDefined |
| native | this:OverexcitationLimiterUserDefined |




