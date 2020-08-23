# Types

## Binding
The engine binds the design collection to the design types in `CDesignCollection::BindDesign`
- Fire OnGlobalTypesInit
- Evaluate TemplateTypes
- Resolve [inheritance](Types.md#inheritance) chains.
- Resolve [overrides](Types.md#overrides)
- Pre-bind
- Bind


### Inheritance
Any type can inherit from **one** other type of the same DesignType. A type [cannot inherit from itself](https://github.com/kronosaur/TranscendenceDev/blob/ad03980dbb7c50a621d71840af28afab91746b56/Mammoth/TSE/CDesignCollection.cpp#L1805), [nor can it inherit from a different DesignType](https://github.com/kronosaur/TranscendenceDev/blob/ad03980dbb7c50a621d71840af28afab91746b56/Mammoth/TSE/CDesignCollection.cpp#L1829)

[CDesignCollection::ResolveInheritingType](https://github.com/kronosaur/TranscendenceDev/blob/ad03980dbb7c50a621d71840af28afab91746b56/Mammoth/TSE/CDesignCollection.cpp#L1768)
### Overrides
Any type can override **one** other type of the same DesignType. A type [cannot override a different DesignType](https://github.com/kronosaur/TranscendenceDev/blob/ad03980dbb7c50a621d71840af28afab91746b56/Mammoth/TSE/CDesignCollection.cpp#L1909)