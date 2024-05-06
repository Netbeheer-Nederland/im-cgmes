# WindTurbineType1or2Dynamics


_Parent class supporting relationships to wind turbines type 1 and type 2 and their control models.  Generator model for wind turbine of type 1 or type 2 is a standard asynchronous generator model._





**URI**: [cim:WindTurbineType1or2Dynamics](http://iec.ch/TC57/CIM100#WindTurbineType1or2Dynamics)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindTurbineType1or2Dynamics
    click WindTurbineType1or2Dynamics href "../WindTurbineType1or2Dynamics"
      DynamicsFunctionBlock <|-- WindTurbineType1or2Dynamics
        click DynamicsFunctionBlock href "../DynamicsFunctionBlock"
      

      WindTurbineType1or2Dynamics <|-- WindType1or2UserDefined
        click WindType1or2UserDefined href "../WindType1or2UserDefined"
      WindTurbineType1or2Dynamics <|-- WindTurbineType1or2IEC
        click WindTurbineType1or2IEC href "../WindTurbineType1or2IEC"
      
      
      WindTurbineType1or2Dynamics : WindTurbineType1or2Dynamics.AsynchronousMachineDynamics
        
          WindTurbineType1or2Dynamics --> AsynchronousMachineDynamics : WindTurbineType1or2Dynamics.AsynchronousMachineDynamics
          click AsynchronousMachineDynamics href "../AsynchronousMachineDynamics"
        
      WindTurbineType1or2Dynamics : IdentifiedObject.description
        
      WindTurbineType1or2Dynamics : DynamicsFunctionBlock.enabled
        
      WindTurbineType1or2Dynamics : IdentifiedObject.mRID
        
      WindTurbineType1or2Dynamics : IdentifiedObject.name
        
      WindTurbineType1or2Dynamics : WindTurbineType1or2Dynamics.RemoteInputSignal
        
          WindTurbineType1or2Dynamics --> RemoteInputSignal : WindTurbineType1or2Dynamics.RemoteInputSignal
          click RemoteInputSignal href "../RemoteInputSignal"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * **WindTurbineType1or2Dynamics**
            * [WindType1or2UserDefined](WindType1or2UserDefined.md)
            * [WindTurbineType1or2IEC](WindTurbineType1or2IEC.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| RemoteInputSignal | [cim:WindTurbineType1or2Dynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#WindTurbineType1or2Dynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this wind generator type 1 or type 2 model | direct |
| AsynchronousMachineDynamics | [cim:WindTurbineType1or2Dynamics.AsynchronousMachineDynamics](http://iec.ch/TC57/CIM100#WindTurbineType1or2Dynamics.AsynchronousMachineDynamics) | 1 <br />  [AsynchronousMachineDynamics](AsynchronousMachineDynamics.md)  | Asynchronous machine model with which this wind generator type 1 or type 2 mo... | direct |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [RemoteInputSignal](RemoteInputSignal.md) | WindTurbineType1or2Dynamics | range | [WindTurbineType1or2Dynamics](WindTurbineType1or2Dynamics.md) |
| [AsynchronousMachineUserDefined](AsynchronousMachineUserDefined.md) | WindTurbineType1or2Dynamics | range | [WindTurbineType1or2Dynamics](WindTurbineType1or2Dynamics.md) |
| [AsynchronousMachineDynamics](AsynchronousMachineDynamics.md) | WindTurbineType1or2Dynamics | range | [WindTurbineType1or2Dynamics](WindTurbineType1or2Dynamics.md) |
| [AsynchronousMachineTimeConstantReactance](AsynchronousMachineTimeConstantReactance.md) | WindTurbineType1or2Dynamics | range | [WindTurbineType1or2Dynamics](WindTurbineType1or2Dynamics.md) |
| [AsynchronousMachineEquivalentCircuit](AsynchronousMachineEquivalentCircuit.md) | WindTurbineType1or2Dynamics | range | [WindTurbineType1or2Dynamics](WindTurbineType1or2Dynamics.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WindTurbineType1or2Dynamics |
| native | this:WindTurbineType1or2Dynamics |




