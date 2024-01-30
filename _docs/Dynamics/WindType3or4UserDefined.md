# WindType3or4UserDefined


_Wind type 3 or type 4 function block whose dynamic behaviour is described by <font color="#0f0f0f">a user-defined model.</font>_





**URI**: [cim:WindType3or4UserDefined](http://iec.ch/TC57/CIM100#WindType3or4UserDefined)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindType3or4UserDefined
      WindTurbineType3or4Dynamics <|-- WindType3or4UserDefined
      
      WindType3or4UserDefined : IdentifiedObject.description
        
      WindType3or4UserDefined : DynamicsFunctionBlock.enabled
        
      WindType3or4UserDefined : IdentifiedObject.mRID
        
      WindType3or4UserDefined : IdentifiedObject.name
        
      WindType3or4UserDefined : WindTurbineType3or4Dynamics.PowerElectronicsConnection
        
          WindType3or4UserDefined --> PowerElectronicsConnection : WindTurbineType3or4Dynamics.PowerElectronicsConnection
        
      WindType3or4UserDefined : WindType3or4UserDefined.proprietary
        
      WindType3or4UserDefined : WindType3or4UserDefined.ProprietaryParameterDynamics
        
          WindType3or4UserDefined --> ProprietaryParameterDynamics : WindType3or4UserDefined.ProprietaryParameterDynamics
        
      WindType3or4UserDefined : WindTurbineType3or4Dynamics.RemoteInputSignal
        
          WindType3or4UserDefined --> RemoteInputSignal : WindTurbineType3or4Dynamics.RemoteInputSignal
        
      WindType3or4UserDefined : WindTurbineType3or4Dynamics.WindPlantDynamics
        
          WindType3or4UserDefined --> WindPlantDynamics : WindTurbineType3or4Dynamics.WindPlantDynamics
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [WindTurbineType3or4Dynamics](WindTurbineType3or4Dynamics.md)
            * **WindType3or4UserDefined**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| proprietary | [cim:WindType3or4UserDefined.proprietary](http://iec.ch/TC57/CIM100#WindType3or4UserDefined.proprietary) | 1..1 <br />  boolean  | Behaviour is based on a proprietary model as opposed to a detailed model | direct |
| ProprietaryParameterDynamics | [cim:WindType3or4UserDefined.ProprietaryParameterDynamics](http://iec.ch/TC57/CIM100#WindType3or4UserDefined.ProprietaryParameterDynamics) | 0..* <br />  [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md)  | Parameter of this proprietary user-defined model | direct |
| PowerElectronicsConnection | [cim:WindTurbineType3or4Dynamics.PowerElectronicsConnection](http://iec.ch/TC57/CIM100#WindTurbineType3or4Dynamics.PowerElectronicsConnection) | 1..1 <br />  [PowerElectronicsConnection](PowerElectronicsConnection.md)  | The power electronics connection associated with this wind turbine type 3 or ... | [WindTurbineType3or4Dynamics](WindTurbineType3or4Dynamics.md) |
| RemoteInputSignal | [cim:WindTurbineType3or4Dynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#WindTurbineType3or4Dynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by these wind turbine type 3 or type 4 models | [WindTurbineType3or4Dynamics](WindTurbineType3or4Dynamics.md) |
| WindPlantDynamics | [cim:WindTurbineType3or4Dynamics.WindPlantDynamics](http://iec.ch/TC57/CIM100#WindTurbineType3or4Dynamics.WindPlantDynamics) | 0..1 <br />  [WindPlantDynamics](WindPlantDynamics.md)  | The wind plant with which the wind turbines type 3 or type 4 are associated | [WindTurbineType3or4Dynamics](WindTurbineType3or4Dynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1..1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md) | WindType3or4UserDefined | range | [WindType3or4UserDefined](WindType3or4UserDefined.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WindType3or4UserDefined |
| native | this:WindType3or4UserDefined |




