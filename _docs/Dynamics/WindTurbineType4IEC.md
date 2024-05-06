# WindTurbineType4IEC


_Parent class supporting relationships to IEC wind turbines type 4 including their control models._





**URI**: [cim:WindTurbineType4IEC](http://iec.ch/TC57/CIM100#WindTurbineType4IEC)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindTurbineType4IEC
    click WindTurbineType4IEC href "../WindTurbineType4IEC"
      WindTurbineType3or4IEC <|-- WindTurbineType4IEC
        click WindTurbineType3or4IEC href "../WindTurbineType3or4IEC"
      

      WindTurbineType4IEC <|-- WindTurbineType4aIEC
        click WindTurbineType4aIEC href "../WindTurbineType4aIEC"
      WindTurbineType4IEC <|-- WindTurbineType4bIEC
        click WindTurbineType4bIEC href "../WindTurbineType4bIEC"
      
      
      WindTurbineType4IEC : IdentifiedObject.description
        
      WindTurbineType4IEC : DynamicsFunctionBlock.enabled
        
      WindTurbineType4IEC : IdentifiedObject.mRID
        
      WindTurbineType4IEC : IdentifiedObject.name
        
      WindTurbineType4IEC : WindTurbineType3or4Dynamics.PowerElectronicsConnection
        
          WindTurbineType4IEC --> PowerElectronicsConnection : WindTurbineType3or4Dynamics.PowerElectronicsConnection
          click PowerElectronicsConnection href "../PowerElectronicsConnection"
        
      WindTurbineType4IEC : WindTurbineType3or4Dynamics.RemoteInputSignal
        
          WindTurbineType4IEC --> RemoteInputSignal : WindTurbineType3or4Dynamics.RemoteInputSignal
          click RemoteInputSignal href "../RemoteInputSignal"
        
      WindTurbineType4IEC : WindTurbineType3or4IEC.WindContCurrLimIEC
        
          WindTurbineType4IEC --> WindContCurrLimIEC : WindTurbineType3or4IEC.WindContCurrLimIEC
          click WindContCurrLimIEC href "../WindContCurrLimIEC"
        
      WindTurbineType4IEC : WindTurbineType3or4IEC.WIndContQIEC
        
          WindTurbineType4IEC --> WindContQIEC : WindTurbineType3or4IEC.WIndContQIEC
          click WindContQIEC href "../WindContQIEC"
        
      WindTurbineType4IEC : WindTurbineType3or4IEC.WindContQLimIEC
        
          WindTurbineType4IEC --> WindContQLimIEC : WindTurbineType3or4IEC.WindContQLimIEC
          click WindContQLimIEC href "../WindContQLimIEC"
        
      WindTurbineType4IEC : WindTurbineType3or4IEC.WindContQPQULimIEC
        
          WindTurbineType4IEC --> WindContQPQULimIEC : WindTurbineType3or4IEC.WindContQPQULimIEC
          click WindContQPQULimIEC href "../WindContQPQULimIEC"
        
      WindTurbineType4IEC : WindTurbineType4IEC.WindGenType3aIEC
        
          WindTurbineType4IEC --> WindGenType3aIEC : WindTurbineType4IEC.WindGenType3aIEC
          click WindGenType3aIEC href "../WindGenType3aIEC"
        
      WindTurbineType4IEC : WindTurbineType3or4Dynamics.WindPlantDynamics
        
          WindTurbineType4IEC --> WindPlantDynamics : WindTurbineType3or4Dynamics.WindPlantDynamics
          click WindPlantDynamics href "../WindPlantDynamics"
        
      WindTurbineType4IEC : WindTurbineType3or4IEC.WindProtectionIEC
        
          WindTurbineType4IEC --> WindProtectionIEC : WindTurbineType3or4IEC.WindProtectionIEC
          click WindProtectionIEC href "../WindProtectionIEC"
        
      WindTurbineType4IEC : WindTurbineType3or4IEC.WindRefFrameRotIEC
        
          WindTurbineType4IEC --> WindRefFrameRotIEC : WindTurbineType3or4IEC.WindRefFrameRotIEC
          click WindRefFrameRotIEC href "../WindRefFrameRotIEC"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [WindTurbineType3or4Dynamics](WindTurbineType3or4Dynamics.md)
            * [WindTurbineType3or4IEC](WindTurbineType3or4IEC.md)
                * **WindTurbineType4IEC**
                    * [WindTurbineType4aIEC](WindTurbineType4aIEC.md)
                    * [WindTurbineType4bIEC](WindTurbineType4bIEC.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| WindGenType3aIEC | [cim:WindTurbineType4IEC.WindGenType3aIEC](http://iec.ch/TC57/CIM100#WindTurbineType4IEC.WindGenType3aIEC) | 0..1 <br />  [WindGenType3aIEC](WindGenType3aIEC.md)  | Wind generator type 3A model associated with this wind turbine type 4 model | direct |
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
| [WindGenType3aIEC](WindGenType3aIEC.md) | WindTurbineType4IEC | range | [WindTurbineType4IEC](WindTurbineType4IEC.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WindTurbineType4IEC |
| native | this:WindTurbineType4IEC |




