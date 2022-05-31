# cumulus

Cloud storage simplified

## Motivation

- Syncthing is great but does not allow for *anything* outside of its core use-case of fast synchronisation between multiple clients
- Nextcloud/Owncloud has poor performance and is very heavy if you're only interested in cloud storage
- Synology Drive works decently but is closed-source and vendor-locked
- Traditional cloud services have great clients but get expensive when storing multiple TBs of data and can't be run locally for high performance storage

## Features

- Resilient storage using multiple sources
  - Easily store multiple copies of your data: phone, local machine, local server, cloud, ...
  - Use local storage servers for increased performance
    - Compatible with ZFS snapshots for easy backups and restores
  - Delayed cloud backup options for reduced bandwidth usage
  - Define where each folder gets stored physically

- Virtual files support
  - Compatible with Windows' virtual files API for on-demand download and space saving

- Web UI, users management, and sharing
  - Data accessible through any web browser
  - Allocate storage to users and manage their access to different storage providers
  - Easily share files or folders with time-limited and access-limited links

- High performance
  - Syncthing-based P2P upload/download for compatible clients
  - Easily saturates gigabyte networks

- Graceful handling of regular uploads and files changes
  - No crashes even when saving heavy Premiere projects with it
  - Bin and local history

- Encryption support
  - Use Cloud services without compromising on privacy

- Compression support
  - Save space and bandwidth with `lz4` (and maybe `zstd` at a later date)

## Download

This project was started on May 31st 2022 and is very much in its early stage. My goal is to release a working alpha before the end of the year.
