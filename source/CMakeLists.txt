
add_library(gothic3sdk STATIC)

target_sources(gothic3sdk PRIVATE
    ${CMAKE_CURRENT_LIST_DIR}/Engine/ge_dx9instance.cpp
    ${CMAKE_CURRENT_LIST_DIR}/Game/ge_scriptadmin.cpp
    ${CMAKE_CURRENT_LIST_DIR}/Game/ge_scriptinit.cpp
    ${CMAKE_CURRENT_LIST_DIR}/Script/gs_propertymacros.inl
    ${CMAKE_CURRENT_LIST_DIR}/Script/gs_psitemwrapper.cpp
    ${CMAKE_CURRENT_LIST_DIR}/Script/gs_scriptargs.cpp
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_arraybase.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_auto_po_smartptr.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_autoptrarray.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_classnamebase.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_delegatebase.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_enumwrapper.cpp
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_enumwrapper.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_objarray.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_objarraysort.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_objstack.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_po_puresmartptr.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_propertycontainer.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_propertyobject.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_propertyobjecttype.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_propertytype.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_propertytypeonly.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_ptrarray.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_ptrarraysort.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_set.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_smallarray.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_streamutil.cpp
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_valarray.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_valmap.inl
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase/ge_volume.inl
    ${CMAKE_CURRENT_LIST_DIR}/Engine.cpp
    ${CMAKE_CURRENT_LIST_DIR}/GFC.cpp
    ${CMAKE_CURRENT_LIST_DIR}/Importer.cpp
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase.cpp
)

target_include_directories(gothic3sdk PUBLIC
    ${CMAKE_CURRENT_LIST_DIR}
    ${CMAKE_CURRENT_LIST_DIR}/Engine
    ${CMAKE_CURRENT_LIST_DIR}/Game
    ${CMAKE_CURRENT_LIST_DIR}/GFC
    ${CMAKE_CURRENT_LIST_DIR}/Importer
    ${CMAKE_CURRENT_LIST_DIR}/Script
    ${CMAKE_CURRENT_LIST_DIR}/SharedBase
)