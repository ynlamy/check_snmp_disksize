This plugin can check the disk size of Windows server and Unix server using SNMP v1 queries.

check_snmp_disksize is written in Bash and is distributed under the GPLv2 license. This plugin have been created by Yoann LAMY.

Usage: ./check_snmp_disksize -H 127.0.0.1 -C public -d C: -w 80 -c 90

-H ADDRESS
Name or IP address of host (default: 127.0.0.1)
-C STRING
Community name for the host's SNMP agent (default: public)
-d STRING
Drive letter (C:) or mount point (/home)
-w INTEGER
Warning level for size in percent (default: 0)
-c INTEGER
Critical level for size in percent (default: 0)
-h
Print this help screen
-V
Print version and license information

This plugin uses the 'snmpget' command and the 'snmpwalk' command included with the NET-SNMP package.
This plugin support performance data output. If the percentage of the warning and critical levels are set 0, then the script returns a OK state.

The nagios plugins come with ABSOLUTELY NO WARRANTY.

You may redistribute copies of the plugins under the terms of the GNU General Public License v2.
