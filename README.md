# photosync

Sync photos from a digital camera or other external devices to a local computer while automatically organizing them and generating a static gallery website.

## Process

Main processes:

1. `photosync-watch` - the base process, watches for newly plugged in drives
2. `photosync-process` - mounts and checks drives that are intended to be processed
3. `photosync` - copies photos from one directory (ext. drive in this case) to a local folder

Helpers:

- `photosync-notify` - notifies about the process
- `photosync-gallery` - generates a static gallery website

## Dependencies

- `udisks2` - unprivileged device mounting
- `exiftool` - retrieving photo creation date
- `curl` - for notifications
- `docker` - for static gallery generation
