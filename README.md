<<<<<<< HEAD
# .-cookbook

Zabbix agent for Windows

## Supported Platforms

Windows 2008
Windows 2012

## Attributes

<table>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td><tt>['.']['bacon']</tt></td>
    <td>Boolean</td>
    <td>whether to include bacon</td>
    <td><tt>true</tt></td>
  </tr>
</table>

## Usage

### .::default

Include `.` in your node's `run_list`:

```json
{
  "run_list": [
    "recipe[.::default]"
  ]
}
```

## License and Authors

Author:: Thomas Vincent (thomasvincent@gmail.com)
=======
Description
===========
Install the Zabbix agent on Windows machines.


Requirements
============
A Zabbix server is required for this to do anything useful.

Originally, I intended this to be added to Nacer Laradji's [Zabbix Cookbook](http://community.opscode.com/cookbooks/zabbix) ([github](https://github.com/laradji/zabbix)), but there were significant problems making it work this way.  (I believe that this is because there are problems in the dependancy chain that prevent this from working directly from the Zabbix cookbook; those cookbooks do not support the Windows platform.)

So, I present to you, a standalone recipe for installing the Zabbix Agent on your Windows hosts.


Attributes
==========
I am attempting to leverage the (mostly) standard attributes that I have included.

At this time, the actual files placed are version 2.0.3 and have been placed in the recipe manually.  Later I may have them fetched as remote_file with respect to the version


Usage
=====
Simply add the "Zabbix\_windows" recipe to a windows machine after establishing your Zabbix server and setting the Attributes as appropriate to your environment.
>>>>>>> eb5af0fab40c247110783ed782d0b0f13e5d9196
