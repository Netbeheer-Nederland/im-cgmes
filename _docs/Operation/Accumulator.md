# Accumulator


_Accumulator represents an accumulated (counted) Measurement, e.g. an energy value._





**URI**: [cim:Accumulator](http://iec.ch/TC57/CIM100#Accumulator)<br />
**Type**: Class




```mermaid
 classDiagram
    class Accumulator
      Measurement <|-- Accumulator
      
      Accumulator : Accumulator.AccumulatorValues
        
          Accumulator --> AccumulatorValue : Accumulator.AccumulatorValues
        
      Accumulator : IdentifiedObject.description
        
      Accumulator : Accumulator.LimitSets
        
          Accumulator --> AccumulatorLimitSet : Accumulator.LimitSets
        
      Accumulator : Measurement.measurementType
        
      Accumulator : IdentifiedObject.mRID
        
      Accumulator : IdentifiedObject.name
        
      Accumulator : Measurement.phases
        
          Accumulator --> PhaseCode : Measurement.phases
        
      Accumulator : Measurement.PowerSystemResource
        
          Accumulator --> PowerSystemResource : Measurement.PowerSystemResource
        
      Accumulator : Measurement.Terminal
        
          Accumulator --> ACDCTerminal : Measurement.Terminal
        
      Accumulator : Measurement.unitMultiplier
        
          Accumulator --> UnitMultiplier : Measurement.unitMultiplier
        
      Accumulator : Measurement.unitSymbol
        
          Accumulator --> UnitSymbol : Measurement.unitSymbol
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [Measurement](Measurement.md)
        * **Accumulator**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| AccumulatorValues | [cim:Accumulator.AccumulatorValues](http://iec.ch/TC57/CIM100#Accumulator.AccumulatorValues) | 0..* <br />  [AccumulatorValue](AccumulatorValue.md)  | The values connected to this measurement | direct |
| LimitSets | [cim:Accumulator.LimitSets](http://iec.ch/TC57/CIM100#Accumulator.LimitSets) | 0..* <br />  [AccumulatorLimitSet](AccumulatorLimitSet.md)  | A measurement may have zero or more limit ranges defined for it | direct |
| Terminal | [cim:Measurement.Terminal](http://iec.ch/TC57/CIM100#Measurement.Terminal) | 0..1 <br />  [ACDCTerminal](ACDCTerminal.md)  | One or more measurements may be associated with a terminal in the network | [Measurement](Measurement.md) |
| measurementType | [cim:Measurement.measurementType](http://iec.ch/TC57/CIM100#Measurement.measurementType) | 1..1 <br />  string  | Specifies the type of measurement | [Measurement](Measurement.md) |
| phases | [cim:Measurement.phases](http://iec.ch/TC57/CIM100#Measurement.phases) | 0..1 <br />  [PhaseCode](PhaseCode.md)  | Indicates to which phases the measurement applies and avoids the need to use ... | [Measurement](Measurement.md) |
| unitMultiplier | [cim:Measurement.unitMultiplier](http://iec.ch/TC57/CIM100#Measurement.unitMultiplier) | 1..1 <br />  [UnitMultiplier](UnitMultiplier.md)  | The unit multiplier of the measured quantity | [Measurement](Measurement.md) |
| unitSymbol | [cim:Measurement.unitSymbol](http://iec.ch/TC57/CIM100#Measurement.unitSymbol) | 1..1 <br />  [UnitSymbol](UnitSymbol.md)  | The unit of measure of the measured quantity | [Measurement](Measurement.md) |
| PowerSystemResource | [cim:Measurement.PowerSystemResource](http://iec.ch/TC57/CIM100#Measurement.PowerSystemResource) | 1..1 <br />  [PowerSystemResource](PowerSystemResource.md)  | The power system resource that contains the measurement | [Measurement](Measurement.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [AccumulatorLimitSet](AccumulatorLimitSet.md) | Measurements | range | [Accumulator](Accumulator.md) |
| [AccumulatorValue](AccumulatorValue.md) | Accumulator | range | [Accumulator](Accumulator.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Accumulator |
| native | this:Accumulator |




