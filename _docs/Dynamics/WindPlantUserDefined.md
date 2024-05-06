# WindPlantUserDefined


_Wind plant function block whose dynamic behaviour is described by <font color="#0f0f0f">a user-defined model.</font>_





**URI**: [cim:WindPlantUserDefined](http://iec.ch/TC57/CIM100#WindPlantUserDefined)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindPlantUserDefined
    click WindPlantUserDefined href "../WindPlantUserDefined"
      WindPlantDynamics <|-- WindPlantUserDefined
        click WindPlantDynamics href "../WindPlantDynamics"
      
      WindPlantUserDefined : IdentifiedObject.description
        
      WindPlantUserDefined : DynamicsFunctionBlock.enabled
        
      WindPlantUserDefined : IdentifiedObject.mRID
        
      WindPlantUserDefined : IdentifiedObject.name
        
      WindPlantUserDefined : WindPlantUserDefined.proprietary
        
      WindPlantUserDefined : WindPlantUserDefined.ProprietaryParameterDynamics
        
          WindPlantUserDefined --> ProprietaryParameterDynamics : WindPlantUserDefined.ProprietaryParameterDynamics
          click ProprietaryParameterDynamics href "../ProprietaryParameterDynamics"
        
      WindPlantUserDefined : WindPlantDynamics.RemoteInputSignal
        
          WindPlantUserDefined --> RemoteInputSignal : WindPlantDynamics.RemoteInputSignal
          click RemoteInputSignal href "../RemoteInputSignal"
        
      WindPlantUserDefined : WindPlantDynamics.WindTurbineType3or4Dynamics
        
          WindPlantUserDefined --> WindTurbineType3or4Dynamics : WindPlantDynamics.WindTurbineType3or4Dynamics
          click WindTurbineType3or4Dynamics href "../WindTurbineType3or4Dynamics"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [WindPlantDynamics](WindPlantDynamics.md)
            * **WindPlantUserDefined**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| proprietary | [cim:WindPlantUserDefined.proprietary](http://iec.ch/TC57/CIM100#WindPlantUserDefined.proprietary) | 1 <br />  boolean  | Behaviour is based on a proprietary model as opposed to a detailed model | direct |
| ProprietaryParameterDynamics | [cim:WindPlantUserDefined.ProprietaryParameterDynamics](http://iec.ch/TC57/CIM100#WindPlantUserDefined.ProprietaryParameterDynamics) | * <br />  [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md)  | Parameter of this proprietary user-defined model | direct |
| RemoteInputSignal | [cim:WindPlantDynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#WindPlantDynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | The remote signal with which this power plant is associated | [WindPlantDynamics](WindPlantDynamics.md) |
| WindTurbineType3or4Dynamics | [cim:WindPlantDynamics.WindTurbineType3or4Dynamics](http://iec.ch/TC57/CIM100#WindPlantDynamics.WindTurbineType3or4Dynamics) | 1..* <br />  [WindTurbineType3or4Dynamics](WindTurbineType3or4Dynamics.md)  | The wind turbine type 3 or type 4 associated with this wind plant | [WindPlantDynamics](WindPlantDynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md) | WindPlantUserDefined | range | [WindPlantUserDefined](WindPlantUserDefined.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WindPlantUserDefined |
| native | this:WindPlantUserDefined |




