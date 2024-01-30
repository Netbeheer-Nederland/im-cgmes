# IdentifiedObject


_This is a root class to provide common identification for all classes needing identification and naming attributes._





**URI**: [cim:IdentifiedObject](http://iec.ch/TC57/CIM100#IdentifiedObject)<br />
**Type**: Class




```mermaid
 classDiagram
    class IdentifiedObject
      IdentifiedObject <|-- ACDCTerminal
      IdentifiedObject <|-- PowerSystemResource
      IdentifiedObject <|-- RemoteInputSignal
      IdentifiedObject <|-- DynamicsFunctionBlock
      IdentifiedObject <|-- GenICompensationForGenJ
      IdentifiedObject <|-- WindAeroConstIEC
      IdentifiedObject <|-- WindAeroOneDimIEC
      IdentifiedObject <|-- WindAeroTwoDimIEC
      IdentifiedObject <|-- WindContCurrLimIEC
      IdentifiedObject <|-- WindContPitchAngleIEC
      IdentifiedObject <|-- WindContPType3IEC
      IdentifiedObject <|-- WindContPType4aIEC
      IdentifiedObject <|-- WindContPType4bIEC
      IdentifiedObject <|-- WindContQIEC
      IdentifiedObject <|-- WindContQLimIEC
      IdentifiedObject <|-- WindContQPQULimIEC
      IdentifiedObject <|-- WindContRotorRIEC
      IdentifiedObject <|-- WindDynamicsLookupTable
      IdentifiedObject <|-- WindGenType3IEC
      IdentifiedObject <|-- WindGenType4IEC
      IdentifiedObject <|-- WindMechIEC
      IdentifiedObject <|-- WindPitchContPowerIEC
      IdentifiedObject <|-- WindPlantFreqPcontrolIEC
      IdentifiedObject <|-- WindPlantReactiveControlIEC
      IdentifiedObject <|-- WindProtectionIEC
      IdentifiedObject <|-- WindRefFrameRotIEC
      IdentifiedObject <|-- LoadDynamics
      IdentifiedObject <|-- LoadStatic
      IdentifiedObject <|-- LoadMotor
      
      IdentifiedObject : IdentifiedObject.description
        
      IdentifiedObject : IdentifiedObject.mRID
        
      IdentifiedObject : IdentifiedObject.name
        
      
```





## Inheritance
* **IdentifiedObject**
    * [ACDCTerminal](ACDCTerminal.md)
    * [PowerSystemResource](PowerSystemResource.md)
    * [RemoteInputSignal](RemoteInputSignal.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
    * [GenICompensationForGenJ](GenICompensationForGenJ.md)
    * [WindAeroConstIEC](WindAeroConstIEC.md)
    * [WindAeroOneDimIEC](WindAeroOneDimIEC.md)
    * [WindAeroTwoDimIEC](WindAeroTwoDimIEC.md)
    * [WindContCurrLimIEC](WindContCurrLimIEC.md)
    * [WindContPitchAngleIEC](WindContPitchAngleIEC.md)
    * [WindContPType3IEC](WindContPType3IEC.md)
    * [WindContPType4aIEC](WindContPType4aIEC.md)
    * [WindContPType4bIEC](WindContPType4bIEC.md)
    * [WindContQIEC](WindContQIEC.md)
    * [WindContQLimIEC](WindContQLimIEC.md)
    * [WindContQPQULimIEC](WindContQPQULimIEC.md)
    * [WindContRotorRIEC](WindContRotorRIEC.md)
    * [WindDynamicsLookupTable](WindDynamicsLookupTable.md)
    * [WindGenType3IEC](WindGenType3IEC.md)
    * [WindGenType4IEC](WindGenType4IEC.md)
    * [WindMechIEC](WindMechIEC.md)
    * [WindPitchContPowerIEC](WindPitchContPowerIEC.md)
    * [WindPlantFreqPcontrolIEC](WindPlantFreqPcontrolIEC.md)
    * [WindPlantReactiveControlIEC](WindPlantReactiveControlIEC.md)
    * [WindProtectionIEC](WindProtectionIEC.md)
    * [WindRefFrameRotIEC](WindRefFrameRotIEC.md)
    * [LoadDynamics](LoadDynamics.md)
    * [LoadStatic](LoadStatic.md)
    * [LoadMotor](LoadMotor.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | direct |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | direct |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | direct |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:IdentifiedObject |
| native | this:IdentifiedObject |




