# PowerSystemStabilizerUserDefined


_<font color="#0f0f0f">Power system stabilizer</font> function block whose dynamic behaviour is described by <font color="#0f0f0f">a user-defined model.</font>_





**URI**: [cim:PowerSystemStabilizerUserDefined](http://iec.ch/TC57/CIM100#PowerSystemStabilizerUserDefined)<br />
**Type**: Class




```mermaid
 classDiagram
    class PowerSystemStabilizerUserDefined
      PowerSystemStabilizerDynamics <|-- PowerSystemStabilizerUserDefined
      
      PowerSystemStabilizerUserDefined : IdentifiedObject.description
        
      PowerSystemStabilizerUserDefined : DynamicsFunctionBlock.enabled
        
      PowerSystemStabilizerUserDefined : PowerSystemStabilizerDynamics.ExcitationSystemDynamics
        
          PowerSystemStabilizerUserDefined --> ExcitationSystemDynamics : PowerSystemStabilizerDynamics.ExcitationSystemDynamics
        
      PowerSystemStabilizerUserDefined : IdentifiedObject.mRID
        
      PowerSystemStabilizerUserDefined : IdentifiedObject.name
        
      PowerSystemStabilizerUserDefined : PowerSystemStabilizerUserDefined.proprietary
        
      PowerSystemStabilizerUserDefined : PowerSystemStabilizerUserDefined.ProprietaryParameterDynamics
        
          PowerSystemStabilizerUserDefined --> ProprietaryParameterDynamics : PowerSystemStabilizerUserDefined.ProprietaryParameterDynamics
        
      PowerSystemStabilizerUserDefined : PowerSystemStabilizerDynamics.RemoteInputSignal
        
          PowerSystemStabilizerUserDefined --> RemoteInputSignal : PowerSystemStabilizerDynamics.RemoteInputSignal
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [PowerSystemStabilizerDynamics](PowerSystemStabilizerDynamics.md)
            * **PowerSystemStabilizerUserDefined**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| proprietary | [cim:PowerSystemStabilizerUserDefined.proprietary](http://iec.ch/TC57/CIM100#PowerSystemStabilizerUserDefined.proprietary) | 1..1 <br />  boolean  | Behaviour is based on a proprietary model as opposed to a detailed model | direct |
| ProprietaryParameterDynamics | [cim:PowerSystemStabilizerUserDefined.ProprietaryParameterDynamics](http://iec.ch/TC57/CIM100#PowerSystemStabilizerUserDefined.ProprietaryParameterDynamics) | 0..* <br />  [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md)  | Parameter of this proprietary user-defined model | direct |
| RemoteInputSignal | [cim:PowerSystemStabilizerDynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#PowerSystemStabilizerDynamics.RemoteInputSignal) | 0..* <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this power system stabilizer model | [PowerSystemStabilizerDynamics](PowerSystemStabilizerDynamics.md) |
| ExcitationSystemDynamics | [cim:PowerSystemStabilizerDynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#PowerSystemStabilizerDynamics.ExcitationSystemDynamics) | 1..1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this power system stabilizer model is asso... | [PowerSystemStabilizerDynamics](PowerSystemStabilizerDynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1..1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md) | PowerSystemStabilizerUserDefined | range | [PowerSystemStabilizerUserDefined](PowerSystemStabilizerUserDefined.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:PowerSystemStabilizerUserDefined |
| native | this:PowerSystemStabilizerUserDefined |




