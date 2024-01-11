# ConnMan
A Qt6-based graphical interface for managing remote file systems, which can be attached to the file system as a local folder. The program is one of the own developments of the blackPanther Project, but it is still in the testing phase, this is the first public version... We have already built in support for several file systems, but if you want something that is not yet included, feel free to write to the project's email address and we will incorporate it.

Remote storages mount to local filesystem with user rights via:
* [fuse](https://github.com/libfuse/libfuse)
* Gio for other method, ex: Samba
* OAuth for Google Drive
* etc

The operation is extremely simple. Add a connection with the add button, enter the address and login information (if any), save it, and simply click the connect button. The program saves the connections to an SQLite3 database.

# Supported protocols

## Currently working functions:

- BindFS - bind a folder to a new path / mirror it /
- LocalFS - mounting a local file system directory to another directory using a different method
- SshFS - mounting SSH server access to the local file system, requires enabling sftp on the SSH server
- NFS - mounting NFS-based sharing to the local file system
- FtpFS - mounting FTP file system to the local file system
- SmbNetFs - mounting Samba shares to the local file system
- Fuse-SMB - Another SAMBA support, does not work with some servers
- EncFS - Managing encrypted volumes
- DavFS - Mounting WebDav services to your local directory

## Not working yet, but built-in

- DavFS2 - Mounting WebDav services to your local directory
- WebDavFS - Managing WebDav shares (under testing)
- CmsFS - Mounting EDF file system
- Samba - Gio-based SAMBA share manager (in progress)

## Not yet built-in, but planned:

- ClusterFS - Managing Bigdata shares
- BtFs - Torrent file system support
- And more that we didn't even think of when writing the article 🙂 or whatever you want

# Other extras

- System tray icon
- Enable automatic startup
- Hidden start on system tray
- Automatic mounting at startup (not yet available)

# Install
Easy install on blackPanther OS

  (command for for English-speaking users)

  `installing blackPanther-connman`

  (command for Hungarian-speaking users)

  `telepites blackPanther-connman`

# Demo On Youtube
https://www.youtube.com/watch?v=iVt7WrvRpnk

# Screenshot
<img src=screenshots/ConnMan-screenshot.png size="90%">


