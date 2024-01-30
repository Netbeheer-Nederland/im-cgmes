# ACDCTerminal


_An electrical connection point (AC or DC) to a piece of conducting equipment. Terminals are connected at physical connection points called connectivity nodes._





**URI**: [cim:ACDCTerminal](http://iec.ch/TC57/CIM100#ACDCTerminal)<br />
**Type**: Class




```mermaid
 classDiagram
    class ACDCTerminal
      IdentifiedObject <|-- ACDCTerminal
      

      ACDCTerminal <|-- Terminal
      
      
      ACDCTerminal : IdentifiedObject.description
        
      ACDCTerminal : ACDCTerminal.Measurements
        
          ACDCTerminal --> Measurement : ACDCTerminal.Measurements
        
      ACDCTerminal : IdentifiedObject.mRID
        
      ACDCTerminal : IdentifiedObject.name
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **ACDCTerminal**
        * [Terminal](Terminal.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| Measurements | [cim:ACDCTerminal.Measurements](http://iec.ch/TC57/CIM100#ACDCTerminal.Measurements) | 0..* <br />  [Measurement](Measurement.md)  | Measurements associated with this terminal defining  where the measurement is... | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [Accumulator](Accumulator.md) | Terminal | range | [ACDCTerminal](ACDCTerminal.md) |
| [Analog](Analog.md) | Terminal | range | [ACDCTerminal](ACDCTerminal.md) |
| [Discrete](Discrete.md) | Terminal | range | [ACDCTerminal](ACDCTerminal.md) |
| [Measurement](Measurement.md) | Terminal | range | [ACDCTerminal](ACDCTerminal.md) |
| [StringMeasurement](StringMeasurement.md) | Terminal | range | [ACDCTerminal](ACDCTerminal.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ACDCTerminal |
| native | this:ACDCTerminal |




