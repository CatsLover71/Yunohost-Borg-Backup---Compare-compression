```
https://paste.yunohost.org/raw/eyuruguluk

args:
  apps:
  - my_webapp
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-smallvideozstd3
  output_directory: null
  system: null
ended_at: 2026-02-21 14:03:52.399044
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - my_webapp
started_at: 2026-02-21 13:58:18.706397
started_by: ******
success: true
yunohost_version: 12.1.39

============


 ------------------------------------------------------------------------------
                         BORG INFO AVANT   
------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:                    0 B                  0 B                  0 B
 
                        Unique chunks         Total chunks
 Chunk index:                       0                    0

 ------------------------------------------------------------------------------
                         TIME BORG CREATE   
 ------------------------------------------------------------------------------
    Command being timed: "/var/www/borg/venv/bin/borg create --compression zstd,3 --exclude-if-present .nobackup --stats ::test-smallvideozstd3-{now} ."
 	User time (seconds): 266.19
 	System time (seconds): 30.55
 	Percent of CPU this job got: 89%
 	Elapsed (wall clock) time (h:mm:ss or m:ss): 5:29.98
 	Average shared text size (kbytes): 0
 	Average unshared data size (kbytes): 0
 	Average stack size (kbytes): 0
 	Average total size (kbytes): 0
 	Maximum resident set size (kbytes): 81216
 	Average resident set size (kbytes): 0
 	Major (requiring I/O) page faults: 0
 	Minor (reclaiming a frame) page faults: 374833
 	Voluntary context switches: 25252
 	Involuntary context switches: 4425
 	Swaps: 0
 	File system inputs: 54877536
 	File system outputs: 41636345
 	Socket messages sent: 0
 	Socket messages received: 0
 	Signals delivered: 0
 	Page size (bytes): 4096
 	Exit status: 0


------------------------------------------------------------------------------
                         BORG INFO APRES   
------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               21.65 GB             21.34 GB             21.32 GB
 
                        Unique chunks         Total chunks
 Chunk index:                    9545                 9590



------------------------------------------------------------------------------
                         TIME GLOBAL   
------------------------------------------------------------------------------
    Command being timed: "sudo yunohost backup create -n test-smallvideozstd3 --method borg_app --apps my_webapp"
	User time (seconds): 0.00
	System time (seconds): 0.00
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 5:33.88
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7296
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 798
	Voluntary context switches: 65
	Involuntary context switches: 3
	Swaps: 0
	File system inputs: 280
	File system outputs: 0
	Socket messages sent: 0
	Socket messages received: 0
	Signals delivered: 0
	Page size (bytes): 4096
	Exit status: 0


 ------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE SMALL VID zstd,3 
 ------------------------------------------------------------------------------
Time (start): Sat, 2026-02-21 13:58:21
Time (end): Sat, 2026-02-21 14:03:50
Duration: 5 minutes 28.90 seconds
Number of files: 1555
Command line: /var/www/borg/venv/bin/borg create --compression zstd,3 --exclude-if-present .nobackup --stats '::test-smallvideozstd3-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               21.65 GB             21.34 GB             21.31 GB
All archives:               21.65 GB             21.34 GB             21.32 GB

                       Unique chunks         Total chunks
Chunk index:                    9545                 9590
```
