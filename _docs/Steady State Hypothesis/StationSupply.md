# StationSupply


_Station supply with load derived from the station output._





**URI**: [cim:StationSupply](http://iec.ch/TC57/CIM100#StationSupply)<br />
**Type**: Class




```mermaid
 classDiagram
    class StationSupply
      EnergyConsumer <|-- StationSupply
      
      StationSupply : Equipment.inService
        
      StationSupply : IdentifiedObject.mRID
        
      StationSupply : EnergyConsumer.p
        
          StationSupply --> ActivePower : EnergyConsumer.p
        
      StationSupply : EnergyConsumer.q
        
          StationSupply --> ReactivePower : EnergyConsumer.q
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * [EnergyConsumer](EnergyConsumer.md)
                        * **StationSupply**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| p | [cim:EnergyConsumer.p](http://iec.ch/TC57/CIM100#EnergyConsumer.p) | 1..1 <br />  [ActivePower](ActivePower.md)  | Active power of the load | [EnergyConsumer](EnergyConsumer.md) |
| q | [cim:EnergyConsumer.q](http://iec.ch/TC57/CIM100#EnergyConsumer.q) | 1..1 <br />  [ReactivePower](ReactivePower.md)  | Reactive power of the load | [EnergyConsumer](EnergyConsumer.md) |
| inService | [cim:Equipment.inService](http://iec.ch/TC57/CIM100#Equipment.inService) | 1..1 <br />  boolean  | Specifies the availability of the equipment | [Equipment](Equipment.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:StationSupply |
| native | this:StationSupply |




