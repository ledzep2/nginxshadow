Nginx Conf Shadow Tool
======================

This is a tool to switch nginx between different confs. Useful specially during site maintenance.

Install
-------

Change CONF_PATH in nginxshadow to your conf path before install. Then run

`setup.py install`


Usage
-----

### Create a named clone of origin nginx conf and change all listening ports. 

`nginxshadow create down --port 80`

This creates an conf clone named "down" and increase all listening port by 80. 

### Switch to a named conf

`nginxshadow switch down`   switch to "down"

`nginxshadow switch origin`     switch to "origin". this is the original conf

### Show current conf

`nginxshadow status`


