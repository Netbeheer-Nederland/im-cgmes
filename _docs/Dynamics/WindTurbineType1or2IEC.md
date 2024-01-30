# WindTurbineType1or2IEC


_Parent class supporting relationships to IEC wind turbines type 1 and type 2 including their control models._

_Generator model for wind turbine of IEC type 1 or type 2 is a standard asynchronous generator model._

_Reference: IEC 61400-27-1:2015, 5.5.2 and 5.5.3._





**URI**: [cim:WindTurbineType1or2IEC](http://iec.ch/TC57/CIM100#WindTurbineType1or2IEC)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindTurbineType1or2IEC
      WindTurbineType1or2Dynamics <|-- WindTurbineType1or2IEC
      

      WindTurbineType1or2IEC <|-- WindGenTurbineType1aIEC
      WindTurbineType1or2IEC <|-- WindGenTurbineType1bIEC
      WindTurbineType1or2IEC <|-- WindGenTurbineType2IEC
      
      
      WindTurbineType1or2IEC : WindTurbineType1or2Dynamics.AsynchronousMachineDynamics
        
          WindTurbineType1or2IEC --> AsynchronousMachineDynamics : WindTurbineType1or2Dynamics.AsynchronousMachineDynamics
        
      WindTurbineType1or2IEC : IdentifiedObject.description
        
      WindTurbineType1or2IEC : DynamicsFunctionBlock.enabled
        
      WindTurbineType1or2IEC : IdentifiedObject.mRID
        
      WindTurbineType1or2IEC : IdentifiedObject.name
        
      WindTurbineType1or2IEC : WindTurbineType1or2Dynamics.RemoteInputSignal
        
          WindTurbineType1or2IEC --> RemoteInputSignal : WindTurbineType1or2Dynamics.RemoteInputSignal
        
      WindTurbineType1or2IEC : WindTurbineType1or2IEC.WindMechIEC
        
          WindTurbineType1or2IEC --> WindMechIEC : WindTurbineType1or2IEC.WindMechIEC
        
      WindTurbineType1or2IEC : WindTurbineType1or2IEC.WindProtectionIEC
        
          WindTurbineType1or2IEC --> WindProtectionIEC : WindTurbineType1or2IEC.WindProtectionIEC
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [WindTurbineType1or2Dynamics](WindTurbineType1or2Dynamics.md)
            * **WindTurbineType1or2IEC**
                * [WindGenTurbineType1aIEC](WindGenTurbineType1aIEC.md)
                * [WindGenTurbineType1bIEC](WindGenTurbineType1bIEC.md)
                * [WindGenTurbineType2IEC](WindGenTurbineType2IEC.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| WindMechIEC | [cim:WindTurbineType1or2IEC.WindMechIEC](http://iec.ch/TC57/CIM100#WindTurbineType1or2IEC.WindMechIEC) | 1..1 <br />  [WindMechIEC](WindMechIEC.md)  | Wind mechanical model associated with this wind generator type 1 or type 2 mo... | direct |
| WindProtectionIEC | [cim:WindTurbineType1or2IEC.WindProtectionIEC](http://iec.ch/TC57/CIM100#WindTurbineType1or2IEC.WindProtectionIEC) | 1..1 <br />  [WindProtectionIEC](WindProtectionIEC.md)  | Wind turbune protection model associated with this wind generator type 1 or t... | direct |
| RemoteInputSignal | [cim:WindTurbineType1or2Dynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#WindTurbineType1or2Dynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this wind generator type 1 or type 2 model | [WindTurbineType1or2Dynamics](WindTurbineType1or2Dynamics.md) |
| AsynchronousMachineDynamics | [cim:WindTurbineType1or2Dynamics.AsynchronousMachineDynamics](http://iec.ch/TC57/CIM100#WindTurbineType1or2Dynamics.AsynchronousMachineDynamics) | 1..1 <br />  [AsynchronousMachineDynamics](AsynchronousMachineDynamics.md)  | Asynchronous machine model with which this wind generator type 1 or type 2 mo... | [WindTurbineType1or2Dynamics](WindTurbineType1or2Dynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1..1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [WindMechIEC](WindMechIEC.md) | WindTurbineType1or2IEC | range | [WindTurbineType1or2IEC](WindTurbineType1or2IEC.md) |
| [WindProtectionIEC](WindProtectionIEC.md) | WindTurbineType1or2IEC | range | [WindTurbineType1or2IEC](WindTurbineType1or2IEC.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WindTurbineType1or2IEC |
| native | this:WindTurbineType1or2IEC |




