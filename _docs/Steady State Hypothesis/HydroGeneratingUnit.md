# HydroGeneratingUnit


_A generating unit whose prime mover is a hydraulic turbine (e.g., Francis, Pelton, Kaplan)._





**URI**: [cim:HydroGeneratingUnit](http://iec.ch/TC57/CIM100#HydroGeneratingUnit)<br />
**Type**: Class




```mermaid
 classDiagram
    class HydroGeneratingUnit
    click HydroGeneratingUnit href "../HydroGeneratingUnit"
      GeneratingUnit <|-- HydroGeneratingUnit
        click GeneratingUnit href "../GeneratingUnit"
      
      HydroGeneratingUnit : Equipment.inService
        
      HydroGeneratingUnit : IdentifiedObject.mRID
        
      HydroGeneratingUnit : GeneratingUnit.normalPF
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [GeneratingUnit](GeneratingUnit.md)
                * **HydroGeneratingUnit**



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
| self | cim:HydroGeneratingUnit |
| native | this:HydroGeneratingUnit |




