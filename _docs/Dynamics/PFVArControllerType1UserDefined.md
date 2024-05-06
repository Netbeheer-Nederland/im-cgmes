# PFVArControllerType1UserDefined


_Power factor or VAr controller type 1 function block whose dynamic behaviour is described by <font color="#0f0f0f">a user-defined model.</font>_





**URI**: [cim:PFVArControllerType1UserDefined](http://iec.ch/TC57/CIM100#PFVArControllerType1UserDefined)<br />
**Type**: Class




```mermaid
 classDiagram
    class PFVArControllerType1UserDefined
    click PFVArControllerType1UserDefined href "../PFVArControllerType1UserDefined"
      PFVArControllerType1Dynamics <|-- PFVArControllerType1UserDefined
        click PFVArControllerType1Dynamics href "../PFVArControllerType1Dynamics"
      
      PFVArControllerType1UserDefined : IdentifiedObject.description
        
      PFVArControllerType1UserDefined : DynamicsFunctionBlock.enabled
        
      PFVArControllerType1UserDefined : PFVArControllerType1Dynamics.ExcitationSystemDynamics
        
          PFVArControllerType1UserDefined --> ExcitationSystemDynamics : PFVArControllerType1Dynamics.ExcitationSystemDynamics
          click ExcitationSystemDynamics href "../ExcitationSystemDynamics"
        
      PFVArControllerType1UserDefined : IdentifiedObject.mRID
        
      PFVArControllerType1UserDefined : IdentifiedObject.name
        
      PFVArControllerType1UserDefined : PFVArControllerType1UserDefined.proprietary
        
      PFVArControllerType1UserDefined : PFVArControllerType1UserDefined.ProprietaryParameterDynamics
        
          PFVArControllerType1UserDefined --> ProprietaryParameterDynamics : PFVArControllerType1UserDefined.ProprietaryParameterDynamics
          click ProprietaryParameterDynamics href "../ProprietaryParameterDynamics"
        
      PFVArControllerType1UserDefined : PFVArControllerType1Dynamics.RemoteInputSignal
        
          PFVArControllerType1UserDefined --> RemoteInputSignal : PFVArControllerType1Dynamics.RemoteInputSignal
          click RemoteInputSignal href "../RemoteInputSignal"
        
      PFVArControllerType1UserDefined : PFVArControllerType1Dynamics.VoltageAdjusterDynamics
        
          PFVArControllerType1UserDefined --> VoltageAdjusterDynamics : PFVArControllerType1Dynamics.VoltageAdjusterDynamics
          click VoltageAdjusterDynamics href "../VoltageAdjusterDynamics"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md)
            * **PFVArControllerType1UserDefined**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| proprietary | [cim:PFVArControllerType1UserDefined.proprietary](http://iec.ch/TC57/CIM100#PFVArControllerType1UserDefined.proprietary) | 1 <br />  boolean  | Behaviour is based on a proprietary model as opposed to a detailed model | direct |
| ProprietaryParameterDynamics | [cim:PFVArControllerType1UserDefined.ProprietaryParameterDynamics](http://iec.ch/TC57/CIM100#PFVArControllerType1UserDefined.ProprietaryParameterDynamics) | * <br />  [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md)  | Parameter of this proprietary user-defined model | direct |
| RemoteInputSignal | [cim:PFVArControllerType1Dynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#PFVArControllerType1Dynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this power factor or VAr controller type 1 model | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| ExcitationSystemDynamics | [cim:PFVArControllerType1Dynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#PFVArControllerType1Dynamics.ExcitationSystemDynamics) | 1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this power actor or VAr controller type 1 ... | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| VoltageAdjusterDynamics | [cim:PFVArControllerType1Dynamics.VoltageAdjusterDynamics](http://iec.ch/TC57/CIM100#PFVArControllerType1Dynamics.VoltageAdjusterDynamics) | 0..1 <br />  [VoltageAdjusterDynamics](VoltageAdjusterDynamics.md)  | Voltage adjuster model associated with this power factor or VAr controller ty... | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md) | PFVArControllerType1UserDefined | range | [PFVArControllerType1UserDefined](PFVArControllerType1UserDefined.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:PFVArControllerType1UserDefined |
| native | this:PFVArControllerType1UserDefined |




