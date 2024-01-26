# CurveData


_Multi-purpose data points for defining a curve.  The use of this generic class is discouraged if a more specific class can be used to specify the X and Y axis values along with their specific data types._





**URI**: [cim:CurveData](http://iec.ch/TC57/CIM100#CurveData)<br />
**Type**: Class




```mermaid
 classDiagram
    class CurveData
      CurveData : CurveData.Curve
        
          CurveData --> Curve : CurveData.Curve
        
      CurveData : CurveData.xvalue
        
      CurveData : CurveData.y1value
        
      CurveData : CurveData.y2value
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| Curve | [cim:CurveData.Curve](http://iec.ch/TC57/CIM100#CurveData.Curve) | 1..1 <br />  [Curve](Curve.md)  | The curve of  this curve data point | direct |
| xvalue | [cim:CurveData.xvalue](http://iec.ch/TC57/CIM100#CurveData.xvalue) | 1..1 <br />  float  | The data value of the X-axis variable,  depending on the X-axis units | direct |
| y1value | [cim:CurveData.y1value](http://iec.ch/TC57/CIM100#CurveData.y1value) | 1..1 <br />  float  | The data value of the  first Y-axis variable, depending on the Y-axis units | direct |
| y2value | [cim:CurveData.y2value](http://iec.ch/TC57/CIM100#CurveData.y2value) | 0..1 <br />  float  | The data value of the second Y-axis variable (if present), depending on the Y... | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [Curve](Curve.md) | CurveDatas | range | [CurveData](CurveData.md) |
| [GrossToNetActivePowerCurve](GrossToNetActivePowerCurve.md) | CurveDatas | range | [CurveData](CurveData.md) |
| [ReactiveCapabilityCurve](ReactiveCapabilityCurve.md) | CurveDatas | range | [CurveData](CurveData.md) |
| [VsCapabilityCurve](VsCapabilityCurve.md) | CurveDatas | range | [CurveData](CurveData.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:CurveData |
| native | this:CurveData |




