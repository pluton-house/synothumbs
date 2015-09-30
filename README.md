# synothumbs
Uses your workstation to create thumbnails and previews for your photos and videos stored on your Synology PhotoStation.
##Dependencies
* python module [Pillow](https://github.com/python-pillow/Pillow) has to be available

##Important notice
* You have to mount the photo folder via **NFS and not SMB**! PhotoStation expects the thumbnails in a folder named @eaDir, this folder cannot be created or accessed via SMB.
* After creating the thumbnails and previews you have to re-index your media files (Control Panel - Media Indexing - Re-index).
* Especially for creating video previews and thumbnails a fast LAN connection is helpful as the complete file has to be read by your workstation.

##Information
Official settings for photo thumbnails can be found on your DiskStation in /usr/syno/etc.defaults/thumb.conf and /usr/syno/etc.defaults/thumb_high.conf. Don't know if something similar exists for video preview and thumbnails as well.
