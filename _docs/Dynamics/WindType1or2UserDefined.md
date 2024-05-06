# WindType1or2UserDefined


_Wind type 1 or type 2 function block whose dynamic behaviour is described by <font color="#0f0f0f">a user-defined model.</font>_





**URI**: [cim:WindType1or2UserDefined](http://iec.ch/TC57/CIM100#WindType1or2UserDefined)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindType1or2UserDefined
    click WindType1or2UserDefined href "../WindType1or2UserDefined"
      WindTurbineType1or2Dynamics <|-- WindType1or2UserDefined
        click WindTurbineType1or2Dynamics href "../WindTurbineType1or2Dynamics"
      
      WindType1or2UserDefined : WindTurbineType1or2Dynamics.AsynchronousMachineDynamics
        
          WindType1or2UserDefined --> AsynchronousMachineDynamics : WindTurbineType1or2Dynamics.AsynchronousMachineDynamics
          click AsynchronousMachineDynamics href "../AsynchronousMachineDynamics"
        
      WindType1or2UserDefined : IdentifiedObject.description
        
      WindType1or2UserDefined : DynamicsFunctionBlock.enabled
        
      WindType1or2UserDefined : IdentifiedObject.mRID
        
      WindType1or2UserDefined : IdentifiedObject.name
        
      WindType1or2UserDefined : WindType1or2UserDefined.proprietary
        
      WindType1or2UserDefined : WindType1or2UserDefined.ProprietaryParameterDynamics
        
          WindType1or2UserDefined --> ProprietaryParameterDynamics : WindType1or2UserDefined.ProprietaryParameterDynamics
          click ProprietaryParameterDynamics href "../ProprietaryParameterDynamics"
        
      WindType1or2UserDefined : WindTurbineType1or2Dynamics.RemoteInputSignal
        
          WindType1or2UserDefined --> RemoteInputSignal : WindTurbineType1or2Dynamics.RemoteInputSignal
          click RemoteInputSignal href "../RemoteInputSignal"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [WindTurbineType1or2Dynamics](WindTurbineType1or2Dynamics.md)
            * **WindType1or2UserDefined**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| proprietary | [cim:WindType1or2UserDefined.proprietary](http://iec.ch/TC57/CIM100#WindType1or2UserDefined.proprietary) | 1 <br />  boolean  | Behaviour is based on a proprietary model as opposed to a detailed model | direct |
| ProprietaryParameterDynamics | [cim:WindType1or2UserDefined.ProprietaryParameterDynamics](http://iec.ch/TC57/CIM100#WindType1or2UserDefined.ProprietaryParameterDynamics) | * <br />  [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md)  | Parameter of this proprietary user-defined model | direct |
| RemoteInputSignal | [cim:WindTurbineType1or2Dynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#WindTurbineType1or2Dynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this wind generator type 1 or type 2 model | [WindTurbineType1or2Dynamics](WindTurbineType1or2Dynamics.md) |
| AsynchronousMachineDynamics | [cim:WindTurbineType1or2Dynamics.AsynchronousMachineDynamics](http://iec.ch/TC57/CIM100#WindTurbineType1or2Dynamics.AsynchronousMachineDynamics) | 1 <br />  [AsynchronousMachineDynamics](AsynchronousMachineDynamics.md)  | Asynchronous machine model with which this wind generator type 1 or type 2 mo... | [WindTurbineType1or2Dynamics](WindTurbineType1or2Dynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md) | WindType1or2UserDefined | range | [WindType1or2UserDefined](WindType1or2UserDefined.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WindType1or2UserDefined |
| native | this:WindType1or2UserDefined |




