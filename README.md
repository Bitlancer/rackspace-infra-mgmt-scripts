# Rackspace Infrastructure Management Scripts

A series of scripts for managing Rackspace infrastructure that utilizes Puppet for configuration management.

| Script                 | Functionality
|------------------------|----------------------------------------- 
| infra_bootstrap        | Provision a VM, schedule daily images, create DNS records, bootstrap Puppet
| infra_delete           | Delete a VM and cleanup the node within Puppet
| inra_list              | List the instances joined to the Puppet master including attributes (utilizes PuppetDB data)
| infra_upgrade          | To assist with patching
| run_r10k               | Run r10k (provision Puppet environments, update Puppet modules, deploy Hiera data)

## Requirements

This is meant to be run on the Puppet master.

* PHP >= 5.3
* PHP-CURL

## Install

Copy the config file `conf/infra-mgmt-config-sample` to `~/.infra-mgmt-config` and
update settings as needed.

