# NuclearGeneratingUnit


_A nuclear generating unit._





**URI**: [cim:NuclearGeneratingUnit](http://iec.ch/TC57/CIM100#NuclearGeneratingUnit)<br />
**Type**: Class




```mermaid
 classDiagram
    class NuclearGeneratingUnit
    click NuclearGeneratingUnit href "../NuclearGeneratingUnit"
      GeneratingUnit <|-- NuclearGeneratingUnit
        click GeneratingUnit href "../GeneratingUnit"
      
      NuclearGeneratingUnit : Equipment.inService
        
      NuclearGeneratingUnit : IdentifiedObject.mRID
        
      NuclearGeneratingUnit : GeneratingUnit.normalPF
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [GeneratingUnit](GeneratingUnit.md)
                * **NuclearGeneratingUnit**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| normalPF | [cim:GeneratingUnit.normalPF](http://iec.ch/TC57/CIM100#GeneratingUnit.normalPF) | 1 <br />  float  | Generating unit economic participation factor | [GeneratingUnit](GeneratingUnit.md) |
| inService | [cim:Equipment.inService](http://iec.ch/TC57/CIM100#Equipment.inService) | 1 <br />  boolean  | Specifies the availability of the equipment | [Equipment](Equipment.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:NuclearGeneratingUnit |
| native | this:NuclearGeneratingUnit |




