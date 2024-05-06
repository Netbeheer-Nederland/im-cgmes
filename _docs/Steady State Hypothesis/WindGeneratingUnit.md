# WindGeneratingUnit


_A wind driven generating unit, connected to the grid by means of a rotating machine.  May be used to represent a single turbine or an aggregation._





**URI**: [cim:WindGeneratingUnit](http://iec.ch/TC57/CIM100#WindGeneratingUnit)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindGeneratingUnit
    click WindGeneratingUnit href "../WindGeneratingUnit"
      GeneratingUnit <|-- WindGeneratingUnit
        click GeneratingUnit href "../GeneratingUnit"
      
      WindGeneratingUnit : Equipment.inService
        
      WindGeneratingUnit : IdentifiedObject.mRID
        
      WindGeneratingUnit : GeneratingUnit.normalPF
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [GeneratingUnit](GeneratingUnit.md)
                * **WindGeneratingUnit**



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
| self | cim:WindGeneratingUnit |
| native | this:WindGeneratingUnit |




