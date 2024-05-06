# VsCapabilityCurve


_The P-Q capability curve for a voltage source converter, with P on X-axis and Qmin and Qmax on Y1-axis and Y2-axis._





**URI**: [cim:VsCapabilityCurve](http://iec.ch/TC57/CIM100#VsCapabilityCurve)<br />
**Type**: Class




```mermaid
 classDiagram
    class VsCapabilityCurve
    click VsCapabilityCurve href "../VsCapabilityCurve"
      Curve <|-- VsCapabilityCurve
        click Curve href "../Curve"
      
      VsCapabilityCurve : Curve.CurveDatas
        
          VsCapabilityCurve --> CurveData : Curve.CurveDatas
          click CurveData href "../CurveData"
        
      VsCapabilityCurve : Curve.curveStyle
        
          VsCapabilityCurve --> CurveStyle : Curve.curveStyle
          click CurveStyle href "../CurveStyle"
        
      VsCapabilityCurve : IdentifiedObject.description
        
      VsCapabilityCurve : IdentifiedObject.energyIdentCodeEic
        
      VsCapabilityCurve : IdentifiedObject.mRID
        
      VsCapabilityCurve : IdentifiedObject.name
        
      VsCapabilityCurve : IdentifiedObject.shortName
        
      VsCapabilityCurve : VsCapabilityCurve.VsConverterDCSides
        
          VsCapabilityCurve --> VsConverter : VsCapabilityCurve.VsConverterDCSides
          click VsConverter href "../VsConverter"
        
      VsCapabilityCurve : Curve.xUnit
        
          VsCapabilityCurve --> UnitSymbol : Curve.xUnit
          click UnitSymbol href "../UnitSymbol"
        
      VsCapabilityCurve : Curve.y1Unit
        
          VsCapabilityCurve --> UnitSymbol : Curve.y1Unit
          click UnitSymbol href "../UnitSymbol"
        
      VsCapabilityCurve : Curve.y2Unit
        
          VsCapabilityCurve --> UnitSymbol : Curve.y2Unit
          click UnitSymbol href "../UnitSymbol"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [Curve](Curve.md)
        * **VsCapabilityCurve**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| VsConverterDCSides | [cim:VsCapabilityCurve.VsConverterDCSides](http://iec.ch/TC57/CIM100#VsCapabilityCurve.VsConverterDCSides) | * <br />  [VsConverter](VsConverter.md)  | All converters with this capability curve | direct |
| curveStyle | [cim:Curve.curveStyle](http://iec.ch/TC57/CIM100#Curve.curveStyle) | 1 <br />  [CurveStyle](CurveStyle.md)  | The style or shape of the curve | [Curve](Curve.md) |
| xUnit | [cim:Curve.xUnit](http://iec.ch/TC57/CIM100#Curve.xUnit) | 1 <br />  [UnitSymbol](UnitSymbol.md)  | The X-axis units of measure | [Curve](Curve.md) |
| y1Unit | [cim:Curve.y1Unit](http://iec.ch/TC57/CIM100#Curve.y1Unit) | 1 <br />  [UnitSymbol](UnitSymbol.md)  | The Y1-axis units of measure | [Curve](Curve.md) |
| y2Unit | [cim:Curve.y2Unit](http://iec.ch/TC57/CIM100#Curve.y2Unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  | The Y2-axis units of measure | [Curve](Curve.md) |
| CurveDatas | [cim:Curve.CurveDatas](http://iec.ch/TC57/CIM100#Curve.CurveDatas) | 1..* <br />  [CurveData](CurveData.md)  | The point data values that define this curve | [Curve](Curve.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [VsConverter](VsConverter.md) | CapabilityCurve | range | [VsCapabilityCurve](VsCapabilityCurve.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:VsCapabilityCurve |
| native | this:VsCapabilityCurve |




