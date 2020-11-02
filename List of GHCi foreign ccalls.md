
1. `libraries/ghci/GHCi/StaticPtrTable.hs`:
	```java
	foreign import ccall "hs_spt_insert_stableptr"
	```
2. `libraries/ghci/GHCi/Run.hs`:
    ```java
	foreign import ccall "revertCAFs"
	foreign import ccall "&rts_stop_next_breakpoint"
	foreign import ccall "&rts_stop_on_exception"
	foreign import ccall "&rts_breakpoint_io_action"
	foreign import ccall unsafe "mkCostCentre"
	```
3. `libraries/ghci/GHCi/ObjLink.hs`:
    ```java
    foreign import ccall unsafe "addDLL"
    foreign import ccall unsafe "initLinker_"
    foreign import ccall unsafe "lookupSymbol"
    foreign import ccall unsafe "loadArchive"
    foreign import ccall unsafe "loadObj"
    foreign import ccall unsafe "purgeObj"
    foreign import ccall unsafe "unloadObj"
    foreign import ccall unsafe "resolveObjs"
    foreign import ccall unsafe "addLibrarySearchPath"
    foreign import ccall unsafe "findSystemLibrary"
    foreign import ccall unsafe "removeLibrarySearchPath"
	```
4. `libraries/ghci/GHCi/InfoTable.hsc`:
    ```java
	foreign import ccall "&stg_interp_constr1_entry"
	foreign import ccall "&stg_interp_constr2_entry"
	foreign import ccall "&stg_interp_constr3_entry"
	foreign import ccall "&stg_interp_constr4_entry"
	foreign import ccall "&stg_interp_constr5_entry"
	foreign import ccall "&stg_interp_constr6_entry"
	foreign import ccall "&stg_interp_constr7_entry"
	foreign import ccall unsafe "allocateExec"
	foreign import ccall unsafe "flushExec"
	```
5. `libraries/ghci/GHCi/FFI.hsc`:
    ```java
	foreign import ccall "&ffi_type_void"
	foreign import ccall "&ffi_type_uint8"
	foreign import ccall "&ffi_type_sint8"
	foreign import ccall "&ffi_type_uint16"
	foreign import ccall "&ffi_type_sint16"
	foreign import ccall "&ffi_type_uint32"
	foreign import ccall "&ffi_type_sint32"
	foreign import ccall "&ffi_type_uint64"
	foreign import ccall "&ffi_type_sint64"
	foreign import ccall "&ffi_type_float"
	foreign import ccall "&ffi_type_double"
	foreign import ccall "&ffi_type_pointer"
	foreign import ccall "ffi_prep_cif"
	```

