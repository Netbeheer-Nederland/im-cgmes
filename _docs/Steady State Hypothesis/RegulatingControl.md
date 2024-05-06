# RegulatingControl


_Specifies a set of equipment that works together to control a power system quantity such as voltage or flow. _

_Remote bus voltage control is possible by specifying the controlled terminal located at some place remote from the controlling equipment._

_The specified terminal shall be associated with the connectivity node of the controlled point.  The most specific subtype of RegulatingControl shall be used in case such equipment participate in the control, e.g. TapChangerControl for tap changers._

_For flow control, load sign convention is used, i.e. positive sign means flow out from a TopologicalNode (bus) into the conducting equipment._

_The attribute minAllowedTargetValue and maxAllowedTargetValue are required in the following cases:_

_- For a power generating module operated in power factor control mode to specify maximum and minimum power factor values;_

_- Whenever it is necessary to have an off center target voltage for the tap changer regulator. For instance, due to long cables to off shore wind farms and the need to have a simpler setup at the off shore transformer platform, the voltage is controlled from the land at the connection point for the off shore wind farm. Since there usually is a voltage rise along the cable, there is typical and overvoltage of up 3-4 kV compared to the on shore station. Thus in normal operation the tap changer on the on shore station is operated with a target set point, which is in the lower parts of the dead band._

_The attributes minAllowedTargetValue and maxAllowedTargetValue are not related to the attribute targetDeadband and thus they are not treated as an alternative of the targetDeadband. They are needed due to limitations in the local substation controller. The attribute targetDeadband is used to prevent the power flow from move the tap position in circles (hunting) that is to be used regardless of the attributes minAllowedTargetValue and maxAllowedTargetValue._





**URI**: [cim:RegulatingControl](http://iec.ch/TC57/CIM100#RegulatingControl)<br />
**Type**: Class




```mermaid
 classDiagram
    class RegulatingControl
    click RegulatingControl href "../RegulatingControl"
      PowerSystemResource <|-- RegulatingControl
        click PowerSystemResource href "../PowerSystemResource"
      

      RegulatingControl <|-- TapChangerControl
        click TapChangerControl href "../TapChangerControl"
      
      
      RegulatingControl : RegulatingControl.discrete
        
      RegulatingControl : RegulatingControl.enabled
        
      RegulatingControl : RegulatingControl.maxAllowedTargetValue
        
      RegulatingControl : RegulatingControl.minAllowedTargetValue
        
      RegulatingControl : IdentifiedObject.mRID
        
      RegulatingControl : RegulatingControl.targetDeadband
        
      RegulatingControl : RegulatingControl.targetValue
        
      RegulatingControl : RegulatingControl.targetValueUnitMultiplier
        
          RegulatingControl --> UnitMultiplier : RegulatingControl.targetValueUnitMultiplier
          click UnitMultiplier href "../UnitMultiplier"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * **RegulatingControl**
            * [TapChangerControl](TapChangerControl.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| discrete | [cim:RegulatingControl.discrete](http://iec.ch/TC57/CIM100#RegulatingControl.discrete) | 1 <br />  boolean  | The regulation is performed in a discrete mode | direct |
| enabled | [cim:RegulatingControl.enabled](http://iec.ch/TC57/CIM100#RegulatingControl.enabled) | 1 <br />  boolean  | The flag tells if regulation is enabled | direct |
| targetDeadband | [cim:RegulatingControl.targetDeadband](http://iec.ch/TC57/CIM100#RegulatingControl.targetDeadband) | 0..1 <br />  float  | This is a deadband used with discrete control to avoid excessive update of co... | direct |
| targetValue | [cim:RegulatingControl.targetValue](http://iec.ch/TC57/CIM100#RegulatingControl.targetValue) | 1 <br />  float  | The target value specified for case input | direct |
| targetValueUnitMultiplier | [cim:RegulatingControl.targetValueUnitMultiplier](http://iec.ch/TC57/CIM100#RegulatingControl.targetValueUnitMultiplier) | 1 <br />  [UnitMultiplier](UnitMultiplier.md)  | Specify the multiplier for used for the targetValue | direct |
| maxAllowedTargetValue | [cim:RegulatingControl.maxAllowedTargetValue](http://iec.ch/TC57/CIM100#RegulatingControl.maxAllowedTargetValue) | 0..1 <br />  float  | Maximum allowed target value (RegulatingControl | direct |
| minAllowedTargetValue | [cim:RegulatingControl.minAllowedTargetValue](http://iec.ch/TC57/CIM100#RegulatingControl.minAllowedTargetValue) | 0..1 <br />  float  | Minimum allowed target value (RegulatingControl | direct |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:RegulatingControl |
| native | this:RegulatingControl |




