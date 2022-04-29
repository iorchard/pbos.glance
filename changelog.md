# Changelog

## 1.0.2 - 2022-04-29

* Config: Modify glance-api.conf

  - set os_glance_tasks_store and os_glance_staging_store for multiple stores

* Tasks: Create oslo concurrency lock directory

  - create /var/lock/glance directory 

## 1.0.1 - 2022-04-08

* Config: Modify glance-api.conf

  - set show_image_direct_url to false b/c wallaby cinder and ceph pacific 
    has a problem when it is set to true.
  - removed the deprecated options - stores, default_store
  - added enabled_backends and default_backend
  - added rbd_thin_provisioning = True for ceph rbd backend
