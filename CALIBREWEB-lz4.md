```
args:
  apps:
  - calibreweb
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-calibreweb1
  output_directory: null
  system: null
ended_at: 2026-02-14 17:19:07.736210
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - calibreweb
started_at: 2026-02-14 17:15:18.420955
started_by: ******
success: true
yunohost_version: 12.1.39

============


 ------------------------------------------------------------------------------
                         BORG INFO AVANT   
 ------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:                2.93 GB              2.68 GB              2.68 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   26726                27040

 ------------------------------------------------------------------------------
                         TIME BORG CREATE   
 ------------------------------------------------------------------------------
 	Command being timed: "/var/www/borg/venv/bin/borg create --exclude-if-present .nobackup --stats ::test-calibreweb1-{now} ."
 	User time (seconds): 149.39
 	System time (seconds): 24.43
 	Percent of CPU this job got: 77%
 	Elapsed (wall clock) time (h:mm:ss or m:ss): 3:45.05
 	Average shared text size (kbytes): 0
 	Average unshared data size (kbytes): 0
 	Average stack size (kbytes): 0
 	Average total size (kbytes): 0
 	Maximum resident set size (kbytes): 114596
 	Average resident set size (kbytes): 0
 	Major (requiring I/O) page faults: 5
 	Minor (reclaiming a frame) page faults: 491666
 	Voluntary context switches: 28890
 	Involuntary context switches: 2593
 	Swaps: 0
 	File system inputs: 38515863
 	File system outputs: 28206907
 	Socket messages sent: 0
 	Socket messages received: 0
 	Signals delivered: 0
 	Page size (bytes): 4096
 	Exit status: 0


 ------------------------------------------------------------------------------
                         BORG INFO APRES   
 ------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               18.90 GB             17.59 GB             17.10 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   49718                51403



------------------------------------------------------------------------------
                         TIME GLOBAL   
------------------------------------------------------------------------------
	Command being timed: "sudo yunohost backup create -n test-calibreweb1 --method borg_app --apps calibreweb"
	User time (seconds): 0.00
	System time (seconds): 0.00
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 4:02.09
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7424
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 11
	Minor (reclaiming a frame) page faults: 801
	Voluntary context switches: 82
	Involuntary context switches: 4
	Swaps: 0
	File system inputs: 1289
	File system outputs: 0
	Socket messages sent: 0
	Socket messages received: 0
	Signals delivered: 0
	Page size (bytes): 4096
	Exit status: 0


 ------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE CALIBREWEB 1 lz4
 ------------------------------------------------------------------------------
Time (start): Sat, 2026-02-14 17:15:21
Time (end): Sat, 2026-02-14 17:19:04
Duration: 3 minutes 42.47 seconds
Number of files: 18795
Command line: /var/www/borg/venv/bin/borg create --exclude-if-present .nobackup --stats '::test-calibreweb1-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               15.97 GB             14.91 GB             14.42 GB
All archives:               18.90 GB             17.59 GB             17.10 GB

                       Unique chunks         Total chunks
Chunk index:                   49746                51432
```
