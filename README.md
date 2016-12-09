# meta-adit
recipes for AGL CES demo 2017 to integrate AudioManager/GenericControllerPlugin

The meta-adit contains recipes for
- AudioManager
- AudioManagerPlugins
- AudioManagerPlugins Configuration
- router module for pulseaudio
- bbappend to add the Audiomanager and it's dependencies to the agl-demo-platform package group.

#### How to add this layer to AGL build
Add the meta-adit to the bblayer.conf file.  
Example: In build/conf/bblayer.conf add
BBLAYERS =+ "\  
    ${METADIR}/meta-renesas \  
    ${METADIR}/meta-renesas/meta-rcar-gen2 \  
\+  ${METADIR}/meta-adit/meta-adit \  
"

