```
args:
  apps:
  - funkwhale
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-funkwhale2
  output_directory: null
  system: null
ended_at: 2026-02-18 13:20:56.538435
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - funkwhale
started_at: 2026-02-18 13:17:37.290627
started_by: ******
success: true
yunohost_version: 12.1.39

============

 ------------------------------------------------------------------------------
                         BORG INFO AVANT   
 ------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               62.46 GB             60.62 GB             60.13 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   67902                69617

 ------------------------------------------------------------------------------
                         TIME BORG CREATE   
 ------------------------------------------------------------------------------
    Command being timed: "/var/www/borg/venv/bin/borg create --compression auto,zstd,3 --exclude-if-present .nobackup --stats ::test-funkwhale2-{now} ."
 	User time (seconds): 144.23
 	System time (seconds): 19.47
 	Percent of CPU this job got: 84%
 	Elapsed (wall clock) time (h:mm:ss or m:ss): 3:13.80
 	Average shared text size (kbytes): 0
 	Average unshared data size (kbytes): 0
 	Average stack size (kbytes): 0
 	Average total size (kbytes): 0
 	Maximum resident set size (kbytes): 114444
 	Average resident set size (kbytes): 0
 	Major (requiring I/O) page faults: 0
 	Minor (reclaiming a frame) page faults: 41203
 	Voluntary context switches: 40527
 	Involuntary context switches: 2171
 	Swaps: 0
 	File system inputs: 36996853
 	File system outputs: 23617594
 	Socket messages sent: 0
 	Socket messages received: 0
 	Signals delivered: 0
 	Page size (bytes): 4096
 	Exit status: 0


 ------------------------------------------------------------------------------
                         BORG INFO APRES   
 ------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               75.74 GB             72.93 GB             72.19 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   95461               102593



 ------------------------------------------------------------------------------
                         TIME GLOBAL   
 ------------------------------------------------------------------------------
    Command being timed: "sudo yunohost backup create -n test-funkwhale2 --method borg_app --apps funkwhale"
	User time (seconds): 0.00
	System time (seconds): 0.00
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 3:19.44
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7552
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 794
	Voluntary context switches: 66
	Involuntary context switches: 2
	Swaps: 0
	File system inputs: 283
	File system outputs: 0
	Socket messages sent: 0
	Socket messages received: 0
	Signals delivered: 0
	Page size (bytes): 4096
	Exit status: 0


 ------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE FUNKWHALE 2 auto,zstd,3
 ------------------------------------------------------------------------------
Time (start): Wed, 2026-02-18 13:17:41
Time (end): Wed, 2026-02-18 13:20:54
Duration: 3 minutes 12.62 seconds
Number of files: 28989
Command line: /var/www/borg/venv/bin/borg create --compression auto,zstd,3 --exclude-if-present .nobackup --stats '::test-funkwhale2-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               13.27 GB             12.30 GB             12.06 GB
All archives:               75.74 GB             72.93 GB             72.19 GB

                       Unique chunks         Total chunks
Chunk index:                   95461               102593
```
