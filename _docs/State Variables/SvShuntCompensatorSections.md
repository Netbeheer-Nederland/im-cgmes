# SvShuntCompensatorSections


_State variable for the number of sections in service for a shunt compensator._





**URI**: [cim:SvShuntCompensatorSections](http://iec.ch/TC57/CIM100#SvShuntCompensatorSections)<br />
**Type**: Class




```mermaid
 classDiagram
    class SvShuntCompensatorSections
      SvShuntCompensatorSections : SvShuntCompensatorSections.sections
        
      SvShuntCompensatorSections : SvShuntCompensatorSections.ShuntCompensator
        
          SvShuntCompensatorSections --> ShuntCompensator : SvShuntCompensatorSections.ShuntCompensator
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ShuntCompensator | [cim:SvShuntCompensatorSections.ShuntCompensator](http://iec.ch/TC57/CIM100#SvShuntCompensatorSections.ShuntCompensator) | 1..1 <br />  [ShuntCompensator](ShuntCompensator.md)  | The shunt compensator for which the state applies | direct |
| sections | [cim:SvShuntCompensatorSections.sections](http://iec.ch/TC57/CIM100#SvShuntCompensatorSections.sections) | 1..1 <br />  float  | The number of sections in service as a continuous variable | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ShuntCompensator](ShuntCompensator.md) | SvShuntCompensatorSections | range | [SvShuntCompensatorSections](SvShuntCompensatorSections.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/StateVariables-EU#Package_StateVariablesProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:SvShuntCompensatorSections |
| native | this:SvShuntCompensatorSections |




