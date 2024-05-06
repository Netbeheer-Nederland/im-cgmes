# Measurement


_A Measurement represents any measured, calculated or non-measured non-calculated quantity. Any piece of equipment may contain Measurements, e.g. a substation may have temperature measurements and door open indications, a transformer may have oil temperature and tank pressure measurements, a bay may contain a number of power flow measurements and a Breaker may contain a switch status measurement. _

_The PSR - Measurement association is intended to capture this use of Measurement and is included in the naming hierarchy based on EquipmentContainer. The naming hierarchy typically has Measurements as leaves, e.g. Substation-VoltageLevel-Bay-Switch-Measurement._

_Some Measurements represent quantities related to a particular sensor location in the network, e.g. a voltage transformer (VT) or potential transformer (PT) at a busbar or a current transformer (CT) at the bar between a breaker and an isolator. The sensing position is not captured in the PSR - Measurement association. Instead it is captured by the Measurement - Terminal association that is used to define the sensing location in the network topology. The location is defined by the connection of the Terminal to ConductingEquipment. _

_If both a Terminal and PSR are associated, and the PSR is of type ConductingEquipment, the associated Terminal should belong to that ConductingEquipment instance._

_When the sensor location is needed both Measurement-PSR and Measurement-Terminal are used. The Measurement-Terminal association is never used alone._





**URI**: [cim:Measurement](http://iec.ch/TC57/CIM100#Measurement)<br />
**Type**: Class




```mermaid
 classDiagram
    class Measurement
    click Measurement href "../Measurement"
      IdentifiedObject <|-- Measurement
        click IdentifiedObject href "../IdentifiedObject"
      

      Measurement <|-- Accumulator
        click Accumulator href "../Accumulator"
      Measurement <|-- Analog
        click Analog href "../Analog"
      Measurement <|-- Discrete
        click Discrete href "../Discrete"
      Measurement <|-- StringMeasurement
        click StringMeasurement href "../StringMeasurement"
      
      
      Measurement : IdentifiedObject.description
        
      Measurement : Measurement.measurementType
        
      Measurement : IdentifiedObject.mRID
        
      Measurement : IdentifiedObject.name
        
      Measurement : Measurement.phases
        
          Measurement --> PhaseCode : Measurement.phases
          click PhaseCode href "../PhaseCode"
        
      Measurement : Measurement.PowerSystemResource
        
          Measurement --> PowerSystemResource : Measurement.PowerSystemResource
          click PowerSystemResource href "../PowerSystemResource"
        
      Measurement : Measurement.Terminal
        
          Measurement --> ACDCTerminal : Measurement.Terminal
          click ACDCTerminal href "../ACDCTerminal"
        
      Measurement : Measurement.unitMultiplier
        
          Measurement --> UnitMultiplier : Measurement.unitMultiplier
          click UnitMultiplier href "../UnitMultiplier"
        
      Measurement : Measurement.unitSymbol
        
          Measurement --> UnitSymbol : Measurement.unitSymbol
          click UnitSymbol href "../UnitSymbol"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **Measurement**
        * [Accumulator](Accumulator.md)
        * [Analog](Analog.md)
        * [Discrete](Discrete.md)
        * [StringMeasurement](StringMeasurement.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| Terminal | [cim:Measurement.Terminal](http://iec.ch/TC57/CIM100#Measurement.Terminal) | 0..1 <br />  [ACDCTerminal](ACDCTerminal.md)  | One or more measurements may be associated with a terminal in the network | direct |
| measurementType | [cim:Measurement.measurementType](http://iec.ch/TC57/CIM100#Measurement.measurementType) | 1 <br />  string  | Specifies the type of measurement | direct |
| phases | [cim:Measurement.phases](http://iec.ch/TC57/CIM100#Measurement.phases) | 0..1 <br />  [PhaseCode](PhaseCode.md)  | Indicates to which phases the measurement applies and avoids the need to use ... | direct |
| unitMultiplier | [cim:Measurement.unitMultiplier](http://iec.ch/TC57/CIM100#Measurement.unitMultiplier) | 1 <br />  [UnitMultiplier](UnitMultiplier.md)  | The unit multiplier of the measured quantity | direct |
| unitSymbol | [cim:Measurement.unitSymbol](http://iec.ch/TC57/CIM100#Measurement.unitSymbol) | 1 <br />  [UnitSymbol](UnitSymbol.md)  | The unit of measure of the measured quantity | direct |
| PowerSystemResource | [cim:Measurement.PowerSystemResource](http://iec.ch/TC57/CIM100#Measurement.PowerSystemResource) | 1 <br />  [PowerSystemResource](PowerSystemResource.md)  | The power system resource that contains the measurement | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ACDCTerminal](ACDCTerminal.md) | Measurements | range | [Measurement](Measurement.md) |
| [PowerSystemResource](PowerSystemResource.md) | Measurements | range | [Measurement](Measurement.md) |
| [Terminal](Terminal.md) | Measurements | range | [Measurement](Measurement.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Measurement |
| native | this:Measurement |




