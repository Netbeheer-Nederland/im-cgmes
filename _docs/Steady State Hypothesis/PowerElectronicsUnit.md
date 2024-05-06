# PowerElectronicsUnit


_A generating unit or battery or aggregation that connects to the AC network using power electronics rather than rotating machines._





**URI**: [cim:PowerElectronicsUnit](http://iec.ch/TC57/CIM100#PowerElectronicsUnit)<br />
**Type**: Class




```mermaid
 classDiagram
    class PowerElectronicsUnit
    click PowerElectronicsUnit href "../PowerElectronicsUnit"
      Equipment <|-- PowerElectronicsUnit
        click Equipment href "../Equipment"
      

      PowerElectronicsUnit <|-- BatteryUnit
        click BatteryUnit href "../BatteryUnit"
      
      
      PowerElectronicsUnit : Equipment.inService
        
      PowerElectronicsUnit : IdentifiedObject.mRID
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * **PowerElectronicsUnit**
                * [BatteryUnit](BatteryUnit.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| inService | [cim:Equipment.inService](http://iec.ch/TC57/CIM100#Equipment.inService) | 1 <br />  boolean  | Specifies the availability of the equipment | [Equipment](Equipment.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:PowerElectronicsUnit |
| native | this:PowerElectronicsUnit |




