# StringMeasurement


_StringMeasurement represents a measurement with values of type string._





**URI**: [cim:StringMeasurement](http://iec.ch/TC57/CIM100#StringMeasurement)<br />
**Type**: Class




```mermaid
 classDiagram
    class StringMeasurement
    click StringMeasurement href "../StringMeasurement"
      Measurement <|-- StringMeasurement
        click Measurement href "../Measurement"
      
      StringMeasurement : IdentifiedObject.description
        
      StringMeasurement : Measurement.measurementType
        
      StringMeasurement : IdentifiedObject.mRID
        
      StringMeasurement : IdentifiedObject.name
        
      StringMeasurement : Measurement.phases
        
          StringMeasurement --> PhaseCode : Measurement.phases
          click PhaseCode href "../PhaseCode"
        
      StringMeasurement : Measurement.PowerSystemResource
        
          StringMeasurement --> PowerSystemResource : Measurement.PowerSystemResource
          click PowerSystemResource href "../PowerSystemResource"
        
      StringMeasurement : StringMeasurement.StringMeasurementValues
        
          StringMeasurement --> StringMeasurementValue : StringMeasurement.StringMeasurementValues
          click StringMeasurementValue href "../StringMeasurementValue"
        
      StringMeasurement : Measurement.Terminal
        
          StringMeasurement --> ACDCTerminal : Measurement.Terminal
          click ACDCTerminal href "../ACDCTerminal"
        
      StringMeasurement : Measurement.unitMultiplier
        
          StringMeasurement --> UnitMultiplier : Measurement.unitMultiplier
          click UnitMultiplier href "../UnitMultiplier"
        
      StringMeasurement : Measurement.unitSymbol
        
          StringMeasurement --> UnitSymbol : Measurement.unitSymbol
          click UnitSymbol href "../UnitSymbol"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [Measurement](Measurement.md)
        * **StringMeasurement**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| StringMeasurementValues | [cim:StringMeasurement.StringMeasurementValues](http://iec.ch/TC57/CIM100#StringMeasurement.StringMeasurementValues) | * <br />  [StringMeasurementValue](StringMeasurementValue.md)  | The values connected to this measurement | direct |
| Terminal | [cim:Measurement.Terminal](http://iec.ch/TC57/CIM100#Measurement.Terminal) | 0..1 <br />  [ACDCTerminal](ACDCTerminal.md)  | One or more measurements may be associated with a terminal in the network | [Measurement](Measurement.md) |
| measurementType | [cim:Measurement.measurementType](http://iec.ch/TC57/CIM100#Measurement.measurementType) | 1 <br />  string  | Specifies the type of measurement | [Measurement](Measurement.md) |
| phases | [cim:Measurement.phases](http://iec.ch/TC57/CIM100#Measurement.phases) | 0..1 <br />  [PhaseCode](PhaseCode.md)  | Indicates to which phases the measurement applies and avoids the need to use ... | [Measurement](Measurement.md) |
| unitMultiplier | [cim:Measurement.unitMultiplier](http://iec.ch/TC57/CIM100#Measurement.unitMultiplier) | 1 <br />  [UnitMultiplier](UnitMultiplier.md)  | The unit multiplier of the measured quantity | [Measurement](Measurement.md) |
| unitSymbol | [cim:Measurement.unitSymbol](http://iec.ch/TC57/CIM100#Measurement.unitSymbol) | 1 <br />  [UnitSymbol](UnitSymbol.md)  | The unit of measure of the measured quantity | [Measurement](Measurement.md) |
| PowerSystemResource | [cim:Measurement.PowerSystemResource](http://iec.ch/TC57/CIM100#Measurement.PowerSystemResource) | 1 <br />  [PowerSystemResource](PowerSystemResource.md)  | The power system resource that contains the measurement | [Measurement](Measurement.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [StringMeasurementValue](StringMeasurementValue.md) | StringMeasurement | range | [StringMeasurement](StringMeasurement.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:StringMeasurement |
| native | this:StringMeasurement |




