# Role Name

Adds a logstash service to your [Ansible Container](https://github.com/ansible/ansible-container) project. Run the following commands
to install the service:

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

??

## Dependencies

[chouseknecht.logstash](https://galaxy.ansible.com/chouseknecht/logstash)

## License

Apache v2

## Author Information

[@chouseknecht](https://github.com/chouseknecht)
