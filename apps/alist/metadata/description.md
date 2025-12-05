# Alist

**A file list program that supports multiple storage backends.**

Alist is a powerful, open-source file management tool that aggregates various storage services into a single, unified interface. It allows you to access, manage, and preview files from local storage, cloud drives, and remote servers all in one place.

### Key Features

* **Unified Management:** Manage files from different cloud providers (Google Drive, OneDrive, S3, etc.) and local storage in a single dashboard.
* **WebDAV Support:** Seamlessly mount your storage as a local drive on your computer using the standard WebDAV protocol.
* **File Previews:** Built-in preview support for videos, audio, images, PDF, Markdown, and Office documents.
* **Offline Download:** Supports offline downloading to your storage backends.
* **Privacy & Security:** Features password protection for specific folders and supports guest user restrictions.
* **Cross-Platform:** Works on all major operating systems and devices via a responsive web interface.

### Supported Storage Providers

Alist supports a vast array of storage backends, including but not limited to:
* **Local Storage**
* **SMB / FTP / SFTP**
* **WebDAV**
* **Object Storage:** Amazon S3, MinIO, Cloudflare R2, Backblaze B2
* **Cloud Drives:** Google Drive, OneDrive, Dropbox, Box, Yandex.Disk, MEGA
* **Others:** Alias, Aliyun Drive, Baidu Netdisk, Quark, PikPak, and many more.

### Default Login
When the container starts for the first time, you can view the randomly generated admin password in the container logs:
`docker logs alist`