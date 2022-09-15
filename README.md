mkdldir
=======

```
mkdldir 1.1.0

USAGE: mkdldir [-ahiprtuv] <outputdir>

Create download directory for Apache HTTP Server.

Directory will be created in <outputdir>. It can be protected using HTTP Digest
with a pair of .htdigest and .htaccess files.

OPTIONS:

	-a        Specify absolute path base to .htaccess file to use.
	          Path will become <pathbase>/<outputdir>/.htaccess.
	          If not specified, will only <outputdir>/.htaccess.
	          (Note AuthUserFile in .htaccess cannot be relative.)
	-h        Show this help screen.
	-i        Make directory private by protecting it with HTTP Digest auth.
	-p        Specify password for digest authentication. Implies -i.
	-r        Specify realm for digest authentication. Implies -i.
	          Will use title (-t) if not specified.
	-t        Specify title for directory. (Default: Download)
	-u        Specify username for digest password. Implies -i.
	          (Default: download)
	-v        Show script name and version number.

```