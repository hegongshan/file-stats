### Command-line based File Statistics Tool (file-stats)

* Usage

```shell
$ ./file-stats -h
usage: file-stats [-h] -r ROOTDIR
                  [-s {type,perm,size,nlink,uid,gid,ctime,mtime,btime,ext,nfile,nline,nhidden,nblock} [{type,perm,size,nlink,uid,gid,ctime,mtime,btime,ext,nfile,nline,nhidden,nblock} ...]]
                  [-j [JOBS]] [-i] [-v] [-q] [--exclude-dirs EXCLUDE_DIRS] [--exclude-files EXCLUDE_FILES]
                  [--exclude-exts EXCLUDE_EXTS] [--exclude-pattern EXCLUDE_PATTERN]
                  [-H | -k | -m | -g | -t | -p | --si] [--size-range] [--per-file] [-n] [-f] [-o OUTPUT]
                  [-J | -C] [--plot-type {bar,pie,cdf}] [--plot-name PLOT_NAME]

file-stats - Command-line based File Statistics Tool

options:
  -h, --help            show this help message and exit
  -r ROOTDIR, --rootdir ROOTDIR
                        Root directory
  -s {type,perm,size,nlink,uid,gid,ctime,mtime,btime,ext,nfile,nline,nhidden,nblock} [{type,perm,size,nlink,uid,gid,ctime,mtime,btime,ext,nfile,nline,nhidden,nblock} ...], --stats {type,perm,size,nlink,uid,gid,ctime,mtime,btime,ext,nfile,nline,nhidden,nblock} [{type,perm,size,nlink,uid,gid,ctime,mtime,btime,ext,nfile,nline,nhidden,nblock} ...]
                        Stats type
  -j [JOBS], --jobs [JOBS]
                        Specify the number of jobs to run simultaneously
  -i, --ignore-hidden-file
                        Ignore hidden files
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
  -H, --human-readable  Human-readable output. Use unit suffixes: Byte, Kilobyte, Megabyte, Gigabyte,
                        Terabyte and Petabyte based on powers of 1024.
  -k, --ki              Use KiB
  -m, --mi              Use MiB
  -g, --gi              Use GiB
  -t, --ti              Use TiB
  -p, --pi              Use PiB
  --si                  Use international system of units (SI)
  --size-range          Show size range
  --per-file            Show the size of each file
  -n, --name            Show user name or group name
  -f, --full-path       Print the full path for each file
  -o OUTPUT, --output OUTPUT
                        Output file
  -J, --json            Export the results in JSON format.
  -C, --csv             Export the results in CSV format.
  --plot-type {bar,pie,cdf}
                        Specify the type of the figure
  --plot-name PLOT_NAME
                        Specify the name of the figure
```