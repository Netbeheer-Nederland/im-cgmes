# LoadAggregate


_Aggregate loads are used to represent all or part of the real and reactive load from one or more loads in the static (power flow) data. This load is usually the aggregation of many individual load devices and the load model is an approximate representation of the aggregate response of the load devices to system disturbances._

_Standard aggregate load model comprised of static and/or dynamic components.  A static load model represents the sensitivity of the real and reactive power consumed by the load to the amplitude and frequency of the bus voltage. A dynamic load model can be used to represent the aggregate response of the motor components of the load._





**URI**: [cim:LoadAggregate](http://iec.ch/TC57/CIM100#LoadAggregate)<br />
**Type**: Class




```mermaid
 classDiagram
    class LoadAggregate
      LoadDynamics <|-- LoadAggregate
      
      LoadAggregate : IdentifiedObject.description
        
      LoadAggregate : LoadDynamics.EnergyConsumer
        
          LoadAggregate --> EnergyConsumer : LoadDynamics.EnergyConsumer
        
      LoadAggregate : LoadAggregate.LoadMotor
        
          LoadAggregate --> LoadMotor : LoadAggregate.LoadMotor
        
      LoadAggregate : LoadAggregate.LoadStatic
        
          LoadAggregate --> LoadStatic : LoadAggregate.LoadStatic
        
      LoadAggregate : IdentifiedObject.mRID
        
      LoadAggregate : IdentifiedObject.name
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [LoadDynamics](LoadDynamics.md)
        * **LoadAggregate**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| LoadMotor | [cim:LoadAggregate.LoadMotor](http://iec.ch/TC57/CIM100#LoadAggregate.LoadMotor) | 0..1 <br />  [LoadMotor](LoadMotor.md)  | Aggregate motor (dynamic) load associated with this aggregate load | direct |
| LoadStatic | [cim:LoadAggregate.LoadStatic](http://iec.ch/TC57/CIM100#LoadAggregate.LoadStatic) | 0..1 <br />  [LoadStatic](LoadStatic.md)  | Aggregate static load associated with this aggregate load | direct |
| EnergyConsumer | [cim:LoadDynamics.EnergyConsumer](http://iec.ch/TC57/CIM100#LoadDynamics.EnergyConsumer) | 0..* <br />  [EnergyConsumer](EnergyConsumer.md)  | Energy consumer to which this dynamics load model applies | [LoadDynamics](LoadDynamics.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [LoadStatic](LoadStatic.md) | LoadAggregate | range | [LoadAggregate](LoadAggregate.md) |
| [LoadMotor](LoadMotor.md) | LoadAggregate | range | [LoadAggregate](LoadAggregate.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:LoadAggregate |
| native | this:LoadAggregate |




