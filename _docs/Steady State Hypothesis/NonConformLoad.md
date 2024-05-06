# NonConformLoad


_NonConformLoad represents loads that do not follow a daily load change pattern and whose changes are not correlated with the daily load change pattern._





**URI**: [cim:NonConformLoad](http://iec.ch/TC57/CIM100#NonConformLoad)<br />
**Type**: Class




```mermaid
 classDiagram
    class NonConformLoad
    click NonConformLoad href "../NonConformLoad"
      EnergyConsumer <|-- NonConformLoad
        click EnergyConsumer href "../EnergyConsumer"
      
      NonConformLoad : Equipment.inService
        
      NonConformLoad : IdentifiedObject.mRID
        
      NonConformLoad : EnergyConsumer.p
        
          NonConformLoad --> ActivePower : EnergyConsumer.p
          click ActivePower href "../ActivePower"
        
      NonConformLoad : EnergyConsumer.q
        
          NonConformLoad --> ReactivePower : EnergyConsumer.q
          click ReactivePower href "../ReactivePower"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * [EnergyConsumer](EnergyConsumer.md)
                        * **NonConformLoad**



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
| self | cim:NonConformLoad |
| native | this:NonConformLoad |




