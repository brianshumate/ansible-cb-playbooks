# Ansible Couchbase Server Playbooks

These are random Ansible playbooks for use with Couchbase Server.

The playbooks perform time saving tasks focused on operating clusters for the
purposes of development and troubleshooting.


| Playbook | Description |
| -------- | ----------- |
| `_cb_dev_python_debian.yml` | installs Couchbase Python SDK environment for a Debian based cluster |
| `_cbcollect_deps.yml` | installs software dependencies for detailed output from the `cbcollect_info` utility |
| `_install_ssh_key.yml` | installs local user's SSH public key to the `authorized_keys` of specified cluster node user; **NOTE**: you must edit the token value *CHANGEME* in this playbook before use |
| `_install_static_config.yml` | installs an alternative `static_config` file; see `files/_example_static_config` for an example that sets all loglevel values to critical |
| `_libcouchbase.yml` | installs libcouchbase development packages |
| `_offline_upgrade.yml` | Performs an offline upgrade of cluster nodes |
| `_rebalance_test.yml` | Rebalance test scenario: Failover node *cb2*, rebalance cluster, and gather logs with `cbcollect_info` |
| `_test_cluster.yml` | Installs a test cluster, creates bucket, loads items |
| `_wipe_cluster.yml` | Uninstalls software, removes all data and configuration |
