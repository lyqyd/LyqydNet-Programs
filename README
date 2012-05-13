LyqydNet-Programs
=================

A collection of ComputerCraft programs using the LyqydNet API for
client-server interactions.

1 - FileD

FileD is the file daemon.  All files stored on the machine running it
are contained in a folder called "share".  This is to provide some
measure of protection against persons trying to upload malicious startup
files, for example. FileD accepts the following message types:

- query: a string is required, but not specified. Suggest using
	"connect"
- data: used for the 'cd' command. Format should be:
	filed;cd <directory>
	'filed;' is usually prepended by the connection API, so the client
	program may send just the 'cd <directory>' string.
- fileList
- fileCopy
- fileMove
- fileDelete
- fileMakeDirectory
- fileQuery
- fileSend
- fileHeader
- fileData
- fileEnd
- close

See the LyqydNet API documentation for more information on the file
transfer protocol packets.

2 - FileC

FileC is the file transfer client. It may be started with no options or
a single option specifying the name of a server to connect to. The
commands available in the client are:

- ls: lists remote files
- cd: changes remote directory
- cp: copies remote files to other remote locations
- mv: moves remote files to other remote locations
- mkdir: creates a remote directory
- rm: removes a remote file
- get: copies a remote file to a local file
- put: copies a local file to a remote file
- open: opens a connection to a server
- close: closes the connection to the server
- exit: closes the open connection if any, then exits the client.