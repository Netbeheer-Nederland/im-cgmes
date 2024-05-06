# LoadDynamics


_Load whose behaviour is described by reference to a standard model <font color="#0f0f0f">or by definition of a user-defined model.</font>_

_A standard feature of dynamic load behaviour modelling is the ability to associate the same behaviour to multiple energy consumers by means of a single load definition.  The load model is always applied to individual bus loads (energy consumers)._





**URI**: [cim:LoadDynamics](http://iec.ch/TC57/CIM100#LoadDynamics)<br />
**Type**: Class




```mermaid
 classDiagram
    class LoadDynamics
    click LoadDynamics href "../LoadDynamics"
      IdentifiedObject <|-- LoadDynamics
        click IdentifiedObject href "../IdentifiedObject"
      

      LoadDynamics <|-- LoadUserDefined
        click LoadUserDefined href "../LoadUserDefined"
      LoadDynamics <|-- LoadComposite
        click LoadComposite href "../LoadComposite"
      LoadDynamics <|-- LoadGenericNonLinear
        click LoadGenericNonLinear href "../LoadGenericNonLinear"
      LoadDynamics <|-- LoadAggregate
        click LoadAggregate href "../LoadAggregate"
      
      
      LoadDynamics : IdentifiedObject.description
        
      LoadDynamics : LoadDynamics.EnergyConsumer
        
          LoadDynamics --> EnergyConsumer : LoadDynamics.EnergyConsumer
          click EnergyConsumer href "../EnergyConsumer"
        
      LoadDynamics : IdentifiedObject.mRID
        
      LoadDynamics : IdentifiedObject.name
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **LoadDynamics**
        * [LoadUserDefined](LoadUserDefined.md)
        * [LoadComposite](LoadComposite.md)
        * [LoadGenericNonLinear](LoadGenericNonLinear.md)
        * [LoadAggregate](LoadAggregate.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| EnergyConsumer | [cim:LoadDynamics.EnergyConsumer](http://iec.ch/TC57/CIM100#LoadDynamics.EnergyConsumer) | * <br />  [EnergyConsumer](EnergyConsumer.md)  | Energy consumer to which this dynamics load model applies | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [EnergyConsumer](EnergyConsumer.md) | LoadDynamics | range | [LoadDynamics](LoadDynamics.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:LoadDynamics |
| native | this:LoadDynamics |




