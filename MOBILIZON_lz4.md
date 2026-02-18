```
args:
  apps:
  - mobilizon
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-mobilizon1
  output_directory: null
  system: null
ended_at: 2026-02-14 16:52:26.496935
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - mobilizon
started_at: 2026-02-14 16:51:24.123055
started_by: ******
success: true
yunohost_version: 12.1.39

============


 ------------------------------------------------------------------------------
                         BORG INFO AVANT   
 ------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:                7.54 MB              3.24 MB              1.63 MB
 
                        Unique chunks         Total chunks
 Chunk index:                      39                   72
 
 ------------------------------------------------------------------------------
                         TIME BORG CREATE   
 ------------------------------------------------------------------------------
 	Command being timed: "/var/www/borg/venv/bin/borg create --exclude-if-present .nobackup --stats ::test-mobilizon1-{now} ."
 	User time (seconds): 30.32
 	System time (seconds): 4.37
 	Percent of CPU this job got: 62%
 	Elapsed (wall clock) time (h:mm:ss or m:ss): 0:55.78
 	Average shared text size (kbytes): 0
 	Average unshared data size (kbytes): 0
 	Average stack size (kbytes): 0
 	Average total size (kbytes): 0
 	Maximum resident set size (kbytes): 101972
 	Average resident set size (kbytes): 0
 	Major (requiring I/O) page faults: 0
 	Minor (reclaiming a frame) page faults: 38180
 	Voluntary context switches: 23349
 	Involuntary context switches: 165
 	Swaps: 0
 	File system inputs: 10961098
 	File system outputs: 5245709
 	Socket messages sent: 0
 	Socket messages received: 0
 	Signals delivered: 0
 	Page size (bytes): 4096
 	Exit status: 0


 ------------------------------------------------------------------------------
                         BORG INFO APRES   
 ------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:                2.93 GB              2.68 GB              2.68 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   26726                27040



 ------------------------------------------------------------------------------
                         TIME GLOBAL   
 ------------------------------------------------------------------------------
    Command being timed: "sudo yunohost backup create -n test-mobilizon1 --method borg_app --apps mobilizon"
	User time (seconds): 0.00
	System time (seconds): 0.01
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 1:02.55
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7552
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 800
	Voluntary context switches: 68
	Involuntary context switches: 3
	Swaps: 0
	File system inputs: 264
	File system outputs: 0
	Socket messages sent: 0
	Socket messages received: 0
	Signals delivered: 0
	Page size (bytes): 4096
	Exit status: 0


 ------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE MOBILIZON 1 lz4
 ------------------------------------------------------------------------------
Time (start): Sat, 2026-02-14 16:51:30
Time (end): Sat, 2026-02-14 16:52:23
Duration: 53.72 seconds
Number of files: 26758
Command line: /var/www/borg/venv/bin/borg create --exclude-if-present .nobackup --stats '::test-mobilizon1-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:                2.92 GB              2.68 GB              2.67 GB
All archives:               18.90 GB             17.59 GB             17.10 GB

                       Unique chunks         Total chunks
Chunk index:                   49746                51432
```
