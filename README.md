# DNXSpelunking

##DNVM

The Dot Net Version Manager.

Written in powershell. Lives in %USERPROFILE%\.dnx\bin\dnvm.ps1. Called from dnvm.cmd in the same directory.

### dnvm alias

Reads, writes, deletes aliases. Aliases live in %USERPROFILE%\.dnx\alias. They are textfiles where the name of the textfile is the alias with .txt appended. The contents of the textfile is the value of the alias - the CLR.

```dnvm alias```

Shows all aliases. Usually, there is just a single alias - default. These are the filenames (or directory names!) in the .dnx\alias folder.

```dnvm alias a b```

Creates alias\a.txt with contents 'b'

```dnvm alias a 123```

Creates alias\a.txt with contents of the current CLR with .123 appended

```dnvm alias a```

Shows the value of the alias a

```dnvm alias a -delete```

Deletes the alias a

```dnvm alias com1 abc```

Exception about Win32 devices

````dnvm alias ab\c test```

Will create the alias only if the directory alias\ab exists.

