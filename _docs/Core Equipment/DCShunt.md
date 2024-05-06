# DCShunt


_A shunt device within the DC system, typically used for filtering.  Needed for transient and short circuit studies._





**URI**: [cim:DCShunt](http://iec.ch/TC57/CIM100#DCShunt)<br />
**Type**: Class




```mermaid
 classDiagram
    class DCShunt
    click DCShunt href "../DCShunt"
      DCConductingEquipment <|-- DCShunt
        click DCConductingEquipment href "../DCConductingEquipment"
      
      DCShunt : Equipment.aggregate
        
      DCShunt : DCShunt.capacitance
        
          DCShunt --> Capacitance : DCShunt.capacitance
          click Capacitance href "../Capacitance"
        
      DCShunt : DCConductingEquipment.DCTerminals
        
          DCShunt --> DCTerminal : DCConductingEquipment.DCTerminals
          click DCTerminal href "../DCTerminal"
        
      DCShunt : IdentifiedObject.description
        
      DCShunt : IdentifiedObject.energyIdentCodeEic
        
      DCShunt : Equipment.EquipmentContainer
        
          DCShunt --> EquipmentContainer : Equipment.EquipmentContainer
          click EquipmentContainer href "../EquipmentContainer"
        
      DCShunt : IdentifiedObject.mRID
        
      DCShunt : IdentifiedObject.name
        
      DCShunt : Equipment.normallyInService
        
      DCShunt : Equipment.OperationalLimitSet
        
          DCShunt --> OperationalLimitSet : Equipment.OperationalLimitSet
          click OperationalLimitSet href "../OperationalLimitSet"
        
      DCShunt : DCConductingEquipment.ratedUdc
        
          DCShunt --> Voltage : DCConductingEquipment.ratedUdc
          click Voltage href "../Voltage"
        
      DCShunt : DCShunt.resistance
        
          DCShunt --> Resistance : DCShunt.resistance
          click Resistance href "../Resistance"
        
      DCShunt : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [DCConductingEquipment](DCConductingEquipment.md)
                * **DCShunt**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| capacitance | [cim:DCShunt.capacitance](http://iec.ch/TC57/CIM100#DCShunt.capacitance) | 1 <br />  [Capacitance](Capacitance.md)  | Capacitance of the DC shunt | direct |
| resistance | [cim:DCShunt.resistance](http://iec.ch/TC57/CIM100#DCShunt.resistance) | 1 <br />  [Resistance](Resistance.md)  | Resistance of the DC device | direct |
| ratedUdc | [cim:DCConductingEquipment.ratedUdc](http://iec.ch/TC57/CIM100#DCConductingEquipment.ratedUdc) | 1 <br />  [Voltage](Voltage.md)  | Rated DC device voltage | [DCConductingEquipment](DCConductingEquipment.md) |
| DCTerminals | [cim:DCConductingEquipment.DCTerminals](http://iec.ch/TC57/CIM100#DCConductingEquipment.DCTerminals) | * <br />  [DCTerminal](DCTerminal.md)  | A DC conducting equipment has DC terminals | [DCConductingEquipment](DCConductingEquipment.md) |
| aggregate | [cim:Equipment.aggregate](http://iec.ch/TC57/CIM100#Equipment.aggregate) | 0..1 <br />  boolean  | The aggregate flag provides an alternative way of representing an aggregated ... | [Equipment](Equipment.md) |
| normallyInService | [cim:Equipment.normallyInService](http://iec.ch/TC57/CIM100#Equipment.normallyInService) | 0..1 <br />  boolean  | Specifies the availability of the equipment under normal operating conditions | [Equipment](Equipment.md) |
| EquipmentContainer | [cim:Equipment.EquipmentContainer](http://iec.ch/TC57/CIM100#Equipment.EquipmentContainer) | 0..1 <br />  [EquipmentContainer](EquipmentContainer.md)  | Container of this equipment | [Equipment](Equipment.md) |
| OperationalLimitSet | [cim:Equipment.OperationalLimitSet](http://iec.ch/TC57/CIM100#Equipment.OperationalLimitSet) | * <br />  [OperationalLimitSet](OperationalLimitSet.md)  | The operational limit sets associated with this equipment | [Equipment](Equipment.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:DCShunt |
| native | this:DCShunt |




