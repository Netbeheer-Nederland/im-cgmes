# WindTurbineType3IEC


_Parent class supporting relationships to IEC wind turbines type 3 including their control models._





**URI**: [cim:WindTurbineType3IEC](http://iec.ch/TC57/CIM100#WindTurbineType3IEC)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindTurbineType3IEC
    click WindTurbineType3IEC href "../WindTurbineType3IEC"
      WindTurbineType3or4IEC <|-- WindTurbineType3IEC
        click WindTurbineType3or4IEC href "../WindTurbineType3or4IEC"
      
      WindTurbineType3IEC : IdentifiedObject.description
        
      WindTurbineType3IEC : DynamicsFunctionBlock.enabled
        
      WindTurbineType3IEC : IdentifiedObject.mRID
        
      WindTurbineType3IEC : IdentifiedObject.name
        
      WindTurbineType3IEC : WindTurbineType3or4Dynamics.PowerElectronicsConnection
        
          WindTurbineType3IEC --> PowerElectronicsConnection : WindTurbineType3or4Dynamics.PowerElectronicsConnection
          click PowerElectronicsConnection href "../PowerElectronicsConnection"
        
      WindTurbineType3IEC : WindTurbineType3or4Dynamics.RemoteInputSignal
        
          WindTurbineType3IEC --> RemoteInputSignal : WindTurbineType3or4Dynamics.RemoteInputSignal
          click RemoteInputSignal href "../RemoteInputSignal"
        
      WindTurbineType3IEC : WindTurbineType3IEC.WindAeroOneDimIEC
        
          WindTurbineType3IEC --> WindAeroOneDimIEC : WindTurbineType3IEC.WindAeroOneDimIEC
          click WindAeroOneDimIEC href "../WindAeroOneDimIEC"
        
      WindTurbineType3IEC : WindTurbineType3IEC.WindAeroTwoDimIEC
        
          WindTurbineType3IEC --> WindAeroTwoDimIEC : WindTurbineType3IEC.WindAeroTwoDimIEC
          click WindAeroTwoDimIEC href "../WindAeroTwoDimIEC"
        
      WindTurbineType3IEC : WindTurbineType3or4IEC.WindContCurrLimIEC
        
          WindTurbineType3IEC --> WindContCurrLimIEC : WindTurbineType3or4IEC.WindContCurrLimIEC
          click WindContCurrLimIEC href "../WindContCurrLimIEC"
        
      WindTurbineType3IEC : WindTurbineType3IEC.WindContPitchAngleIEC
        
          WindTurbineType3IEC --> WindContPitchAngleIEC : WindTurbineType3IEC.WindContPitchAngleIEC
          click WindContPitchAngleIEC href "../WindContPitchAngleIEC"
        
      WindTurbineType3IEC : WindTurbineType3IEC.WindContPType3IEC
        
          WindTurbineType3IEC --> WindContPType3IEC : WindTurbineType3IEC.WindContPType3IEC
          click WindContPType3IEC href "../WindContPType3IEC"
        
      WindTurbineType3IEC : WindTurbineType3or4IEC.WIndContQIEC
        
          WindTurbineType3IEC --> WindContQIEC : WindTurbineType3or4IEC.WIndContQIEC
          click WindContQIEC href "../WindContQIEC"
        
      WindTurbineType3IEC : WindTurbineType3or4IEC.WindContQLimIEC
        
          WindTurbineType3IEC --> WindContQLimIEC : WindTurbineType3or4IEC.WindContQLimIEC
          click WindContQLimIEC href "../WindContQLimIEC"
        
      WindTurbineType3IEC : WindTurbineType3or4IEC.WindContQPQULimIEC
        
          WindTurbineType3IEC --> WindContQPQULimIEC : WindTurbineType3or4IEC.WindContQPQULimIEC
          click WindContQPQULimIEC href "../WindContQPQULimIEC"
        
      WindTurbineType3IEC : WindTurbineType3IEC.WindGenType3IEC
        
          WindTurbineType3IEC --> WindGenType3IEC : WindTurbineType3IEC.WindGenType3IEC
          click WindGenType3IEC href "../WindGenType3IEC"
        
      WindTurbineType3IEC : WindTurbineType3IEC.WindMechIEC
        
          WindTurbineType3IEC --> WindMechIEC : WindTurbineType3IEC.WindMechIEC
          click WindMechIEC href "../WindMechIEC"
        
      WindTurbineType3IEC : WindTurbineType3or4Dynamics.WindPlantDynamics
        
          WindTurbineType3IEC --> WindPlantDynamics : WindTurbineType3or4Dynamics.WindPlantDynamics
          click WindPlantDynamics href "../WindPlantDynamics"
        
      WindTurbineType3IEC : WindTurbineType3or4IEC.WindProtectionIEC
        
          WindTurbineType3IEC --> WindProtectionIEC : WindTurbineType3or4IEC.WindProtectionIEC
          click WindProtectionIEC href "../WindProtectionIEC"
        
      WindTurbineType3IEC : WindTurbineType3or4IEC.WindRefFrameRotIEC
        
          WindTurbineType3IEC --> WindRefFrameRotIEC : WindTurbineType3or4IEC.WindRefFrameRotIEC
          click WindRefFrameRotIEC href "../WindRefFrameRotIEC"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [WindTurbineType3or4Dynamics](WindTurbineType3or4Dynamics.md)
            * [WindTurbineType3or4IEC](WindTurbineType3or4IEC.md)
                * **WindTurbineType3IEC**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| WindAeroOneDimIEC | [cim:WindTurbineType3IEC.WindAeroOneDimIEC](http://iec.ch/TC57/CIM100#WindTurbineType3IEC.WindAeroOneDimIEC) | 0..1 <br />  [WindAeroOneDimIEC](WindAeroOneDimIEC.md)  | Wind aerodynamic model associated with this wind generator type 3 model | direct |
| WindAeroTwoDimIEC | [cim:WindTurbineType3IEC.WindAeroTwoDimIEC](http://iec.ch/TC57/CIM100#WindTurbineType3IEC.WindAeroTwoDimIEC) | 0..1 <br />  [WindAeroTwoDimIEC](WindAeroTwoDimIEC.md)  | Wind aerodynamic model associated with this wind turbine type 3 model | direct |
| WindContPitchAngleIEC | [cim:WindTurbineType3IEC.WindContPitchAngleIEC](http://iec.ch/TC57/CIM100#WindTurbineType3IEC.WindContPitchAngleIEC) | 1 <br />  [WindContPitchAngleIEC](WindContPitchAngleIEC.md)  | Wind control pitch angle model associated with this wind turbine type 3 | direct |
| WindContPType3IEC | [cim:WindTurbineType3IEC.WindContPType3IEC](http://iec.ch/TC57/CIM100#WindTurbineType3IEC.WindContPType3IEC) | 1 <br />  [WindContPType3IEC](WindContPType3IEC.md)  | Wind control P type 3 model associated with this wind turbine type 3 model | direct |
| WindGenType3IEC | [cim:WindTurbineType3IEC.WindGenType3IEC](http://iec.ch/TC57/CIM100#WindTurbineType3IEC.WindGenType3IEC) | 0..1 <br />  [WindGenType3IEC](WindGenType3IEC.md)  | Wind generator type 3 model associated with this wind turbine type 3 model | direct |
| WindMechIEC | [cim:WindTurbineType3IEC.WindMechIEC](http://iec.ch/TC57/CIM100#WindTurbineType3IEC.WindMechIEC) | 1 <br />  [WindMechIEC](WindMechIEC.md)  | Wind mechanical model associated with this wind turbine type 3 model | direct |
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
| [WindAeroOneDimIEC](WindAeroOneDimIEC.md) | WindTurbineType3IEC | range | [WindTurbineType3IEC](WindTurbineType3IEC.md) |
| [WindAeroTwoDimIEC](WindAeroTwoDimIEC.md) | WindTurbineType3IEC | range | [WindTurbineType3IEC](WindTurbineType3IEC.md) |
| [WindContPitchAngleIEC](WindContPitchAngleIEC.md) | WindTurbineType3IEC | range | [WindTurbineType3IEC](WindTurbineType3IEC.md) |
| [WindContPType3IEC](WindContPType3IEC.md) | WindTurbineType3IEC | range | [WindTurbineType3IEC](WindTurbineType3IEC.md) |
| [WindGenType3aIEC](WindGenType3aIEC.md) | WindTurbineType3IEC | range | [WindTurbineType3IEC](WindTurbineType3IEC.md) |
| [WindGenType3bIEC](WindGenType3bIEC.md) | WindTurbineType3IEC | range | [WindTurbineType3IEC](WindTurbineType3IEC.md) |
| [WindGenType3IEC](WindGenType3IEC.md) | WindTurbineType3IEC | range | [WindTurbineType3IEC](WindTurbineType3IEC.md) |
| [WindMechIEC](WindMechIEC.md) | WindTurbineType3IEC | range | [WindTurbineType3IEC](WindTurbineType3IEC.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WindTurbineType3IEC |
| native | this:WindTurbineType3IEC |




