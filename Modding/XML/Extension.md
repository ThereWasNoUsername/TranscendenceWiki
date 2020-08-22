# Extension

## Extension Types

### TranscendenceAdventure
- Shows up on Adventure Select
- Defines <AdventureDesc> type
- Loaded on select
- Poor debugging support

### TranscendenceExtension
- Can be loaded on Adventure Select

### TranscendenceLibrary
- Must be a <Library> reference by loaded extension to be active.
### TranscendenceModule
- Must be a <Module> reference by loaded extension to be active.

## Contents

### Libraries
For information about the library itself, see [TranscendenceLibrary](Extension.md#transcendencelibrary)
- <Library>
  - unid: UNID of <TranscendenceLibrary> to reference
### Modules
For information about the module itself, see [TranscendenceModule](Extension.md#transcendencemodule)
- <Modules>
  - <Module>
    - filename: Relative path to <TranscendenceModule> file

### Globals
A Lisp block that runs upon extension load. Use it to define custom helper functions that the rest of your code will need.

### [DesignTypes](DesignType.md)

