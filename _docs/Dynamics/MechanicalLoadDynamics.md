# MechanicalLoadDynamics


_Mechanical load function block whose behaviour is described by reference to a standard model <font color="#0f0f0f">or by definition of a user-defined model.</font>_





**URI**: [cim:MechanicalLoadDynamics](http://iec.ch/TC57/CIM100#MechanicalLoadDynamics)<br />
**Type**: Class




```mermaid
 classDiagram
    class MechanicalLoadDynamics
      DynamicsFunctionBlock <|-- MechanicalLoadDynamics
      

      MechanicalLoadDynamics <|-- MechanicalLoadUserDefined
      MechanicalLoadDynamics <|-- MechLoad1
      
      
      MechanicalLoadDynamics : MechanicalLoadDynamics.AsynchronousMachineDynamics
        
          MechanicalLoadDynamics --> AsynchronousMachineDynamics : MechanicalLoadDynamics.AsynchronousMachineDynamics
        
      MechanicalLoadDynamics : IdentifiedObject.description
        
      MechanicalLoadDynamics : DynamicsFunctionBlock.enabled
        
      MechanicalLoadDynamics : IdentifiedObject.mRID
        
      MechanicalLoadDynamics : IdentifiedObject.name
        
      MechanicalLoadDynamics : MechanicalLoadDynamics.SynchronousMachineDynamics
        
          MechanicalLoadDynamics --> SynchronousMachineDynamics : MechanicalLoadDynamics.SynchronousMachineDynamics
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * **MechanicalLoadDynamics**
            * [MechanicalLoadUserDefined](MechanicalLoadUserDefined.md)
            * [MechLoad1](MechLoad1.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| SynchronousMachineDynamics | [cim:MechanicalLoadDynamics.SynchronousMachineDynamics](http://iec.ch/TC57/CIM100#MechanicalLoadDynamics.SynchronousMachineDynamics) | 0..1 <br />  [SynchronousMachineDynamics](SynchronousMachineDynamics.md)  | Synchronous machine model with which this mechanical load model is associated | direct |
| AsynchronousMachineDynamics | [cim:MechanicalLoadDynamics.AsynchronousMachineDynamics](http://iec.ch/TC57/CIM100#MechanicalLoadDynamics.AsynchronousMachineDynamics) | 0..1 <br />  [AsynchronousMachineDynamics](AsynchronousMachineDynamics.md)  | Asynchronous machine model with which this mechanical load model is associate... | direct |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1..1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [SynchronousMachineUserDefined](SynchronousMachineUserDefined.md) | MechanicalLoadDynamics | range | [MechanicalLoadDynamics](MechanicalLoadDynamics.md) |
| [AsynchronousMachineUserDefined](AsynchronousMachineUserDefined.md) | MechanicalLoadDynamics | range | [MechanicalLoadDynamics](MechanicalLoadDynamics.md) |
| [SynchronousMachineSimplified](SynchronousMachineSimplified.md) | MechanicalLoadDynamics | range | [MechanicalLoadDynamics](MechanicalLoadDynamics.md) |
| [SynchronousMachineDynamics](SynchronousMachineDynamics.md) | MechanicalLoadDynamics | range | [MechanicalLoadDynamics](MechanicalLoadDynamics.md) |
| [SynchronousMachineDetailed](SynchronousMachineDetailed.md) | MechanicalLoadDynamics | range | [MechanicalLoadDynamics](MechanicalLoadDynamics.md) |
| [SynchronousMachineTimeConstantReactance](SynchronousMachineTimeConstantReactance.md) | MechanicalLoadDynamics | range | [MechanicalLoadDynamics](MechanicalLoadDynamics.md) |
| [SynchronousMachineEquivalentCircuit](SynchronousMachineEquivalentCircuit.md) | MechanicalLoadDynamics | range | [MechanicalLoadDynamics](MechanicalLoadDynamics.md) |
| [AsynchronousMachineDynamics](AsynchronousMachineDynamics.md) | MechanicalLoadDynamics | range | [MechanicalLoadDynamics](MechanicalLoadDynamics.md) |
| [AsynchronousMachineTimeConstantReactance](AsynchronousMachineTimeConstantReactance.md) | MechanicalLoadDynamics | range | [MechanicalLoadDynamics](MechanicalLoadDynamics.md) |
| [AsynchronousMachineEquivalentCircuit](AsynchronousMachineEquivalentCircuit.md) | MechanicalLoadDynamics | range | [MechanicalLoadDynamics](MechanicalLoadDynamics.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:MechanicalLoadDynamics |
| native | this:MechanicalLoadDynamics |




