# ConductingEquipment


_The parts of the AC power system that are designed to carry current or that are conductively connected through terminals._





**URI**: [cim:ConductingEquipment](http://iec.ch/TC57/CIM100#ConductingEquipment)<br />
**Type**: Class




```mermaid
 classDiagram
    class ConductingEquipment
      Equipment <|-- ConductingEquipment
      

      ConductingEquipment <|-- Conductor
      ConductingEquipment <|-- Connector
      ConductingEquipment <|-- EarthFaultCompensator
      ConductingEquipment <|-- EnergyConnection
      ConductingEquipment <|-- EquivalentEquipment
      ConductingEquipment <|-- PowerTransformer
      ConductingEquipment <|-- SeriesCompensator
      
      
      ConductingEquipment : IdentifiedObject.mRID
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * **ConductingEquipment**
                * [Conductor](Conductor.md)
                * [Connector](Connector.md)
                * [EarthFaultCompensator](EarthFaultCompensator.md)
                * [EnergyConnection](EnergyConnection.md)
                * [EquivalentEquipment](EquivalentEquipment.md)
                * [PowerTransformer](PowerTransformer.md)
                * [SeriesCompensator](SeriesCompensator.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/ShortCircuit-EU#Package_ShortCircuitProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ConductingEquipment |
| native | this:ConductingEquipment |




