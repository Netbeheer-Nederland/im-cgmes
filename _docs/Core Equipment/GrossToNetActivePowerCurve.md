# GrossToNetActivePowerCurve


_Relationship between the generating unit's gross active power output on the X-axis (measured at the terminals of the machine(s)) and the generating unit's net active power output on the Y-axis (based on utility-defined measurements at the power station). Station service loads, when modelled, should be treated as non-conforming bus loads. There may be more than one curve, depending on the auxiliary equipment that is in service._





**URI**: [cim:GrossToNetActivePowerCurve](http://iec.ch/TC57/CIM100#GrossToNetActivePowerCurve)<br />
**Type**: Class




```mermaid
 classDiagram
    class GrossToNetActivePowerCurve
    click GrossToNetActivePowerCurve href "../GrossToNetActivePowerCurve"
      Curve <|-- GrossToNetActivePowerCurve
        click Curve href "../Curve"
      
      GrossToNetActivePowerCurve : Curve.CurveDatas
        
          GrossToNetActivePowerCurve --> CurveData : Curve.CurveDatas
          click CurveData href "../CurveData"
        
      GrossToNetActivePowerCurve : Curve.curveStyle
        
          GrossToNetActivePowerCurve --> CurveStyle : Curve.curveStyle
          click CurveStyle href "../CurveStyle"
        
      GrossToNetActivePowerCurve : IdentifiedObject.description
        
      GrossToNetActivePowerCurve : IdentifiedObject.energyIdentCodeEic
        
      GrossToNetActivePowerCurve : GrossToNetActivePowerCurve.GeneratingUnit
        
          GrossToNetActivePowerCurve --> GeneratingUnit : GrossToNetActivePowerCurve.GeneratingUnit
          click GeneratingUnit href "../GeneratingUnit"
        
      GrossToNetActivePowerCurve : IdentifiedObject.mRID
        
      GrossToNetActivePowerCurve : IdentifiedObject.name
        
      GrossToNetActivePowerCurve : IdentifiedObject.shortName
        
      GrossToNetActivePowerCurve : Curve.xUnit
        
          GrossToNetActivePowerCurve --> UnitSymbol : Curve.xUnit
          click UnitSymbol href "../UnitSymbol"
        
      GrossToNetActivePowerCurve : Curve.y1Unit
        
          GrossToNetActivePowerCurve --> UnitSymbol : Curve.y1Unit
          click UnitSymbol href "../UnitSymbol"
        
      GrossToNetActivePowerCurve : Curve.y2Unit
        
          GrossToNetActivePowerCurve --> UnitSymbol : Curve.y2Unit
          click UnitSymbol href "../UnitSymbol"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [Curve](Curve.md)
        * **GrossToNetActivePowerCurve**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| GeneratingUnit | [cim:GrossToNetActivePowerCurve.GeneratingUnit](http://iec.ch/TC57/CIM100#GrossToNetActivePowerCurve.GeneratingUnit) | 1 <br />  [GeneratingUnit](GeneratingUnit.md)  | A generating unit may have a gross active power to net active power curve, de... | direct |
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
| [GeneratingUnit](GeneratingUnit.md) | GrossToNetActivePowerCurves | range | [GrossToNetActivePowerCurve](GrossToNetActivePowerCurve.md) |
| [HydroGeneratingUnit](HydroGeneratingUnit.md) | GrossToNetActivePowerCurves | range | [GrossToNetActivePowerCurve](GrossToNetActivePowerCurve.md) |
| [NuclearGeneratingUnit](NuclearGeneratingUnit.md) | GrossToNetActivePowerCurves | range | [GrossToNetActivePowerCurve](GrossToNetActivePowerCurve.md) |
| [SolarGeneratingUnit](SolarGeneratingUnit.md) | GrossToNetActivePowerCurves | range | [GrossToNetActivePowerCurve](GrossToNetActivePowerCurve.md) |
| [ThermalGeneratingUnit](ThermalGeneratingUnit.md) | GrossToNetActivePowerCurves | range | [GrossToNetActivePowerCurve](GrossToNetActivePowerCurve.md) |
| [WindGeneratingUnit](WindGeneratingUnit.md) | GrossToNetActivePowerCurves | range | [GrossToNetActivePowerCurve](GrossToNetActivePowerCurve.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:GrossToNetActivePowerCurve |
| native | this:GrossToNetActivePowerCurve |




