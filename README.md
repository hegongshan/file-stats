### Command-line based File Statistics Tool (file-stats)

* Usage

```shell
$ ./file-stats -h
usage: file-stats [-h] -r ROOTDIR
                  [-s {type,perm,size,nlink,uid,gid,ctime,mtime,btime,ext,nfile,nline,nhidden,nblock,archive,compress,encrypted,readonly,appendonly,executable} [{type,perm,size,nlink,uid,gid,ctime,mtime,btime,ext,nfile,nline,nhidden,nblock,archive,compress,encrypted,readonly,appendonly,executable} ...]]
                  [-j [JOBS]] [-i] [--detail] [-v] [-q] [--exclude-dirs EXCLUDE_DIRS]
                  [--exclude-files EXCLUDE_FILES] [--exclude-exts EXCLUDE_EXTS]
                  [--exclude-pattern EXCLUDE_PATTERN] [--raw | -H | -k | -m | -g | -t | -p] [--si]
                  [--size-range] [-n] [--symbol] [-f] [-o OUTPUT] [-J | -C | --plot-type {bar,pie,cdf}]

file-stats - Command-line based File Statistics Tool

options:
  -h, --help            show this help message and exit
  -r ROOTDIR, --rootdir ROOTDIR
                        Root directory
  -s {type,perm,size,nlink,uid,gid,ctime,mtime,btime,ext,nfile,nline,nhidden,nblock,archive,compress,encrypted,readonly,appendonly,executable} [{type,perm,size,nlink,uid,gid,ctime,mtime,btime,ext,nfile,nline,nhidden,nblock,archive,compress,encrypted,readonly,appendonly,executable} ...], --stats {type,perm,size,nlink,uid,gid,ctime,mtime,btime,ext,nfile,nline,nhidden,nblock,archive,compress,encrypted,readonly,appendonly,executable} [{type,perm,size,nlink,uid,gid,ctime,mtime,btime,ext,nfile,nline,nhidden,nblock,archive,compress,encrypted,readonly,appendonly,executable} ...]
                        Stats type
  -j [JOBS], --jobs [JOBS]
                        Specify the number of jobs to run simultaneously
  -i, --ignore-hidden-file
                        Ignore hidden files
  --detail              Show detail
  -v, --verbose         Verbose mode
  -q, --quiet           Quiet mode
  --exclude-dirs EXCLUDE_DIRS
                        Exclude dirs
  --exclude-files EXCLUDE_FILES
                        Exclude files
  --exclude-exts EXCLUDE_EXTS
                        Exclude file name extensions
  --exclude-pattern EXCLUDE_PATTERN
                        UNIX shell pattern
  --raw                 Do not show B unit suffix
  -H, --human-readable  Human-readable output.
  -k                    Use KiB, or KB with --si
  -m                    Use MiB, or MB with --si
  -g                    Use GiB, or GB with --si
  -t                    Use TiB, or TB with --si
  -p                    Use PiB, or PB with --si
  --si                  Use international system of units (SI)
  --size-range          Show size range
  -n, --name            Show user name or group name
  --symbol              Show symbolic permission
  -f, --full-path       Print the full path for each file
  -o OUTPUT, --output OUTPUT
                        Output file
  -J, --json            Export the results in JSON format.
  -C, --csv             Export the results in CSV format.
  --plot-type {bar,pie,cdf}
                        Specify the type of the figure
```