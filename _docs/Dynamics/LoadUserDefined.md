# LoadUserDefined


_Load whose dynamic behaviour is described by a user-defined model._





**URI**: [cim:LoadUserDefined](http://iec.ch/TC57/CIM100#LoadUserDefined)<br />
**Type**: Class




```mermaid
 classDiagram
    class LoadUserDefined
    click LoadUserDefined href "../LoadUserDefined"
      LoadDynamics <|-- LoadUserDefined
        click LoadDynamics href "../LoadDynamics"
      
      LoadUserDefined : IdentifiedObject.description
        
      LoadUserDefined : LoadDynamics.EnergyConsumer
        
          LoadUserDefined --> EnergyConsumer : LoadDynamics.EnergyConsumer
          click EnergyConsumer href "../EnergyConsumer"
        
      LoadUserDefined : IdentifiedObject.mRID
        
      LoadUserDefined : IdentifiedObject.name
        
      LoadUserDefined : LoadUserDefined.proprietary
        
      LoadUserDefined : LoadUserDefined.ProprietaryParameterDynamics
        
          LoadUserDefined --> ProprietaryParameterDynamics : LoadUserDefined.ProprietaryParameterDynamics
          click ProprietaryParameterDynamics href "../ProprietaryParameterDynamics"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [LoadDynamics](LoadDynamics.md)
        * **LoadUserDefined**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| proprietary | [cim:LoadUserDefined.proprietary](http://iec.ch/TC57/CIM100#LoadUserDefined.proprietary) | 1 <br />  boolean  | Behaviour is based on a proprietary model as opposed to a detailed model | direct |
| ProprietaryParameterDynamics | [cim:LoadUserDefined.ProprietaryParameterDynamics](http://iec.ch/TC57/CIM100#LoadUserDefined.ProprietaryParameterDynamics) | * <br />  [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md)  | Parameter of this proprietary user-defined model | direct |
| EnergyConsumer | [cim:LoadDynamics.EnergyConsumer](http://iec.ch/TC57/CIM100#LoadDynamics.EnergyConsumer) | * <br />  [EnergyConsumer](EnergyConsumer.md)  | Energy consumer to which this dynamics load model applies | [LoadDynamics](LoadDynamics.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ProprietaryParameterDynamics](ProprietaryParameterDynamics.md) | LoadUserDefined | range | [LoadUserDefined](LoadUserDefined.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:LoadUserDefined |
| native | this:LoadUserDefined |




