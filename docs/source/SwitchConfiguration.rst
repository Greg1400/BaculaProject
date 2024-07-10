.. _Switch:

Switch Configuration
====================

.. _mainconfiguration:
First Configuration
~~~~~~~~~~~~~~~~~~

#. Connect to the switch by connecting to ``port 1``

#. Open a Command Prompt

#. 

.. code-block:: console

    C:\\Users\\GHERZIG> telnet 192.168.1.254

#. On the "Login Screen" enter the following credential
``User Name:`` = ``admin`` - ``Password:`` = ``admin``

.. _ourconfiguration:
Our configuration
~~~~~~~~~~~~~~~~~~

(credentials)=

``User Name`` = administrator
``Password`` = L4TLinksys

#. Go under ``1.System Configuration Menu``
#. ``6.IP Configuration`` > ``1. IPv4 Configuration`` > ``1. Ipv4 Address Settings``

.. code-block:: telnet                         

                          IPv4 Address - Configuration
                         ============================


                      IPv4 Address:         192.168.1.254

                      Subnet Mask:          255.255.255.0

                      Default Gateway:      0.0.0.0

                      Management VLAN:      1    VLAN ID

                      DHCP Client:          DISABLE


That's all we can do from telnet or SSH. To go to further settings, we should pass to browser. Use ``Microsoft Edge`` in ``Explorer mode``


.. _explorermode:
Turning to Explorer mode
------------------------

Open Microsoft Edge and click on the 3 ". . ." up right. Go to ``Settings`` > ``Default Browser``. 

#. Under ``Internet Explorer compatibility``
  #. ``Allow site to be reloaded in Internet Explorer mode (IE mode)`` : Allow
  #. ``Internet Explorer mode pages`` : Add
    #. Enter the URL of the switch = ``http://192.168.1.254/``
#. Close and reopen MS Edge and go to the address of the switch

#. You will perhaps have to accept to reload in IE mode
#. Now, you're able to connect through the web to the Switch Configuration with the `credentials <credentials>`_ above.

.. note::
    ``Startup Configuration File`` and ``Running Configuration File`` are different. 
    In order to have the configuration you've made as the startup, do the following steps:
    #. Go to ``Admin`` panel

    #. ``File Management``

    #. ``Copy Files``

    #. Click on ``Copy Configuration``

        #. ``Source File Name`` : Running Configuration

        #. ``Destination File Name`` : Startup Configuration
