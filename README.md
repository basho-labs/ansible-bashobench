basho-labs.bashobench
========

Configures basho_bench.

Requirements
------------

None

Role Variables
--------------


| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| benchmark_cluster_group | riak_cluster | group name of servers to target |
| bashobench_concurrent | 50 | number of concurrent connections |
| bashobench_duration | 30 | length of the test |
| bashobench_key_count | 1000000 | number of keys to write |
| bashobench_key_start_int | 0 | starting integer to count from |
| bashobench_keygen | partitioned_sequential_int | key generator to use |
| bashobench_operations | get | type of operations to use |
| bashobench_rate | max | rate to use |
| bashobench_set | test | name of the test suite |
| bashobench_value_bs | 1048576 | size of Riak CS object to use |
| riakcs_creds_path | /tmp/riakcs_creds.yml | path to riakcs creds |
| s3client_host_base | aws.amazon.com | basename to use for benchmark's s3 driver |
| s3client_proxy_port | 8080 | port number used to connect to s3 service |


Dependencies
------------

None

Example Playbook
-------------------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: bashobench
      roles:
         - basho-labs.bashobench

License
-------

Apache

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
