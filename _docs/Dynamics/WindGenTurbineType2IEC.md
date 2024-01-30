# WindGenTurbineType2IEC


_Wind turbine IEC type 2._

__

_Reference: IEC 61400-27-1:2015, 5.5.3._





**URI**: [cim:WindGenTurbineType2IEC](http://iec.ch/TC57/CIM100#WindGenTurbineType2IEC)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindGenTurbineType2IEC
      WindTurbineType1or2IEC <|-- WindGenTurbineType2IEC
      
      WindGenTurbineType2IEC : WindTurbineType1or2Dynamics.AsynchronousMachineDynamics
        
          WindGenTurbineType2IEC --> AsynchronousMachineDynamics : WindTurbineType1or2Dynamics.AsynchronousMachineDynamics
        
      WindGenTurbineType2IEC : IdentifiedObject.description
        
      WindGenTurbineType2IEC : DynamicsFunctionBlock.enabled
        
      WindGenTurbineType2IEC : IdentifiedObject.mRID
        
      WindGenTurbineType2IEC : IdentifiedObject.name
        
      WindGenTurbineType2IEC : WindTurbineType1or2Dynamics.RemoteInputSignal
        
          WindGenTurbineType2IEC --> RemoteInputSignal : WindTurbineType1or2Dynamics.RemoteInputSignal
        
      WindGenTurbineType2IEC : WindGenTurbineType2IEC.WindContRotorRIEC
        
          WindGenTurbineType2IEC --> WindContRotorRIEC : WindGenTurbineType2IEC.WindContRotorRIEC
        
      WindGenTurbineType2IEC : WindTurbineType1or2IEC.WindMechIEC
        
          WindGenTurbineType2IEC --> WindMechIEC : WindTurbineType1or2IEC.WindMechIEC
        
      WindGenTurbineType2IEC : WindGenTurbineType2IEC.WindPitchContPowerIEC
        
          WindGenTurbineType2IEC --> WindPitchContPowerIEC : WindGenTurbineType2IEC.WindPitchContPowerIEC
        
      WindGenTurbineType2IEC : WindTurbineType1or2IEC.WindProtectionIEC
        
          WindGenTurbineType2IEC --> WindProtectionIEC : WindTurbineType1or2IEC.WindProtectionIEC
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [WindTurbineType1or2Dynamics](WindTurbineType1or2Dynamics.md)
            * [WindTurbineType1or2IEC](WindTurbineType1or2IEC.md)
                * **WindGenTurbineType2IEC**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| WindContRotorRIEC | [cim:WindGenTurbineType2IEC.WindContRotorRIEC](http://iec.ch/TC57/CIM100#WindGenTurbineType2IEC.WindContRotorRIEC) | 1..1 <br />  [WindContRotorRIEC](WindContRotorRIEC.md)  | Wind control rotor resistance model associated with wind turbine type 2 model | direct |
| WindPitchContPowerIEC | [cim:WindGenTurbineType2IEC.WindPitchContPowerIEC](http://iec.ch/TC57/CIM100#WindGenTurbineType2IEC.WindPitchContPowerIEC) | 1..1 <br />  [WindPitchContPowerIEC](WindPitchContPowerIEC.md)  | Pitch control power model associated with this wind turbine type 2 model | direct |
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
| [WindContRotorRIEC](WindContRotorRIEC.md) | WindGenTurbineType2IEC | range | [WindGenTurbineType2IEC](WindGenTurbineType2IEC.md) |
| [WindPitchContPowerIEC](WindPitchContPowerIEC.md) | WindGenTurbineType2IEC | range | [WindGenTurbineType2IEC](WindGenTurbineType2IEC.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WindGenTurbineType2IEC |
| native | this:WindGenTurbineType2IEC |




