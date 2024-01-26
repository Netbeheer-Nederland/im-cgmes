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
      PowerSystemResource <|-- RegulatingControl
      

      RegulatingControl <|-- TapChangerControl
      
      
      RegulatingControl : IdentifiedObject.description
        
      RegulatingControl : IdentifiedObject.energyIdentCodeEic
        
      RegulatingControl : RegulatingControl.mode
        
          RegulatingControl --> RegulatingControlModeKind : RegulatingControl.mode
        
      RegulatingControl : IdentifiedObject.mRID
        
      RegulatingControl : IdentifiedObject.name
        
      RegulatingControl : RegulatingControl.RegulatingCondEq
        
          RegulatingControl --> RegulatingCondEq : RegulatingControl.RegulatingCondEq
        
      RegulatingControl : RegulatingControl.RegulationSchedule
        
          RegulatingControl --> RegulationSchedule : RegulatingControl.RegulationSchedule
        
      RegulatingControl : IdentifiedObject.shortName
        
      RegulatingControl : RegulatingControl.Terminal
        
          RegulatingControl --> Terminal : RegulatingControl.Terminal
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * **RegulatingControl**
            * [TapChangerControl](TapChangerControl.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| RegulationSchedule | [cim:RegulatingControl.RegulationSchedule](http://iec.ch/TC57/CIM100#RegulatingControl.RegulationSchedule) | 0..* <br />  [RegulationSchedule](RegulationSchedule.md)  | Schedule for this regulating control | direct |
| RegulatingCondEq | [cim:RegulatingControl.RegulatingCondEq](http://iec.ch/TC57/CIM100#RegulatingControl.RegulatingCondEq) | 0..* <br />  [RegulatingCondEq](RegulatingCondEq.md)  | The equipment that participates in this regulating control scheme | direct |
| mode | [cim:RegulatingControl.mode](http://iec.ch/TC57/CIM100#RegulatingControl.mode) | 1..1 <br />  [RegulatingControlModeKind](RegulatingControlModeKind.md)  | The regulating control mode presently available | direct |
| Terminal | [cim:RegulatingControl.Terminal](http://iec.ch/TC57/CIM100#RegulatingControl.Terminal) | 1..1 <br />  [Terminal](Terminal.md)  | The terminal associated with this regulating control | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [AsynchronousMachine](AsynchronousMachine.md) | RegulatingControl | range | [RegulatingControl](RegulatingControl.md) |
| [RegulationSchedule](RegulationSchedule.md) | RegulatingControl | range | [RegulatingControl](RegulatingControl.md) |
| [ExternalNetworkInjection](ExternalNetworkInjection.md) | RegulatingControl | range | [RegulatingControl](RegulatingControl.md) |
| [LinearShuntCompensator](LinearShuntCompensator.md) | RegulatingControl | range | [RegulatingControl](RegulatingControl.md) |
| [NonlinearShuntCompensator](NonlinearShuntCompensator.md) | RegulatingControl | range | [RegulatingControl](RegulatingControl.md) |
| [PowerElectronicsConnection](PowerElectronicsConnection.md) | RegulatingControl | range | [RegulatingControl](RegulatingControl.md) |
| [RegulatingCondEq](RegulatingCondEq.md) | RegulatingControl | range | [RegulatingControl](RegulatingControl.md) |
| [RotatingMachine](RotatingMachine.md) | RegulatingControl | range | [RegulatingControl](RegulatingControl.md) |
| [ShuntCompensator](ShuntCompensator.md) | RegulatingControl | range | [RegulatingControl](RegulatingControl.md) |
| [StaticVarCompensator](StaticVarCompensator.md) | RegulatingControl | range | [RegulatingControl](RegulatingControl.md) |
| [SynchronousMachine](SynchronousMachine.md) | RegulatingControl | range | [RegulatingControl](RegulatingControl.md) |
| [Terminal](Terminal.md) | RegulatingControl | range | [RegulatingControl](RegulatingControl.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:RegulatingControl |
| native | this:RegulatingControl |




