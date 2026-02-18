```
args:
  apps:
  - my_webapp
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-smallvideo2BIS
  output_directory: null
  system: null
ended_at: 2026-02-18 11:37:40.870917
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - my_webapp
started_at: 2026-02-18 11:33:01.009064
started_by: ******
success: true
yunohost_version: 12.1.39

============


 ------------------------------------------------------------------------------
                         BORG INFO AVANT   
 ------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:                3.82 MB              1.64 MB              1.65 MB
 
                        Unique chunks         Total chunks
 Chunk index:                      63                   64

 ------------------------------------------------------------------------------
                         TIME BORG CREATE   
 ------------------------------------------------------------------------------
    Command being timed: "/var/www/borg/venv/bin/borg create --compression auto,zstd,3 --exclude-if-present .nobackup --stats ::test-smallvideo2BIS-{now} ."
 	User time (seconds): 212.73
 	System time (seconds): 29.07
 	Percent of CPU this job got: 87%
 	Elapsed (wall clock) time (h:mm:ss or m:ss): 4:36.23
 	Average shared text size (kbytes): 0
 	Average unshared data size (kbytes): 0
 	Average stack size (kbytes): 0
 	Average total size (kbytes): 0
 	Maximum resident set size (kbytes): 81528
 	Average resident set size (kbytes): 0
 	Major (requiring I/O) page faults: 0
 	Minor (reclaiming a frame) page faults: 466790
 	Voluntary context switches: 24086
 	Involuntary context switches: 3691
 	Swaps: 0
 	File system inputs: 54856208
 	File system outputs: 41883434
 	Socket messages sent: 0
 	Socket messages received: 0
 	Signals delivered: 0
 	Page size (bytes): 4096
 	Exit status: 0


-------------------------------------------------------------------------------
                         BORG INFO APRES   
-------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               21.65 GB             21.46 GB             21.44 GB
 
                        Unique chunks         Total chunks
 Chunk index:                    9673                 9708



------------------------------------------------------------------------------
                         TIME GLOBAL   
------------------------------------------------------------------------------
    Command being timed: "sudo yunohost backup create -n test-smallvideo2BIS --method borg_app --apps my_webapp"
	User time (seconds): 0.00
	System time (seconds): 0.01
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 4:40.04
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7680
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 796
	Voluntary context switches: 58
	Involuntary context switches: 1
	Swaps: 0
	File system inputs: 283
	File system outputs: 0
	Socket messages sent: 0
	Socket messages received: 0
	Signals delivered: 0
	Page size (bytes): 4096
	Exit status: 0


 ------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE SMALL-VIDEO auto,zstd,3
 ------------------------------------------------------------------------------
Time (start): Wed, 2026-02-18 11:33:03
Time (end): Wed, 2026-02-18 11:37:39
Duration: 4 minutes 35.40 seconds
Number of files: 1555
Command line: /var/www/borg/venv/bin/borg create --compression auto,zstd,3 --exclude-if-present .nobackup --stats '::test-smallvideo2BIS-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               21.65 GB             21.45 GB             21.44 GB
All archives:               21.65 GB             21.46 GB             21.44 GB

                       Unique chunks         Total chunks
Chunk index:                    9673                 9708
```
