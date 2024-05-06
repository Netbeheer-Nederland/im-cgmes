# Cut


_A cut separates a line segment into two parts. The cut appears as a switch inserted between these two parts and connects them together. As the cut is normally open there is no galvanic connection between the two line segment parts. But it is possible to close the cut to get galvanic connection._

_The cut terminals are oriented towards the line segment terminals with the same sequence number. Hence the cut terminal with sequence number equal to 1 is oriented to the line segment's terminal with sequence number equal to 1._

_The cut terminals also act as connection points for jumpers and other equipment, e.g. a mobile generator. To enable this, connectivity nodes are placed at the cut terminals. Once the connectivity nodes are in place any conducting equipment can be connected at them._





**URI**: [cim:Cut](http://iec.ch/TC57/CIM100#Cut)<br />
**Type**: Class




```mermaid
 classDiagram
    class Cut
    click Cut href "../Cut"
      Switch <|-- Cut
        click Switch href "../Switch"
      
      Cut : Cut.ACLineSegment
        
          Cut --> ACLineSegment : Cut.ACLineSegment
          click ACLineSegment href "../ACLineSegment"
        
      Cut : Equipment.aggregate
        
      Cut : ConductingEquipment.BaseVoltage
        
          Cut --> BaseVoltage : ConductingEquipment.BaseVoltage
          click BaseVoltage href "../BaseVoltage"
        
      Cut : IdentifiedObject.description
        
      Cut : IdentifiedObject.energyIdentCodeEic
        
      Cut : Equipment.EquipmentContainer
        
          Cut --> EquipmentContainer : Equipment.EquipmentContainer
          click EquipmentContainer href "../EquipmentContainer"
        
      Cut : Cut.lengthFromTerminal1
        
          Cut --> Length : Cut.lengthFromTerminal1
          click Length href "../Length"
        
      Cut : IdentifiedObject.mRID
        
      Cut : IdentifiedObject.name
        
      Cut : Equipment.normallyInService
        
      Cut : Switch.normalOpen
        
      Cut : Equipment.OperationalLimitSet
        
          Cut --> OperationalLimitSet : Equipment.OperationalLimitSet
          click OperationalLimitSet href "../OperationalLimitSet"
        
      Cut : Switch.ratedCurrent
        
          Cut --> CurrentFlow : Switch.ratedCurrent
          click CurrentFlow href "../CurrentFlow"
        
      Cut : Switch.retained
        
      Cut : IdentifiedObject.shortName
        
      Cut : Switch.SwitchSchedules
        
          Cut --> SwitchSchedule : Switch.SwitchSchedules
          click SwitchSchedule href "../SwitchSchedule"
        
      Cut : ConductingEquipment.Terminals
        
          Cut --> Terminal : ConductingEquipment.Terminals
          click Terminal href "../Terminal"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [Switch](Switch.md)
                    * **Cut**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ACLineSegment | [cim:Cut.ACLineSegment](http://iec.ch/TC57/CIM100#Cut.ACLineSegment) | 1 <br />  [ACLineSegment](ACLineSegment.md)  | The line segment to which the cut is applied | direct |
| lengthFromTerminal1 | [cim:Cut.lengthFromTerminal1](http://iec.ch/TC57/CIM100#Cut.lengthFromTerminal1) | 0..1 <br />  [Length](Length.md)  | The length to the place where the cut is located starting from side one of th... | direct |
| normalOpen | [cim:Switch.normalOpen](http://iec.ch/TC57/CIM100#Switch.normalOpen) | 1 <br />  boolean  | The attribute is used in cases when no Measurement for the status value is pr... | [Switch](Switch.md) |
| ratedCurrent | [cim:Switch.ratedCurrent](http://iec.ch/TC57/CIM100#Switch.ratedCurrent) | 0..1 <br />  [CurrentFlow](CurrentFlow.md)  | The maximum continuous current carrying capacity in amps governed by the devi... | [Switch](Switch.md) |
| retained | [cim:Switch.retained](http://iec.ch/TC57/CIM100#Switch.retained) | 1 <br />  boolean  | Branch is retained in the topological solution | [Switch](Switch.md) |
| SwitchSchedules | [cim:Switch.SwitchSchedules](http://iec.ch/TC57/CIM100#Switch.SwitchSchedules) | * <br />  [SwitchSchedule](SwitchSchedule.md)  | A Switch can be associated with SwitchSchedules | [Switch](Switch.md) |
| BaseVoltage | [cim:ConductingEquipment.BaseVoltage](http://iec.ch/TC57/CIM100#ConductingEquipment.BaseVoltage) | 0..1 <br />  [BaseVoltage](BaseVoltage.md)  | Base voltage of this conducting equipment | [ConductingEquipment](ConductingEquipment.md) |
| Terminals | [cim:ConductingEquipment.Terminals](http://iec.ch/TC57/CIM100#ConductingEquipment.Terminals) | * <br />  [Terminal](Terminal.md)  | Conducting equipment have terminals that may be connected to other conducting... | [ConductingEquipment](ConductingEquipment.md) |
| aggregate | [cim:Equipment.aggregate](http://iec.ch/TC57/CIM100#Equipment.aggregate) | 0..1 <br />  boolean  | The aggregate flag provides an alternative way of representing an aggregated ... | [Equipment](Equipment.md) |
| normallyInService | [cim:Equipment.normallyInService](http://iec.ch/TC57/CIM100#Equipment.normallyInService) | 0..1 <br />  boolean  | Specifies the availability of the equipment under normal operating conditions | [Equipment](Equipment.md) |
| EquipmentContainer | [cim:Equipment.EquipmentContainer](http://iec.ch/TC57/CIM100#Equipment.EquipmentContainer) | 0..1 <br />  [EquipmentContainer](EquipmentContainer.md)  | Container of this equipment | [Equipment](Equipment.md) |
| OperationalLimitSet | [cim:Equipment.OperationalLimitSet](http://iec.ch/TC57/CIM100#Equipment.OperationalLimitSet) | * <br />  [OperationalLimitSet](OperationalLimitSet.md)  | The operational limit sets associated with this equipment | [Equipment](Equipment.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ACLineSegment](ACLineSegment.md) | Cut | range | [Cut](Cut.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Cut |
| native | this:Cut |




