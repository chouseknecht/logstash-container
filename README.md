# Role Name

Based on [geerlingguy.logstash](https://galaxy.ansible.com/geerlingguy/logstash), adds a logstash service to your [Ansible Container](https://github.com/ansible/ansible-container) project. 
Run the following commands to install the service:

```
# Set the working directory to your Ansible Container project root
$ cd myproject

# Install the service
$ ansible-container install chouseknecht.logstash-container
```

## Requirements

- [Ansible Container](https://github.com/ansible/ansible-container)
- An existing Ansible Container project. To create a project, simply run the following:
    ```
    # Create an empty project directory
    $ mkdir myproject

    # Set the working directory to the new directory
    $ cd myproject

    # Initialize the project
    $ ansible-contiainer init
    ```

- An elasticsearch service. Use [chouseknecht.logstash](https://galaxy.ansible.com/chouseknecht/elasticsearch-container), if you need to add one.

## Role Variables

logstash_elasticsearch_hosts: http://elasticsearch:9200 
> Specify the URL for accessing the Elasticsearch host.

logstash_listen_port_beats: 5044
> The port where the logstash service can be reached.

logstash_monitor_local_syslog: false 
logstash_local_syslog_path: /var/log/syslog
> Use these, if you want to monitor syslog for the logstash container.

logstash_ssl_dir: /etc/pki/logstash
logstash_ssl_certificate_file: ""
logstash_ssl_key_file: ""
> Use to configure SSL certificates.

logstash_install_plugins
> Provide a list of plugins you want installed.

## Dependencies

[geerlingguy.java](https://galaxy.ansible.com/geerlingguy/java)

## License

Apache v2

## Author Information

[@chouseknecht](https://github.com/chouseknecht)
