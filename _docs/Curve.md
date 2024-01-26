# Curve


_A multi-purpose curve or functional relationship between an independent variable (X-axis) and dependent (Y-axis) variables._





**URI**: [cim:Curve](http://iec.ch/TC57/CIM100#Curve)<br />
**Type**: Class




```mermaid
 classDiagram
    class Curve
      IdentifiedObject <|-- Curve
      

      Curve <|-- GrossToNetActivePowerCurve
      Curve <|-- ReactiveCapabilityCurve
      Curve <|-- VsCapabilityCurve
      
      
      Curve : Curve.CurveDatas
        
          Curve --> CurveData : Curve.CurveDatas
        
      Curve : Curve.curveStyle
        
          Curve --> CurveStyle : Curve.curveStyle
        
      Curve : IdentifiedObject.description
        
      Curve : IdentifiedObject.energyIdentCodeEic
        
      Curve : IdentifiedObject.mRID
        
      Curve : IdentifiedObject.name
        
      Curve : IdentifiedObject.shortName
        
      Curve : Curve.xUnit
        
          Curve --> UnitSymbol : Curve.xUnit
        
      Curve : Curve.y1Unit
        
          Curve --> UnitSymbol : Curve.y1Unit
        
      Curve : Curve.y2Unit
        
          Curve --> UnitSymbol : Curve.y2Unit
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **Curve**
        * [GrossToNetActivePowerCurve](GrossToNetActivePowerCurve.md)
        * [ReactiveCapabilityCurve](ReactiveCapabilityCurve.md)
        * [VsCapabilityCurve](VsCapabilityCurve.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| curveStyle | [cim:Curve.curveStyle](http://iec.ch/TC57/CIM100#Curve.curveStyle) | 1..1 <br />  [CurveStyle](CurveStyle.md)  | The style or shape of the curve | direct |
| xUnit | [cim:Curve.xUnit](http://iec.ch/TC57/CIM100#Curve.xUnit) | 1..1 <br />  [UnitSymbol](UnitSymbol.md)  | The X-axis units of measure | direct |
| y1Unit | [cim:Curve.y1Unit](http://iec.ch/TC57/CIM100#Curve.y1Unit) | 1..1 <br />  [UnitSymbol](UnitSymbol.md)  | The Y1-axis units of measure | direct |
| y2Unit | [cim:Curve.y2Unit](http://iec.ch/TC57/CIM100#Curve.y2Unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  | The Y2-axis units of measure | direct |
| CurveDatas | [cim:Curve.CurveDatas](http://iec.ch/TC57/CIM100#Curve.CurveDatas) | 1..* <br />  [CurveData](CurveData.md)  | The point data values that define this curve | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [CurveData](CurveData.md) | Curve | range | [Curve](Curve.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Curve |
| native | this:Curve |




