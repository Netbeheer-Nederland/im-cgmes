# CsConverter


_DC side of the current source converter (CSC)._

_The firing angle controls the dc voltage at the converter, both for rectifier and inverter. The difference between the dc voltages of the rectifier and inverter determines the dc current. The extinction angle is used to limit the dc voltage at the inverter, if needed, and is not used in active power control. The firing angle, transformer tap position and number of connected filters are the primary means to control a current source dc line. Higher level controls are built on top, e.g. dc voltage, dc current and active power. From a steady state perspective it is sufficient to specify the wanted active power transfer (ACDCConverter.targetPpcc) and the control functions will set the dc voltage, dc current, firing angle, transformer tap position and number of connected filters to meet this. Therefore attributes targetAlpha and targetGamma are not applicable in this case._

_The reactive power consumed by the converter is a function of the firing angle, transformer tap position and number of connected filter, which can be approximated with half of the active power. The losses is a function of the dc voltage and dc current._

_The attributes minAlpha and maxAlpha define the range of firing angles for rectifier operation between which no discrete tap changer action takes place. The range is typically 10-18 degrees._

_The attributes minGamma and maxGamma define the range of extinction angles for inverter operation between which no discrete tap changer action takes place. The range is typically 17-20 degrees._





**URI**: [cim:CsConverter](http://iec.ch/TC57/CIM100#CsConverter)<br />
**Type**: Class




```mermaid
 classDiagram
    class CsConverter
      ACDCConverter <|-- CsConverter
      
      CsConverter : CsConverter.alpha
        
          CsConverter --> AngleDegrees : CsConverter.alpha
        
      CsConverter : CsConverter.gamma
        
          CsConverter --> AngleDegrees : CsConverter.gamma
        
      CsConverter : ACDCConverter.idc
        
          CsConverter --> CurrentFlow : ACDCConverter.idc
        
      CsConverter : ACDCConverter.poleLossP
        
          CsConverter --> ActivePower : ACDCConverter.poleLossP
        
      CsConverter : ConductingEquipment.SvStatus
        
          CsConverter --> SvStatus : ConductingEquipment.SvStatus
        
      CsConverter : ACDCConverter.uc
        
          CsConverter --> Voltage : ACDCConverter.uc
        
      CsConverter : ACDCConverter.udc
        
          CsConverter --> Voltage : ACDCConverter.udc
        
      
```





## Inheritance
* [ConductingEquipment](ConductingEquipment.md)
    * [ACDCConverter](ACDCConverter.md)
        * **CsConverter**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| alpha | [cim:CsConverter.alpha](http://iec.ch/TC57/CIM100#CsConverter.alpha) | 1..1 <br />  [AngleDegrees](AngleDegrees.md)  | Firing angle that determines the dc voltage at the converter dc terminal | direct |
| gamma | [cim:CsConverter.gamma](http://iec.ch/TC57/CIM100#CsConverter.gamma) | 1..1 <br />  [AngleDegrees](AngleDegrees.md)  | Extinction angle | direct |
| idc | [cim:ACDCConverter.idc](http://iec.ch/TC57/CIM100#ACDCConverter.idc) | 1..1 <br />  [CurrentFlow](CurrentFlow.md)  | Converter DC current, also called Id | [ACDCConverter](ACDCConverter.md) |
| poleLossP | [cim:ACDCConverter.poleLossP](http://iec.ch/TC57/CIM100#ACDCConverter.poleLossP) | 1..1 <br />  [ActivePower](ActivePower.md)  | The active power loss at a DC Pole  | [ACDCConverter](ACDCConverter.md) |
| uc | [cim:ACDCConverter.uc](http://iec.ch/TC57/CIM100#ACDCConverter.uc) | 1..1 <br />  [Voltage](Voltage.md)  | Line-to-line converter voltage, the voltage at the AC side of the valve | [ACDCConverter](ACDCConverter.md) |
| udc | [cim:ACDCConverter.udc](http://iec.ch/TC57/CIM100#ACDCConverter.udc) | 1..1 <br />  [Voltage](Voltage.md)  | Converter voltage at the DC side, also called Ud | [ACDCConverter](ACDCConverter.md) |
| SvStatus | [cim:ConductingEquipment.SvStatus](http://iec.ch/TC57/CIM100#ConductingEquipment.SvStatus) | 0..1 <br />  [SvStatus](SvStatus.md)  | The status state variable associated with this conducting equipment | [ConductingEquipment](ConductingEquipment.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/StateVariables-EU#Package_StateVariablesProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:CsConverter |
| native | this:CsConverter |




