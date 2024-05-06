# TurbineLoadControllerUserDefined


_Turbine load controller function block whose dynamic behaviour is described by <font color="#0f0f0f">a user-defined model.</font>_





**URI**: [cim:TurbineLoadControllerUserDefined](http://iec.ch/TC57/CIM100#TurbineLoadControllerUserDefined)<br />
**Type**: Class




```mermaid
 classDiagram
    class TurbineLoadControllerUserDefined
    click TurbineLoadControllerUserDefined href "../TurbineLoadControllerUserDefined"
      TurbineLoadControllerDynamics <|-- TurbineLoadControllerUserDefined
        click TurbineLoadControllerDynamics href "../TurbineLoadControllerDynamics"
      
      TurbineLoadControllerUserDefined : IdentifiedObject.description
        
      TurbineLoadControllerUserDefined : DynamicsFunctionBlock.enabled
        
      TurbineLoadControllerUserDefined : IdentifiedObject.mRID
        
      TurbineLoadControllerUserDefined : IdentifiedObject.name
        
      TurbineLoadControllerUserDefined : TurbineLoadControllerUserDefined.proprietary
        
      TurbineLoadControllerUserDefined : TurbineLoadControllerUserDefined.ProprietaryParameterDynamics
        
          TurbineLoadControllerUserDefined --> ProprietaryParameterDynamics : TurbineLoadControllerUserDefined.ProprietaryParameterDynamics
          click ProprietaryParameterDynamics href "../ProprietaryParameterDynamics"
        
      TurbineLoadControllerUserDefined : TurbineLoadControllerDynamics.TurbineGovernorDynamics
        
          TurbineLoadControllerUserDefined --> TurbineGovernorDynamics : TurbineLoadControllerDynamics.TurbineGovernorDynamics
          click TurbineGovernorDynamics href "../TurbineGovernorDynamics"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [TurbineLoadControllerDynamics](TurbineLoadControllerDynamics.md)
            * **TurbineLoadControllerUserDefined**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| proprietary | [cim:TurbineLoadControllerUserDefined.proprietary](http://iec.ch/TC57/CIM100#TurbineLoadControllerUserDefined.proprietary) | 1 <br />  boolean  | Behaviour is based on a proprietary model as opposed to a detailed model | direct |
| ProprietaryParameterDynamics | [cim:TurbineLoadControllerUserDefined.ProprietaryParameterDynamics](http://iec.ch/TC57/CIM100#TurbineLoadControllerUserDefined.ProprietaryParameterDynamics) | * <br />  [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md)  | Parameter of this proprietary user-defined model | direct |
| TurbineGovernorDynamics | [cim:TurbineLoadControllerDynamics.TurbineGovernorDynamics](http://iec.ch/TC57/CIM100#TurbineLoadControllerDynamics.TurbineGovernorDynamics) | 1 <br />  [TurbineGovernorDynamics](TurbineGovernorDynamics.md)  | Turbine-governor controlled by this turbine load controller | [TurbineLoadControllerDynamics](TurbineLoadControllerDynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md) | TurbineLoadControllerUserDefined | range | [TurbineLoadControllerUserDefined](TurbineLoadControllerUserDefined.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:TurbineLoadControllerUserDefined |
| native | this:TurbineLoadControllerUserDefined |




