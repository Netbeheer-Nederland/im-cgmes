# Equipment


_The parts of a power system that are physical devices, electronic or mechanical._





**URI**: [cim:Equipment](http://iec.ch/TC57/CIM100#Equipment)<br />
**Type**: Class




```mermaid
 classDiagram
    class Equipment
    click Equipment href "../Equipment"
      PowerSystemResource <|-- Equipment
        click PowerSystemResource href "../PowerSystemResource"
      

      Equipment <|-- ConductingEquipment
        click ConductingEquipment href "../ConductingEquipment"
      Equipment <|-- GeneratingUnit
        click GeneratingUnit href "../GeneratingUnit"
      Equipment <|-- PowerElectronicsUnit
        click PowerElectronicsUnit href "../PowerElectronicsUnit"
      
      
      Equipment : Equipment.inService
        
      Equipment : IdentifiedObject.mRID
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * **Equipment**
            * [ConductingEquipment](ConductingEquipment.md)
            * [GeneratingUnit](GeneratingUnit.md)
            * [PowerElectronicsUnit](PowerElectronicsUnit.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| inService | [cim:Equipment.inService](http://iec.ch/TC57/CIM100#Equipment.inService) | 1 <br />  boolean  | Specifies the availability of the equipment | direct |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Equipment |
| native | this:Equipment |




