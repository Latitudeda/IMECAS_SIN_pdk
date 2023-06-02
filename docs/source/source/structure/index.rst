PDK structure
======================

Process Design Kit (PDK) is a tool for designated users to generate circuit layouts based on IMECAS SiN design rules and technology settings.

``IMECAS_SiN_pdk`` package includes four subfolders: ``components``, ``examples``, ``technology``, and ``util``.

* ``components``

    * BlackBox cells : All blackbox cells are named and designed by IMECAS and cannot be changed

    * Parametrized cells (PCells): Designed by **LDA**, including ``Bend``, ``Straight``. Please see ``gpdk > components`` for more designed components.

* ``examples``

    * ``MMItest`` : Test circuit to test if the blackbox cell (``SIN_MMI1X2_C``, ``SIN_FGC_TE_C``), auto routing, and auto link function works normally under the pdk setting. Please see ``gpdk > examples`` for more circuit examples.

* ``technology``

    * Store the technology setting which matched the IMECAS SiN design rules. We recommend users not to change the settings in technology folder.

    * See chapter ``Technology setting`` for more specific definition.

* ``util``

    * Useful functions when generating circuit layouts.

    * Please see **PhotoCAD** online manual for more information.

* ``layers.lyp`` : This file allows layout tools e.g. Klayout to recognize the layer information when displaying gds file to the layout tool.

    .. image:: ../images/lyp.png

