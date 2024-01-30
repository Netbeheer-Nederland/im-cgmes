# TurbineGovernorUserDefined


_Turbine-governor function block whose dynamic behaviour is described by <font color="#0f0f0f">a user-defined model.</font>_





**URI**: [cim:TurbineGovernorUserDefined](http://iec.ch/TC57/CIM100#TurbineGovernorUserDefined)<br />
**Type**: Class




```mermaid
 classDiagram
    class TurbineGovernorUserDefined
      TurbineGovernorDynamics <|-- TurbineGovernorUserDefined
      
      TurbineGovernorUserDefined : TurbineGovernorDynamics.AsynchronousMachineDynamics
        
          TurbineGovernorUserDefined --> AsynchronousMachineDynamics : TurbineGovernorDynamics.AsynchronousMachineDynamics
        
      TurbineGovernorUserDefined : IdentifiedObject.description
        
      TurbineGovernorUserDefined : DynamicsFunctionBlock.enabled
        
      TurbineGovernorUserDefined : IdentifiedObject.mRID
        
      TurbineGovernorUserDefined : IdentifiedObject.name
        
      TurbineGovernorUserDefined : TurbineGovernorUserDefined.proprietary
        
      TurbineGovernorUserDefined : TurbineGovernorUserDefined.ProprietaryParameterDynamics
        
          TurbineGovernorUserDefined --> ProprietaryParameterDynamics : TurbineGovernorUserDefined.ProprietaryParameterDynamics
        
      TurbineGovernorUserDefined : TurbineGovernorDynamics.SynchronousMachineDynamics
        
          TurbineGovernorUserDefined --> SynchronousMachineDynamics : TurbineGovernorDynamics.SynchronousMachineDynamics
        
      TurbineGovernorUserDefined : TurbineGovernorDynamics.TurbineLoadControllerDynamics
        
          TurbineGovernorUserDefined --> TurbineLoadControllerDynamics : TurbineGovernorDynamics.TurbineLoadControllerDynamics
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [TurbineGovernorDynamics](TurbineGovernorDynamics.md)
            * **TurbineGovernorUserDefined**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| proprietary | [cim:TurbineGovernorUserDefined.proprietary](http://iec.ch/TC57/CIM100#TurbineGovernorUserDefined.proprietary) | 1..1 <br />  boolean  | Behaviour is based on a proprietary model as opposed to a detailed model | direct |
| ProprietaryParameterDynamics | [cim:TurbineGovernorUserDefined.ProprietaryParameterDynamics](http://iec.ch/TC57/CIM100#TurbineGovernorUserDefined.ProprietaryParameterDynamics) | 0..* <br />  [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md)  | Parameter of this proprietary user-defined model | direct |
| SynchronousMachineDynamics | [cim:TurbineGovernorDynamics.SynchronousMachineDynamics](http://iec.ch/TC57/CIM100#TurbineGovernorDynamics.SynchronousMachineDynamics) | 0..1 <br />  [SynchronousMachineDynamics](SynchronousMachineDynamics.md)  | Synchronous machine model with which this turbine-governor model is associate... | [TurbineGovernorDynamics](TurbineGovernorDynamics.md) |
| AsynchronousMachineDynamics | [cim:TurbineGovernorDynamics.AsynchronousMachineDynamics](http://iec.ch/TC57/CIM100#TurbineGovernorDynamics.AsynchronousMachineDynamics) | 0..1 <br />  [AsynchronousMachineDynamics](AsynchronousMachineDynamics.md)  | Asynchronous machine model with which this turbine-governor model is associat... | [TurbineGovernorDynamics](TurbineGovernorDynamics.md) |
| TurbineLoadControllerDynamics | [cim:TurbineGovernorDynamics.TurbineLoadControllerDynamics](http://iec.ch/TC57/CIM100#TurbineGovernorDynamics.TurbineLoadControllerDynamics) | 0..1 <br />  [TurbineLoadControllerDynamics](TurbineLoadControllerDynamics.md)  | Turbine load controller providing input to this turbine-governor | [TurbineGovernorDynamics](TurbineGovernorDynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1..1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md) | TurbineGovernorUserDefined | range | [TurbineGovernorUserDefined](TurbineGovernorUserDefined.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:TurbineGovernorUserDefined |
| native | this:TurbineGovernorUserDefined |




