# Conductor


_Combination of conducting material with consistent electrical characteristics, building a single electrical system, used to carry current between points in the power system._





**URI**: [cim:Conductor](http://iec.ch/TC57/CIM100#Conductor)<br />
**Type**: Class




```mermaid
 classDiagram
    class Conductor
    click Conductor href "../Conductor"
      ConductingEquipment <|-- Conductor
        click ConductingEquipment href "../ConductingEquipment"
      

      Conductor <|-- ACLineSegment
        click ACLineSegment href "../ACLineSegment"
      
      
      Conductor : IdentifiedObject.mRID
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * **Conductor**
                    * [ACLineSegment](ACLineSegment.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/ShortCircuit-EU#Package_ShortCircuitProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Conductor |
| native | this:Conductor |




