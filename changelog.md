# Changelog

## 1.0.1 - 2022-04-20

* Config: Modify glance-api.conf

  - set show_image_direct_url to false b/c wallaby cinder and ceph pacific 
    has a problem when it is set to true.
  - removed the deprecated options - stores, default_store
  - added enabled_backends and default_backend
  - added rbd_thin_provisioning = True for ceph rbd backend
