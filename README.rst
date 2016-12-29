=====================
zbackup
=====================
freebsd zfs auto backup daemon written in Python3.5 with coroutine 


Usage
===================
put ``zbackup`` in ``/usr/local/bin`` and rename ``zbackup.rc`` to ``zbackup`` and put it inside ``/usr/local/etc/rc.d``.
And put ``zbackup.conf`` to where your ``zbackup_config``, which is in ``rc.conf``, point to. And don't forget ``zbackup_enable="YES"``
in ``rc.conf``.


::
   
   usage: ./zbackup [[--list | --delete] target dataset [ID] | target dataset [rotation count]] | -d  [-c ConfigFile]
   
   zfs backup, if no addition argument, create snapshot

   optional arguments:
   -h, --help            show this help message and exit
   
   --delete              delete snapshot
   --list                list snapshot
   dataset               target dataset
   rotation              specify ID or rotation number

   -d, --daemon          start daemon mode
   -c [CONFIG], --config [CONFIG]
                         config file of daemon mode





			     
