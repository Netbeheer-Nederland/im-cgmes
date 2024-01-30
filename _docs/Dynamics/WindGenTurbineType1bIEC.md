# WindGenTurbineType1bIEC


_Wind turbine IEC type 1B._

__

_Reference: IEC 61400-27-1:2015, 5.5.2.3._





**URI**: [cim:WindGenTurbineType1bIEC](http://iec.ch/TC57/CIM100#WindGenTurbineType1bIEC)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindGenTurbineType1bIEC
      WindTurbineType1or2IEC <|-- WindGenTurbineType1bIEC
      
      WindGenTurbineType1bIEC : WindTurbineType1or2Dynamics.AsynchronousMachineDynamics
        
          WindGenTurbineType1bIEC --> AsynchronousMachineDynamics : WindTurbineType1or2Dynamics.AsynchronousMachineDynamics
        
      WindGenTurbineType1bIEC : IdentifiedObject.description
        
      WindGenTurbineType1bIEC : DynamicsFunctionBlock.enabled
        
      WindGenTurbineType1bIEC : IdentifiedObject.mRID
        
      WindGenTurbineType1bIEC : IdentifiedObject.name
        
      WindGenTurbineType1bIEC : WindTurbineType1or2Dynamics.RemoteInputSignal
        
          WindGenTurbineType1bIEC --> RemoteInputSignal : WindTurbineType1or2Dynamics.RemoteInputSignal
        
      WindGenTurbineType1bIEC : WindTurbineType1or2IEC.WindMechIEC
        
          WindGenTurbineType1bIEC --> WindMechIEC : WindTurbineType1or2IEC.WindMechIEC
        
      WindGenTurbineType1bIEC : WindGenTurbineType1bIEC.WindPitchContPowerIEC
        
          WindGenTurbineType1bIEC --> WindPitchContPowerIEC : WindGenTurbineType1bIEC.WindPitchContPowerIEC
        
      WindGenTurbineType1bIEC : WindTurbineType1or2IEC.WindProtectionIEC
        
          WindGenTurbineType1bIEC --> WindProtectionIEC : WindTurbineType1or2IEC.WindProtectionIEC
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [WindTurbineType1or2Dynamics](WindTurbineType1or2Dynamics.md)
            * [WindTurbineType1or2IEC](WindTurbineType1or2IEC.md)
                * **WindGenTurbineType1bIEC**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| WindPitchContPowerIEC | [cim:WindGenTurbineType1bIEC.WindPitchContPowerIEC](http://iec.ch/TC57/CIM100#WindGenTurbineType1bIEC.WindPitchContPowerIEC) | 1..1 <br />  [WindPitchContPowerIEC](WindPitchContPowerIEC.md)  | Pitch control power model associated with this wind turbine type 1B model | direct |
| WindMechIEC | [cim:WindTurbineType1or2IEC.WindMechIEC](http://iec.ch/TC57/CIM100#WindTurbineType1or2IEC.WindMechIEC) | 1..1 <br />  [WindMechIEC](WindMechIEC.md)  | Wind mechanical model associated with this wind generator type 1 or type 2 mo... | [WindTurbineType1or2IEC](WindTurbineType1or2IEC.md) |
| WindProtectionIEC | [cim:WindTurbineType1or2IEC.WindProtectionIEC](http://iec.ch/TC57/CIM100#WindTurbineType1or2IEC.WindProtectionIEC) | 1..1 <br />  [WindProtectionIEC](WindProtectionIEC.md)  | Wind turbune protection model associated with this wind generator type 1 or t... | [WindTurbineType1or2IEC](WindTurbineType1or2IEC.md) |
| RemoteInputSignal | [cim:WindTurbineType1or2Dynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#WindTurbineType1or2Dynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this wind generator type 1 or type 2 model | [WindTurbineType1or2Dynamics](WindTurbineType1or2Dynamics.md) |
| AsynchronousMachineDynamics | [cim:WindTurbineType1or2Dynamics.AsynchronousMachineDynamics](http://iec.ch/TC57/CIM100#WindTurbineType1or2Dynamics.AsynchronousMachineDynamics) | 1..1 <br />  [AsynchronousMachineDynamics](AsynchronousMachineDynamics.md)  | Asynchronous machine model with which this wind generator type 1 or type 2 mo... | [WindTurbineType1or2Dynamics](WindTurbineType1or2Dynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1..1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [WindPitchContPowerIEC](WindPitchContPowerIEC.md) | WindGenTurbineType1bIEC | range | [WindGenTurbineType1bIEC](WindGenTurbineType1bIEC.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WindGenTurbineType1bIEC |
| native | this:WindGenTurbineType1bIEC |




