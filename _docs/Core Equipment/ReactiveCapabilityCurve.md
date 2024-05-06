# ReactiveCapabilityCurve


_Reactive power rating envelope versus the synchronous machine's active power, in both the generating and motoring modes. For each active power value there is a corresponding high and low reactive power limit  value. Typically there will be a separate curve for each coolant condition, such as hydrogen pressure.  The Y1 axis values represent reactive minimum and the Y2 axis values represent reactive maximum._





**URI**: [cim:ReactiveCapabilityCurve](http://iec.ch/TC57/CIM100#ReactiveCapabilityCurve)<br />
**Type**: Class




```mermaid
 classDiagram
    class ReactiveCapabilityCurve
    click ReactiveCapabilityCurve href "../ReactiveCapabilityCurve"
      Curve <|-- ReactiveCapabilityCurve
        click Curve href "../Curve"
      
      ReactiveCapabilityCurve : Curve.CurveDatas
        
          ReactiveCapabilityCurve --> CurveData : Curve.CurveDatas
          click CurveData href "../CurveData"
        
      ReactiveCapabilityCurve : Curve.curveStyle
        
          ReactiveCapabilityCurve --> CurveStyle : Curve.curveStyle
          click CurveStyle href "../CurveStyle"
        
      ReactiveCapabilityCurve : IdentifiedObject.description
        
      ReactiveCapabilityCurve : IdentifiedObject.energyIdentCodeEic
        
      ReactiveCapabilityCurve : ReactiveCapabilityCurve.EquivalentInjection
        
          ReactiveCapabilityCurve --> EquivalentInjection : ReactiveCapabilityCurve.EquivalentInjection
          click EquivalentInjection href "../EquivalentInjection"
        
      ReactiveCapabilityCurve : ReactiveCapabilityCurve.InitiallyUsedBySynchronousMachines
        
          ReactiveCapabilityCurve --> SynchronousMachine : ReactiveCapabilityCurve.InitiallyUsedBySynchronousMachines
          click SynchronousMachine href "../SynchronousMachine"
        
      ReactiveCapabilityCurve : IdentifiedObject.mRID
        
      ReactiveCapabilityCurve : IdentifiedObject.name
        
      ReactiveCapabilityCurve : IdentifiedObject.shortName
        
      ReactiveCapabilityCurve : Curve.xUnit
        
          ReactiveCapabilityCurve --> UnitSymbol : Curve.xUnit
          click UnitSymbol href "../UnitSymbol"
        
      ReactiveCapabilityCurve : Curve.y1Unit
        
          ReactiveCapabilityCurve --> UnitSymbol : Curve.y1Unit
          click UnitSymbol href "../UnitSymbol"
        
      ReactiveCapabilityCurve : Curve.y2Unit
        
          ReactiveCapabilityCurve --> UnitSymbol : Curve.y2Unit
          click UnitSymbol href "../UnitSymbol"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [Curve](Curve.md)
        * **ReactiveCapabilityCurve**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| EquivalentInjection | [cim:ReactiveCapabilityCurve.EquivalentInjection](http://iec.ch/TC57/CIM100#ReactiveCapabilityCurve.EquivalentInjection) | * <br />  [EquivalentInjection](EquivalentInjection.md)  | The equivalent injection using this reactive capability curve | direct |
| InitiallyUsedBySynchronousMachines | [cim:ReactiveCapabilityCurve.InitiallyUsedBySynchronousMachines](http://iec.ch/TC57/CIM100#ReactiveCapabilityCurve.InitiallyUsedBySynchronousMachines) | 1..* <br />  [SynchronousMachine](SynchronousMachine.md)  | Synchronous machines using this curve as default | direct |
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
| [EquivalentInjection](EquivalentInjection.md) | ReactiveCapabilityCurve | range | [ReactiveCapabilityCurve](ReactiveCapabilityCurve.md) |
| [SynchronousMachine](SynchronousMachine.md) | InitialReactiveCapabilityCurve | range | [ReactiveCapabilityCurve](ReactiveCapabilityCurve.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ReactiveCapabilityCurve |
| native | this:ReactiveCapabilityCurve |




