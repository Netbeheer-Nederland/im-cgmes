# EarthFaultCompensator


_A conducting equipment used to represent a connection to ground which is typically used to compensate earth faults.   An earth fault compensator device modelled with a single terminal implies a second terminal solidly connected to ground.  If two terminals are modelled, the ground is not assumed and normal connection rules apply._





**URI**: [cim:EarthFaultCompensator](http://iec.ch/TC57/CIM100#EarthFaultCompensator)<br />
**Type**: Class




```mermaid
 classDiagram
    class EarthFaultCompensator
      ConductingEquipment <|-- EarthFaultCompensator
      

      EarthFaultCompensator <|-- GroundingImpedance
      EarthFaultCompensator <|-- PetersenCoil
      
      
      EarthFaultCompensator : Equipment.aggregate
        
      EarthFaultCompensator : ConductingEquipment.BaseVoltage
        
          EarthFaultCompensator --> BaseVoltage : ConductingEquipment.BaseVoltage
        
      EarthFaultCompensator : IdentifiedObject.description
        
      EarthFaultCompensator : IdentifiedObject.energyIdentCodeEic
        
      EarthFaultCompensator : Equipment.EquipmentContainer
        
          EarthFaultCompensator --> EquipmentContainer : Equipment.EquipmentContainer
        
      EarthFaultCompensator : IdentifiedObject.mRID
        
      EarthFaultCompensator : IdentifiedObject.name
        
      EarthFaultCompensator : Equipment.normallyInService
        
      EarthFaultCompensator : Equipment.OperationalLimitSet
        
          EarthFaultCompensator --> OperationalLimitSet : Equipment.OperationalLimitSet
        
      EarthFaultCompensator : IdentifiedObject.shortName
        
      EarthFaultCompensator : ConductingEquipment.Terminals
        
          EarthFaultCompensator --> Terminal : ConductingEquipment.Terminals
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * **EarthFaultCompensator**
                    * [GroundingImpedance](GroundingImpedance.md)
                    * [PetersenCoil](PetersenCoil.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
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









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:EarthFaultCompensator |
| native | this:EarthFaultCompensator |




