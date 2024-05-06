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
    click CsConverter href "../CsConverter"
      ACDCConverter <|-- CsConverter
        click ACDCConverter href "../ACDCConverter"
      
      CsConverter : Equipment.aggregate
        
      CsConverter : ACDCConverter.baseS
        
          CsConverter --> ApparentPower : ACDCConverter.baseS
          click ApparentPower href "../ApparentPower"
        
      CsConverter : ConductingEquipment.BaseVoltage
        
          CsConverter --> BaseVoltage : ConductingEquipment.BaseVoltage
          click BaseVoltage href "../BaseVoltage"
        
      CsConverter : ACDCConverter.DCTerminals
        
          CsConverter --> ACDCConverterDCTerminal : ACDCConverter.DCTerminals
          click ACDCConverterDCTerminal href "../ACDCConverterDCTerminal"
        
      CsConverter : IdentifiedObject.description
        
      CsConverter : IdentifiedObject.energyIdentCodeEic
        
      CsConverter : Equipment.EquipmentContainer
        
          CsConverter --> EquipmentContainer : Equipment.EquipmentContainer
          click EquipmentContainer href "../EquipmentContainer"
        
      CsConverter : ACDCConverter.idleLoss
        
          CsConverter --> ActivePower : ACDCConverter.idleLoss
          click ActivePower href "../ActivePower"
        
      CsConverter : CsConverter.maxAlpha
        
          CsConverter --> AngleDegrees : CsConverter.maxAlpha
          click AngleDegrees href "../AngleDegrees"
        
      CsConverter : CsConverter.maxGamma
        
          CsConverter --> AngleDegrees : CsConverter.maxGamma
          click AngleDegrees href "../AngleDegrees"
        
      CsConverter : CsConverter.maxIdc
        
          CsConverter --> CurrentFlow : CsConverter.maxIdc
          click CurrentFlow href "../CurrentFlow"
        
      CsConverter : ACDCConverter.maxP
        
          CsConverter --> ActivePower : ACDCConverter.maxP
          click ActivePower href "../ActivePower"
        
      CsConverter : ACDCConverter.maxUdc
        
          CsConverter --> Voltage : ACDCConverter.maxUdc
          click Voltage href "../Voltage"
        
      CsConverter : CsConverter.minAlpha
        
          CsConverter --> AngleDegrees : CsConverter.minAlpha
          click AngleDegrees href "../AngleDegrees"
        
      CsConverter : CsConverter.minGamma
        
          CsConverter --> AngleDegrees : CsConverter.minGamma
          click AngleDegrees href "../AngleDegrees"
        
      CsConverter : CsConverter.minIdc
        
          CsConverter --> CurrentFlow : CsConverter.minIdc
          click CurrentFlow href "../CurrentFlow"
        
      CsConverter : ACDCConverter.minP
        
          CsConverter --> ActivePower : ACDCConverter.minP
          click ActivePower href "../ActivePower"
        
      CsConverter : ACDCConverter.minUdc
        
          CsConverter --> Voltage : ACDCConverter.minUdc
          click Voltage href "../Voltage"
        
      CsConverter : IdentifiedObject.mRID
        
      CsConverter : IdentifiedObject.name
        
      CsConverter : Equipment.normallyInService
        
      CsConverter : ACDCConverter.numberOfValves
        
      CsConverter : Equipment.OperationalLimitSet
        
          CsConverter --> OperationalLimitSet : Equipment.OperationalLimitSet
          click OperationalLimitSet href "../OperationalLimitSet"
        
      CsConverter : ACDCConverter.PccTerminal
        
          CsConverter --> Terminal : ACDCConverter.PccTerminal
          click Terminal href "../Terminal"
        
      CsConverter : CsConverter.ratedIdc
        
          CsConverter --> CurrentFlow : CsConverter.ratedIdc
          click CurrentFlow href "../CurrentFlow"
        
      CsConverter : ACDCConverter.ratedUdc
        
          CsConverter --> Voltage : ACDCConverter.ratedUdc
          click Voltage href "../Voltage"
        
      CsConverter : ACDCConverter.resistiveLoss
        
          CsConverter --> Resistance : ACDCConverter.resistiveLoss
          click Resistance href "../Resistance"
        
      CsConverter : IdentifiedObject.shortName
        
      CsConverter : ACDCConverter.switchingLoss
        
          CsConverter --> ActivePowerPerCurrentFlow : ACDCConverter.switchingLoss
          click ActivePowerPerCurrentFlow href "../ActivePowerPerCurrentFlow"
        
      CsConverter : ConductingEquipment.Terminals
        
          CsConverter --> Terminal : ConductingEquipment.Terminals
          click Terminal href "../Terminal"
        
      CsConverter : ACDCConverter.valveU0
        
          CsConverter --> Voltage : ACDCConverter.valveU0
          click Voltage href "../Voltage"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [ACDCConverter](ACDCConverter.md)
                    * **CsConverter**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| maxAlpha | [cim:CsConverter.maxAlpha](http://iec.ch/TC57/CIM100#CsConverter.maxAlpha) | 0..1 <br />  [AngleDegrees](AngleDegrees.md)  | Maximum firing angle | direct |
| maxGamma | [cim:CsConverter.maxGamma](http://iec.ch/TC57/CIM100#CsConverter.maxGamma) | 0..1 <br />  [AngleDegrees](AngleDegrees.md)  | Maximum extinction angle | direct |
| maxIdc | [cim:CsConverter.maxIdc](http://iec.ch/TC57/CIM100#CsConverter.maxIdc) | 0..1 <br />  [CurrentFlow](CurrentFlow.md)  | The maximum direct current (Id) on the DC side at which the converter should ... | direct |
| minAlpha | [cim:CsConverter.minAlpha](http://iec.ch/TC57/CIM100#CsConverter.minAlpha) | 0..1 <br />  [AngleDegrees](AngleDegrees.md)  | Minimum firing angle | direct |
| minGamma | [cim:CsConverter.minGamma](http://iec.ch/TC57/CIM100#CsConverter.minGamma) | 0..1 <br />  [AngleDegrees](AngleDegrees.md)  | Minimum extinction angle | direct |
| minIdc | [cim:CsConverter.minIdc](http://iec.ch/TC57/CIM100#CsConverter.minIdc) | 0..1 <br />  [CurrentFlow](CurrentFlow.md)  | The minimum direct current (Id) on the DC side at which the converter should ... | direct |
| ratedIdc | [cim:CsConverter.ratedIdc](http://iec.ch/TC57/CIM100#CsConverter.ratedIdc) | 0..1 <br />  [CurrentFlow](CurrentFlow.md)  | Rated converter DC current, also called IdN | direct |
| baseS | [cim:ACDCConverter.baseS](http://iec.ch/TC57/CIM100#ACDCConverter.baseS) | 0..1 <br />  [ApparentPower](ApparentPower.md)  | Base apparent power of the converter pole | [ACDCConverter](ACDCConverter.md) |
| idleLoss | [cim:ACDCConverter.idleLoss](http://iec.ch/TC57/CIM100#ACDCConverter.idleLoss) | 0..1 <br />  [ActivePower](ActivePower.md)  | Active power loss in pole at no power transfer | [ACDCConverter](ACDCConverter.md) |
| maxUdc | [cim:ACDCConverter.maxUdc](http://iec.ch/TC57/CIM100#ACDCConverter.maxUdc) | 0..1 <br />  [Voltage](Voltage.md)  | The maximum voltage on the DC side at which the converter should operate | [ACDCConverter](ACDCConverter.md) |
| minUdc | [cim:ACDCConverter.minUdc](http://iec.ch/TC57/CIM100#ACDCConverter.minUdc) | 0..1 <br />  [Voltage](Voltage.md)  | The minimum voltage on the DC side at which the converter should operate | [ACDCConverter](ACDCConverter.md) |
| numberOfValves | [cim:ACDCConverter.numberOfValves](http://iec.ch/TC57/CIM100#ACDCConverter.numberOfValves) | 0..1 <br />  integer  | Number of valves in the converter | [ACDCConverter](ACDCConverter.md) |
| ratedUdc | [cim:ACDCConverter.ratedUdc](http://iec.ch/TC57/CIM100#ACDCConverter.ratedUdc) | 0..1 <br />  [Voltage](Voltage.md)  | Rated converter DC voltage, also called UdN | [ACDCConverter](ACDCConverter.md) |
| resistiveLoss | [cim:ACDCConverter.resistiveLoss](http://iec.ch/TC57/CIM100#ACDCConverter.resistiveLoss) | 0..1 <br />  [Resistance](Resistance.md)  | It is converter’s configuration data used in power flow | [ACDCConverter](ACDCConverter.md) |
| switchingLoss | [cim:ACDCConverter.switchingLoss](http://iec.ch/TC57/CIM100#ACDCConverter.switchingLoss) | 0..1 <br />  [ActivePowerPerCurrentFlow](ActivePowerPerCurrentFlow.md)  | Switching losses, relative to the base apparent power 'baseS' | [ACDCConverter](ACDCConverter.md) |
| valveU0 | [cim:ACDCConverter.valveU0](http://iec.ch/TC57/CIM100#ACDCConverter.valveU0) | 0..1 <br />  [Voltage](Voltage.md)  | Valve threshold voltage, also called Uvalve | [ACDCConverter](ACDCConverter.md) |
| maxP | [cim:ACDCConverter.maxP](http://iec.ch/TC57/CIM100#ACDCConverter.maxP) | 0..1 <br />  [ActivePower](ActivePower.md)  | Maximum active power limit | [ACDCConverter](ACDCConverter.md) |
| minP | [cim:ACDCConverter.minP](http://iec.ch/TC57/CIM100#ACDCConverter.minP) | 0..1 <br />  [ActivePower](ActivePower.md)  | Minimum active power limit | [ACDCConverter](ACDCConverter.md) |
| PccTerminal | [cim:ACDCConverter.PccTerminal](http://iec.ch/TC57/CIM100#ACDCConverter.PccTerminal) | 0..1 <br />  [Terminal](Terminal.md)  | Point of common coupling terminal for this converter DC side | [ACDCConverter](ACDCConverter.md) |
| DCTerminals | [cim:ACDCConverter.DCTerminals](http://iec.ch/TC57/CIM100#ACDCConverter.DCTerminals) | * <br />  [ACDCConverterDCTerminal](ACDCConverterDCTerminal.md)  | A DC converter have DC converter terminals | [ACDCConverter](ACDCConverter.md) |
| BaseVoltage | [cim:ConductingEquipment.BaseVoltage](http://iec.ch/TC57/CIM100#ConductingEquipment.BaseVoltage) | 0..1 <br />  [BaseVoltage](BaseVoltage.md)  | Base voltage of this conducting equipment | [ConductingEquipment](ConductingEquipment.md) |
| Terminals | [cim:ConductingEquipment.Terminals](http://iec.ch/TC57/CIM100#ConductingEquipment.Terminals) | * <br />  [Terminal](Terminal.md)  | Conducting equipment have terminals that may be connected to other conducting... | [ConductingEquipment](ConductingEquipment.md) |
| aggregate | [cim:Equipment.aggregate](http://iec.ch/TC57/CIM100#Equipment.aggregate) | 0..1 <br />  boolean  | The aggregate flag provides an alternative way of representing an aggregated ... | [Equipment](Equipment.md) |
| normallyInService | [cim:Equipment.normallyInService](http://iec.ch/TC57/CIM100#Equipment.normallyInService) | 0..1 <br />  boolean  | Specifies the availability of the equipment under normal operating conditions | [Equipment](Equipment.md) |
| EquipmentContainer | [cim:Equipment.EquipmentContainer](http://iec.ch/TC57/CIM100#Equipment.EquipmentContainer) | 0..1 <br />  [EquipmentContainer](EquipmentContainer.md)  | Container of this equipment | [Equipment](Equipment.md) |
| OperationalLimitSet | [cim:Equipment.OperationalLimitSet](http://iec.ch/TC57/CIM100#Equipment.OperationalLimitSet) | * <br />  [OperationalLimitSet](OperationalLimitSet.md)  | The operational limit sets associated with this equipment | [Equipment](Equipment.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:CsConverter |
| native | this:CsConverter |




