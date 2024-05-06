# Analog


_Analog represents an analog Measurement._





**URI**: [cim:Analog](http://iec.ch/TC57/CIM100#Analog)<br />
**Type**: Class




```mermaid
 classDiagram
    class Analog
    click Analog href "../Analog"
      Measurement <|-- Analog
        click Measurement href "../Measurement"
      
      Analog : Analog.AnalogValues
        
          Analog --> AnalogValue : Analog.AnalogValues
          click AnalogValue href "../AnalogValue"
        
      Analog : IdentifiedObject.description
        
      Analog : Analog.LimitSets
        
          Analog --> AnalogLimitSet : Analog.LimitSets
          click AnalogLimitSet href "../AnalogLimitSet"
        
      Analog : Measurement.measurementType
        
      Analog : IdentifiedObject.mRID
        
      Analog : IdentifiedObject.name
        
      Analog : Measurement.phases
        
          Analog --> PhaseCode : Measurement.phases
          click PhaseCode href "../PhaseCode"
        
      Analog : Analog.positiveFlowIn
        
      Analog : Measurement.PowerSystemResource
        
          Analog --> PowerSystemResource : Measurement.PowerSystemResource
          click PowerSystemResource href "../PowerSystemResource"
        
      Analog : Measurement.Terminal
        
          Analog --> ACDCTerminal : Measurement.Terminal
          click ACDCTerminal href "../ACDCTerminal"
        
      Analog : Measurement.unitMultiplier
        
          Analog --> UnitMultiplier : Measurement.unitMultiplier
          click UnitMultiplier href "../UnitMultiplier"
        
      Analog : Measurement.unitSymbol
        
          Analog --> UnitSymbol : Measurement.unitSymbol
          click UnitSymbol href "../UnitSymbol"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [Measurement](Measurement.md)
        * **Analog**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| positiveFlowIn | [cim:Analog.positiveFlowIn](http://iec.ch/TC57/CIM100#Analog.positiveFlowIn) | 0..1 <br />  boolean  | If true then this measurement is an active power, reactive power or current w... | direct |
| AnalogValues | [cim:Analog.AnalogValues](http://iec.ch/TC57/CIM100#Analog.AnalogValues) | * <br />  [AnalogValue](AnalogValue.md)  | The values connected to this measurement | direct |
| LimitSets | [cim:Analog.LimitSets](http://iec.ch/TC57/CIM100#Analog.LimitSets) | * <br />  [AnalogLimitSet](AnalogLimitSet.md)  | A measurement may have zero or more limit ranges defined for it | direct |
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
| [AnalogLimitSet](AnalogLimitSet.md) | Measurements | range | [Analog](Analog.md) |
| [AnalogValue](AnalogValue.md) | Analog | range | [Analog](Analog.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Operation-EU#Package_OperationProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Analog |
| native | this:Analog |




