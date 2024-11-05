if(WITH_PYTHON)
    include_directories(${PYTHON_INCLUDE_DIRS})
    
    calamares_add_plugin(mkinitcpio
        TYPE job
        EXPORT_MACRO PLUGINDLLEXPORT_PRO
        SOURCES
            Module.cpp
            main.py
        SHARED_LIB
        NO_INSTALL
    )
    
    install(FILES
        main.py
        module.desc
        DESTINATION ${CALAMARES_PLUGINDIR}/mkinitcpio
    )
endif()
