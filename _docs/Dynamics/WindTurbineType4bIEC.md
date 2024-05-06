# WindTurbineType4bIEC


_Wind turbine IEC type 4B._

_Reference: IEC 61400-27-1:2015, 5.5.5.3._





**URI**: [cim:WindTurbineType4bIEC](http://iec.ch/TC57/CIM100#WindTurbineType4bIEC)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindTurbineType4bIEC
    click WindTurbineType4bIEC href "../WindTurbineType4bIEC"
      WindTurbineType4IEC <|-- WindTurbineType4bIEC
        click WindTurbineType4IEC href "../WindTurbineType4IEC"
      
      WindTurbineType4bIEC : IdentifiedObject.description
        
      WindTurbineType4bIEC : DynamicsFunctionBlock.enabled
        
      WindTurbineType4bIEC : IdentifiedObject.mRID
        
      WindTurbineType4bIEC : IdentifiedObject.name
        
      WindTurbineType4bIEC : WindTurbineType3or4Dynamics.PowerElectronicsConnection
        
          WindTurbineType4bIEC --> PowerElectronicsConnection : WindTurbineType3or4Dynamics.PowerElectronicsConnection
          click PowerElectronicsConnection href "../PowerElectronicsConnection"
        
      WindTurbineType4bIEC : WindTurbineType3or4Dynamics.RemoteInputSignal
        
          WindTurbineType4bIEC --> RemoteInputSignal : WindTurbineType3or4Dynamics.RemoteInputSignal
          click RemoteInputSignal href "../RemoteInputSignal"
        
      WindTurbineType4bIEC : WindTurbineType3or4IEC.WindContCurrLimIEC
        
          WindTurbineType4bIEC --> WindContCurrLimIEC : WindTurbineType3or4IEC.WindContCurrLimIEC
          click WindContCurrLimIEC href "../WindContCurrLimIEC"
        
      WindTurbineType4bIEC : WindTurbineType4bIEC.WindContPType4bIEC
        
          WindTurbineType4bIEC --> WindContPType4bIEC : WindTurbineType4bIEC.WindContPType4bIEC
          click WindContPType4bIEC href "../WindContPType4bIEC"
        
      WindTurbineType4bIEC : WindTurbineType3or4IEC.WIndContQIEC
        
          WindTurbineType4bIEC --> WindContQIEC : WindTurbineType3or4IEC.WIndContQIEC
          click WindContQIEC href "../WindContQIEC"
        
      WindTurbineType4bIEC : WindTurbineType3or4IEC.WindContQLimIEC
        
          WindTurbineType4bIEC --> WindContQLimIEC : WindTurbineType3or4IEC.WindContQLimIEC
          click WindContQLimIEC href "../WindContQLimIEC"
        
      WindTurbineType4bIEC : WindTurbineType3or4IEC.WindContQPQULimIEC
        
          WindTurbineType4bIEC --> WindContQPQULimIEC : WindTurbineType3or4IEC.WindContQPQULimIEC
          click WindContQPQULimIEC href "../WindContQPQULimIEC"
        
      WindTurbineType4bIEC : WindTurbineType4IEC.WindGenType3aIEC
        
          WindTurbineType4bIEC --> WindGenType3aIEC : WindTurbineType4IEC.WindGenType3aIEC
          click WindGenType3aIEC href "../WindGenType3aIEC"
        
      WindTurbineType4bIEC : WindTurbineType4bIEC.WindGenType4IEC
        
          WindTurbineType4bIEC --> WindGenType4IEC : WindTurbineType4bIEC.WindGenType4IEC
          click WindGenType4IEC href "../WindGenType4IEC"
        
      WindTurbineType4bIEC : WindTurbineType4bIEC.WindMechIEC
        
          WindTurbineType4bIEC --> WindMechIEC : WindTurbineType4bIEC.WindMechIEC
          click WindMechIEC href "../WindMechIEC"
        
      WindTurbineType4bIEC : WindTurbineType3or4Dynamics.WindPlantDynamics
        
          WindTurbineType4bIEC --> WindPlantDynamics : WindTurbineType3or4Dynamics.WindPlantDynamics
          click WindPlantDynamics href "../WindPlantDynamics"
        
      WindTurbineType4bIEC : WindTurbineType3or4IEC.WindProtectionIEC
        
          WindTurbineType4bIEC --> WindProtectionIEC : WindTurbineType3or4IEC.WindProtectionIEC
          click WindProtectionIEC href "../WindProtectionIEC"
        
      WindTurbineType4bIEC : WindTurbineType3or4IEC.WindRefFrameRotIEC
        
          WindTurbineType4bIEC --> WindRefFrameRotIEC : WindTurbineType3or4IEC.WindRefFrameRotIEC
          click WindRefFrameRotIEC href "../WindRefFrameRotIEC"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [WindTurbineType3or4Dynamics](WindTurbineType3or4Dynamics.md)
            * [WindTurbineType3or4IEC](WindTurbineType3or4IEC.md)
                * [WindTurbineType4IEC](WindTurbineType4IEC.md)
                    * **WindTurbineType4bIEC**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| WindContPType4bIEC | [cim:WindTurbineType4bIEC.WindContPType4bIEC](http://iec.ch/TC57/CIM100#WindTurbineType4bIEC.WindContPType4bIEC) | 1 <br />  [WindContPType4bIEC](WindContPType4bIEC.md)  | Wind control P type 4B model associated with this wind turbine type 4B model | direct |
| WindGenType4IEC | [cim:WindTurbineType4bIEC.WindGenType4IEC](http://iec.ch/TC57/CIM100#WindTurbineType4bIEC.WindGenType4IEC) | 0..1 <br />  [WindGenType4IEC](WindGenType4IEC.md)  | Wind generator type 4 model associated with this wind turbine type 4B model | direct |
| WindMechIEC | [cim:WindTurbineType4bIEC.WindMechIEC](http://iec.ch/TC57/CIM100#WindTurbineType4bIEC.WindMechIEC) | 1 <br />  [WindMechIEC](WindMechIEC.md)  | Wind mechanical model associated with this wind turbine type 4B model | direct |
| WindGenType3aIEC | [cim:WindTurbineType4IEC.WindGenType3aIEC](http://iec.ch/TC57/CIM100#WindTurbineType4IEC.WindGenType3aIEC) | 0..1 <br />  [WindGenType3aIEC](WindGenType3aIEC.md)  | Wind generator type 3A model associated with this wind turbine type 4 model | [WindTurbineType4IEC](WindTurbineType4IEC.md) |
| WindContCurrLimIEC | [cim:WindTurbineType3or4IEC.WindContCurrLimIEC](http://iec.ch/TC57/CIM100#WindTurbineType3or4IEC.WindContCurrLimIEC) | 1 <br />  [WindContCurrLimIEC](WindContCurrLimIEC.md)  | Wind control current limitation model associated with this wind turbine type ... | [WindTurbineType3or4IEC](WindTurbineType3or4IEC.md) |
| WIndContQIEC | [cim:WindTurbineType3or4IEC.WIndContQIEC](http://iec.ch/TC57/CIM100#WindTurbineType3or4IEC.WIndContQIEC) | 1 <br />  [WindContQIEC](WindContQIEC.md)  | Wind control Q model associated with this wind turbine type 3 or type 4 model | [WindTurbineType3or4IEC](WindTurbineType3or4IEC.md) |
| WindContQLimIEC | [cim:WindTurbineType3or4IEC.WindContQLimIEC](http://iec.ch/TC57/CIM100#WindTurbineType3or4IEC.WindContQLimIEC) | 0..1 <br />  [WindContQLimIEC](WindContQLimIEC.md)  | Constant Q limitation model associated with this wind generator type 3 or typ... | [WindTurbineType3or4IEC](WindTurbineType3or4IEC.md) |
| WindContQPQULimIEC | [cim:WindTurbineType3or4IEC.WindContQPQULimIEC](http://iec.ch/TC57/CIM100#WindTurbineType3or4IEC.WindContQPQULimIEC) | 0..1 <br />  [WindContQPQULimIEC](WindContQPQULimIEC.md)  | QP and QU limitation model associated with this wind generator type 3 or type... | [WindTurbineType3or4IEC](WindTurbineType3or4IEC.md) |
| WindProtectionIEC | [cim:WindTurbineType3or4IEC.WindProtectionIEC](http://iec.ch/TC57/CIM100#WindTurbineType3or4IEC.WindProtectionIEC) | 1 <br />  [WindProtectionIEC](WindProtectionIEC.md)  | Wind turbune protection model associated with this wind generator type 3 or t... | [WindTurbineType3or4IEC](WindTurbineType3or4IEC.md) |
| WindRefFrameRotIEC | [cim:WindTurbineType3or4IEC.WindRefFrameRotIEC](http://iec.ch/TC57/CIM100#WindTurbineType3or4IEC.WindRefFrameRotIEC) | 1 <br />  [WindRefFrameRotIEC](WindRefFrameRotIEC.md)  | Reference frame rotation model associated with this wind turbine type 3 or ty... | [WindTurbineType3or4IEC](WindTurbineType3or4IEC.md) |
| PowerElectronicsConnection | [cim:WindTurbineType3or4Dynamics.PowerElectronicsConnection](http://iec.ch/TC57/CIM100#WindTurbineType3or4Dynamics.PowerElectronicsConnection) | 1 <br />  [PowerElectronicsConnection](PowerElectronicsConnection.md)  | The power electronics connection associated with this wind turbine type 3 or ... | [WindTurbineType3or4Dynamics](WindTurbineType3or4Dynamics.md) |
| RemoteInputSignal | [cim:WindTurbineType3or4Dynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#WindTurbineType3or4Dynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by these wind turbine type 3 or type 4 models | [WindTurbineType3or4Dynamics](WindTurbineType3or4Dynamics.md) |
| WindPlantDynamics | [cim:WindTurbineType3or4Dynamics.WindPlantDynamics](http://iec.ch/TC57/CIM100#WindTurbineType3or4Dynamics.WindPlantDynamics) | 0..1 <br />  [WindPlantDynamics](WindPlantDynamics.md)  | The wind plant with which the wind turbines type 3 or type 4 are associated | [WindTurbineType3or4Dynamics](WindTurbineType3or4Dynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [WindContPType4bIEC](WindContPType4bIEC.md) | WindTurbineType4bIEC | range | [WindTurbineType4bIEC](WindTurbineType4bIEC.md) |
| [WindGenType4IEC](WindGenType4IEC.md) | WindTurbineType4bIEC | range | [WindTurbineType4bIEC](WindTurbineType4bIEC.md) |
| [WindMechIEC](WindMechIEC.md) | WindTurbineType4bIEC | range | [WindTurbineType4bIEC](WindTurbineType4bIEC.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WindTurbineType4bIEC |
| native | this:WindTurbineType4bIEC |




