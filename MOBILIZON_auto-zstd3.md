```
args:
  apps:
  - mobilizon
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-Mobilizon2
  output_directory: null
  system: null
ended_at: 2026-02-18 13:07:32.189662
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - mobilizon
started_at: 2026-02-18 13:06:24.114996
started_by: ******
success: true
yunohost_version: 12.1.39

============


 ------------------------------------------------------------------------------
                         BORG INFO AVANT   
 ------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               59.54 GB             58.01 GB             57.52 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   41233                42664

 ------------------------------------------------------------------------------
                         TIME BORG CREATE   
 ------------------------------------------------------------------------------
    Command being timed: "/var/www/borg/venv/bin/borg create --compression auto,zstd,3 --exclude-if-present .nobackup --stats ::test-Mobilizon2-{now} ."
 	User time (seconds): 35.65
 	System time (seconds): 4.86
 	Percent of CPU this job got: 67%
 	Elapsed (wall clock) time (h:mm:ss or m:ss): 1:00.47
 	Average shared text size (kbytes): 0
 	Average unshared data size (kbytes): 0
 	Average stack size (kbytes): 0
 	Average total size (kbytes): 0
 	Maximum resident set size (kbytes): 105096
 	Average resident set size (kbytes): 0
 	Major (requiring I/O) page faults: 0
 	Minor (reclaiming a frame) page faults: 38716
 	Voluntary context switches: 34022
 	Involuntary context switches: 518
 	Swaps: 0
 	File system inputs: 10960159
 	File system outputs: 5141000
 	Socket messages sent: 0
 	Socket messages received: 0
 	Signals delivered: 0
 	Page size (bytes): 4096
 	Exit status: 0


 ------------------------------------------------------------------------------
                         BORG INFO APRES   
 ------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               62.46 GB             60.62 GB             60.13 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   67902                69617



 ------------------------------------------------------------------------------
                         TIME GLOBAL   
 ------------------------------------------------------------------------------
    Command being timed: "sudo yunohost backup create -n test-Mobilizon2 --method borg_app --apps mobilizon"
	User time (seconds): 0.00
	System time (seconds): 0.00
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 1:08.28
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7680
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 794
	Voluntary context switches: 61
	Involuntary context switches: 6
	Swaps: 0
	File system inputs: 267
	File system outputs: 0
	Socket messages sent: 0
	Socket messages received: 0
	Signals delivered: 0
	Page size (bytes): 4096
	Exit status: 0


 ------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE MOBILIZON 2 auto,zstd,3
 ------------------------------------------------------------------------------
Time (start): Wed, 2026-02-18 13:06:30
Time (end): Wed, 2026-02-18 13:07:30
Duration: 59.46 seconds
Number of files: 26758
Command line: /var/www/borg/venv/bin/borg create --compression auto,zstd,3 --exclude-if-present .nobackup --stats '::test-Mobilizon2-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:                2.92 GB              2.61 GB              2.61 GB
All archives:               62.46 GB             60.62 GB             60.13 GB

                       Unique chunks         Total chunks
Chunk index:                   67902                69617
```
