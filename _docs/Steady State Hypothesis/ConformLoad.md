# ConformLoad


_ConformLoad represent loads that follow a daily load change pattern where the pattern can be used to scale the load with a system load._





**URI**: [cim:ConformLoad](http://iec.ch/TC57/CIM100#ConformLoad)<br />
**Type**: Class




```mermaid
 classDiagram
    class ConformLoad
    click ConformLoad href "../ConformLoad"
      EnergyConsumer <|-- ConformLoad
        click EnergyConsumer href "../EnergyConsumer"
      
      ConformLoad : Equipment.inService
        
      ConformLoad : IdentifiedObject.mRID
        
      ConformLoad : EnergyConsumer.p
        
          ConformLoad --> ActivePower : EnergyConsumer.p
          click ActivePower href "../ActivePower"
        
      ConformLoad : EnergyConsumer.q
        
          ConformLoad --> ReactivePower : EnergyConsumer.q
          click ReactivePower href "../ReactivePower"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * [EnergyConsumer](EnergyConsumer.md)
                        * **ConformLoad**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| p | [cim:EnergyConsumer.p](http://iec.ch/TC57/CIM100#EnergyConsumer.p) | 1 <br />  [ActivePower](ActivePower.md)  | Active power of the load | [EnergyConsumer](EnergyConsumer.md) |
| q | [cim:EnergyConsumer.q](http://iec.ch/TC57/CIM100#EnergyConsumer.q) | 1 <br />  [ReactivePower](ReactivePower.md)  | Reactive power of the load | [EnergyConsumer](EnergyConsumer.md) |
| inService | [cim:Equipment.inService](http://iec.ch/TC57/CIM100#Equipment.inService) | 1 <br />  boolean  | Specifies the availability of the equipment | [Equipment](Equipment.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ConformLoad |
| native | this:ConformLoad |




