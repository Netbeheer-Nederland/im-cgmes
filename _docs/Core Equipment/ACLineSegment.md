# ACLineSegment


_A wire or combination of wires, with consistent electrical characteristics, building a single electrical system, used to carry alternating current between points in the power system._

_For symmetrical, transposed three phase lines, it is sufficient to use attributes of the line segment, which describe impedances and admittances for the entire length of the segment.  Additionally impedances can be computed by using length and associated per length impedances._

_The BaseVoltage at the two ends of ACLineSegments in a Line shall have the same BaseVoltage.nominalVoltage. However, boundary lines may have slightly different BaseVoltage.nominalVoltages and variation is allowed. Larger voltage difference in general requires use of an equivalent branch._





**URI**: [cim:ACLineSegment](http://iec.ch/TC57/CIM100#ACLineSegment)<br />
**Type**: Class




```mermaid
 classDiagram
    class ACLineSegment
      Conductor <|-- ACLineSegment
      
      ACLineSegment : Equipment.aggregate
        
      ACLineSegment : ConductingEquipment.BaseVoltage
        
          ACLineSegment --> BaseVoltage : ConductingEquipment.BaseVoltage
        
      ACLineSegment : ACLineSegment.bch
        
          ACLineSegment --> Susceptance : ACLineSegment.bch
        
      ACLineSegment : ACLineSegment.Clamp
        
          ACLineSegment --> Clamp : ACLineSegment.Clamp
        
      ACLineSegment : ACLineSegment.Cut
        
          ACLineSegment --> Cut : ACLineSegment.Cut
        
      ACLineSegment : IdentifiedObject.description
        
      ACLineSegment : IdentifiedObject.energyIdentCodeEic
        
      ACLineSegment : Equipment.EquipmentContainer
        
          ACLineSegment --> EquipmentContainer : Equipment.EquipmentContainer
        
      ACLineSegment : ACLineSegment.gch
        
          ACLineSegment --> Conductance : ACLineSegment.gch
        
      ACLineSegment : Conductor.length
        
          ACLineSegment --> Length : Conductor.length
        
      ACLineSegment : IdentifiedObject.mRID
        
      ACLineSegment : IdentifiedObject.name
        
      ACLineSegment : Equipment.normallyInService
        
      ACLineSegment : Equipment.OperationalLimitSet
        
          ACLineSegment --> OperationalLimitSet : Equipment.OperationalLimitSet
        
      ACLineSegment : ACLineSegment.r
        
          ACLineSegment --> Resistance : ACLineSegment.r
        
      ACLineSegment : IdentifiedObject.shortName
        
      ACLineSegment : ConductingEquipment.Terminals
        
          ACLineSegment --> Terminal : ConductingEquipment.Terminals
        
      ACLineSegment : ACLineSegment.x
        
          ACLineSegment --> Reactance : ACLineSegment.x
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [Conductor](Conductor.md)
                    * **ACLineSegment**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| bch | [cim:ACLineSegment.bch](http://iec.ch/TC57/CIM100#ACLineSegment.bch) | 1..1 <br />  [Susceptance](Susceptance.md)  | Positive sequence shunt (charging) susceptance, uniformly distributed, of the... | direct |
| gch | [cim:ACLineSegment.gch](http://iec.ch/TC57/CIM100#ACLineSegment.gch) | 0..1 <br />  [Conductance](Conductance.md)  | Positive sequence shunt (charging) conductance, uniformly distributed, of the... | direct |
| r | [cim:ACLineSegment.r](http://iec.ch/TC57/CIM100#ACLineSegment.r) | 1..1 <br />  [Resistance](Resistance.md)  | Positive sequence series resistance of the entire line section | direct |
| x | [cim:ACLineSegment.x](http://iec.ch/TC57/CIM100#ACLineSegment.x) | 1..1 <br />  [Reactance](Reactance.md)  | Positive sequence series reactance of the entire line section | direct |
| Clamp | [cim:ACLineSegment.Clamp](http://iec.ch/TC57/CIM100#ACLineSegment.Clamp) | 0..* <br />  [Clamp](Clamp.md)  | The clamps connected to the line segment | direct |
| Cut | [cim:ACLineSegment.Cut](http://iec.ch/TC57/CIM100#ACLineSegment.Cut) | 0..* <br />  [Cut](Cut.md)  | Cuts applied to the line segment | direct |
| length | [cim:Conductor.length](http://iec.ch/TC57/CIM100#Conductor.length) | 0..1 <br />  [Length](Length.md)  | Segment length for calculating line section capabilities | [Conductor](Conductor.md) |
| BaseVoltage | [cim:ConductingEquipment.BaseVoltage](http://iec.ch/TC57/CIM100#ConductingEquipment.BaseVoltage) | 0..1 <br />  [BaseVoltage](BaseVoltage.md)  | Base voltage of this conducting equipment | [ConductingEquipment](ConductingEquipment.md) |
| Terminals | [cim:ConductingEquipment.Terminals](http://iec.ch/TC57/CIM100#ConductingEquipment.Terminals) | 0..* <br />  [Terminal](Terminal.md)  | Conducting equipment have terminals that may be connected to other conducting... | [ConductingEquipment](ConductingEquipment.md) |
| aggregate | [cim:Equipment.aggregate](http://iec.ch/TC57/CIM100#Equipment.aggregate) | 0..1 <br />  boolean  | The aggregate flag provides an alternative way of representing an aggregated ... | [Equipment](Equipment.md) |
| normallyInService | [cim:Equipment.normallyInService](http://iec.ch/TC57/CIM100#Equipment.normallyInService) | 0..1 <br />  boolean  | Specifies the availability of the equipment under normal operating conditions | [Equipment](Equipment.md) |
| EquipmentContainer | [cim:Equipment.EquipmentContainer](http://iec.ch/TC57/CIM100#Equipment.EquipmentContainer) | 0..1 <br />  [EquipmentContainer](EquipmentContainer.md)  | Container of this equipment | [Equipment](Equipment.md) |
| OperationalLimitSet | [cim:Equipment.OperationalLimitSet](http://iec.ch/TC57/CIM100#Equipment.OperationalLimitSet) | 0..* <br />  [OperationalLimitSet](OperationalLimitSet.md)  | The operational limit sets associated with this equipment | [Equipment](Equipment.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [Clamp](Clamp.md) | ACLineSegment | range | [ACLineSegment](ACLineSegment.md) |
| [Cut](Cut.md) | ACLineSegment | range | [ACLineSegment](ACLineSegment.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ACLineSegment |
| native | this:ACLineSegment |




