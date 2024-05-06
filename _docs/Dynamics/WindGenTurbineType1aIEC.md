# WindGenTurbineType1aIEC


_Wind turbine IEC type 1A._

_Reference: IEC 61400-27-1:2015, 5.5.2.2._





**URI**: [cim:WindGenTurbineType1aIEC](http://iec.ch/TC57/CIM100#WindGenTurbineType1aIEC)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindGenTurbineType1aIEC
    click WindGenTurbineType1aIEC href "../WindGenTurbineType1aIEC"
      WindTurbineType1or2IEC <|-- WindGenTurbineType1aIEC
        click WindTurbineType1or2IEC href "../WindTurbineType1or2IEC"
      
      WindGenTurbineType1aIEC : WindTurbineType1or2Dynamics.AsynchronousMachineDynamics
        
          WindGenTurbineType1aIEC --> AsynchronousMachineDynamics : WindTurbineType1or2Dynamics.AsynchronousMachineDynamics
          click AsynchronousMachineDynamics href "../AsynchronousMachineDynamics"
        
      WindGenTurbineType1aIEC : IdentifiedObject.description
        
      WindGenTurbineType1aIEC : DynamicsFunctionBlock.enabled
        
      WindGenTurbineType1aIEC : IdentifiedObject.mRID
        
      WindGenTurbineType1aIEC : IdentifiedObject.name
        
      WindGenTurbineType1aIEC : WindTurbineType1or2Dynamics.RemoteInputSignal
        
          WindGenTurbineType1aIEC --> RemoteInputSignal : WindTurbineType1or2Dynamics.RemoteInputSignal
          click RemoteInputSignal href "../RemoteInputSignal"
        
      WindGenTurbineType1aIEC : WindGenTurbineType1aIEC.WindAeroConstIEC
        
          WindGenTurbineType1aIEC --> WindAeroConstIEC : WindGenTurbineType1aIEC.WindAeroConstIEC
          click WindAeroConstIEC href "../WindAeroConstIEC"
        
      WindGenTurbineType1aIEC : WindTurbineType1or2IEC.WindMechIEC
        
          WindGenTurbineType1aIEC --> WindMechIEC : WindTurbineType1or2IEC.WindMechIEC
          click WindMechIEC href "../WindMechIEC"
        
      WindGenTurbineType1aIEC : WindTurbineType1or2IEC.WindProtectionIEC
        
          WindGenTurbineType1aIEC --> WindProtectionIEC : WindTurbineType1or2IEC.WindProtectionIEC
          click WindProtectionIEC href "../WindProtectionIEC"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [WindTurbineType1or2Dynamics](WindTurbineType1or2Dynamics.md)
            * [WindTurbineType1or2IEC](WindTurbineType1or2IEC.md)
                * **WindGenTurbineType1aIEC**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| WindAeroConstIEC | [cim:WindGenTurbineType1aIEC.WindAeroConstIEC](http://iec.ch/TC57/CIM100#WindGenTurbineType1aIEC.WindAeroConstIEC) | 1 <br />  [WindAeroConstIEC](WindAeroConstIEC.md)  | Wind aerodynamic model associated with this wind turbine type 1A model | direct |
| WindMechIEC | [cim:WindTurbineType1or2IEC.WindMechIEC](http://iec.ch/TC57/CIM100#WindTurbineType1or2IEC.WindMechIEC) | 1 <br />  [WindMechIEC](WindMechIEC.md)  | Wind mechanical model associated with this wind generator type 1 or type 2 mo... | [WindTurbineType1or2IEC](WindTurbineType1or2IEC.md) |
| WindProtectionIEC | [cim:WindTurbineType1or2IEC.WindProtectionIEC](http://iec.ch/TC57/CIM100#WindTurbineType1or2IEC.WindProtectionIEC) | 1 <br />  [WindProtectionIEC](WindProtectionIEC.md)  | Wind turbune protection model associated with this wind generator type 1 or t... | [WindTurbineType1or2IEC](WindTurbineType1or2IEC.md) |
| RemoteInputSignal | [cim:WindTurbineType1or2Dynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#WindTurbineType1or2Dynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this wind generator type 1 or type 2 model | [WindTurbineType1or2Dynamics](WindTurbineType1or2Dynamics.md) |
| AsynchronousMachineDynamics | [cim:WindTurbineType1or2Dynamics.AsynchronousMachineDynamics](http://iec.ch/TC57/CIM100#WindTurbineType1or2Dynamics.AsynchronousMachineDynamics) | 1 <br />  [AsynchronousMachineDynamics](AsynchronousMachineDynamics.md)  | Asynchronous machine model with which this wind generator type 1 or type 2 mo... | [WindTurbineType1or2Dynamics](WindTurbineType1or2Dynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [WindAeroConstIEC](WindAeroConstIEC.md) | WindGenTurbineType1aIEC | range | [WindGenTurbineType1aIEC](WindGenTurbineType1aIEC.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WindGenTurbineType1aIEC |
| native | this:WindGenTurbineType1aIEC |




