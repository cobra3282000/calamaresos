calamares_add_plugin(mkinitcpio
    TYPE job
    EXPORT_MACRO PLUGINDLLEXPORT_PRO
    SOURCES
        main.py
    SHARED_LIB
)
