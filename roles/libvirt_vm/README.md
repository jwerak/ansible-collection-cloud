Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

### Required Variables

- `libvirt_vm_images_path_source`: Path to source VM images directory (no default, MUST be provided)
- `libvirt_vm_name`: Name of the VM to create

### Optional Variables

- `libvirt_vm_hostname`: Hostname for the VM (default: 'linux')
- `libvirt_vm_disk_size`: Disk size in GB (default: 20)
- `libvirt_vm_vcpus`: Number of virtual CPUs (default: 2)
- `libvirt_vm_ram_mb`: RAM size in MB (default: 2048)
- `libvirt_vm_images_path_destination`: Destination path for VM images (default: '/var/lib/libvirt/images')
- `libvirt_vm_bridge`: Network bridge to use (default: 'bridge0')
- `libvirt_vm_osinfo`: OS information for the VM (optional)
- `libvirt_uri`: Libvirt connection URI (default: 'qemu:///system')

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
