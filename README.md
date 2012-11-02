# collectd-puppet-reports

collectd module to gather metrics from puppet reports.

## Prerequisite

* A collectd installation with python support
* The python pyyaml library installed
* Puppet agents with reporting enabled

## Configuration

```
<LoadPlugin python>
    Globals true
</LoadPlugin>

<Plugin python>
  <Module puppet-reports>
    ReportsDir "/var/lib/puppet/reports"
  </Module>
</Plugin>
```
	