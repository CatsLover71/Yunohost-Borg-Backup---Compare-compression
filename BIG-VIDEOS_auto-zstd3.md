```
args:
  apps:
  - my_webapp__2
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-bigvideo2
  output_directory: null
  system: null
ended_at: 2026-02-18 12:38:32.414956
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - my_webapp__2
started_at: 2026-02-18 12:34:12.526564
started_by: ******
success: true
yunohost_version: 12.1.39

============


------------------------------------------------------------------------------
                         BORG INFO AVANT   
------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               21.65 GB             21.46 GB             21.44 GB
 
                        Unique chunks         Total chunks
 Chunk index:                    9673                 9708

 ------------------------------------------------------------------------------
                         TIME BORG CREATE   
 ------------------------------------------------------------------------------
    Command being timed: "/var/www/borg/venv/bin/borg create --compression auto,zstd,3 --exclude-if-present .nobackup --stats ::test-bigvideo2-{now} ."
 	User time (seconds): 201.85
 	System time (seconds): 33.61
 	Percent of CPU this job got: 91%
 	Elapsed (wall clock) time (h:mm:ss or m:ss): 4:16.21
 	Average shared text size (kbytes): 0
 	Average unshared data size (kbytes): 0
 	Average stack size (kbytes): 0
 	Average total size (kbytes): 0
 	Maximum resident set size (kbytes): 84228
 	Average resident set size (kbytes): 0
 	Major (requiring I/O) page faults: 0
 	Minor (reclaiming a frame) page faults: 33525
 	Voluntary context switches: 13482
 	Involuntary context switches: 4194
 	Swaps: 0
 	File system inputs: 49241348
 	File system outputs: 42825998
 	Socket messages sent: 0
 	Socket messages received: 0
 	Signals delivered: 0
 	Page size (bytes): 4096
 	Exit status: 0


-------------------------------------------------------------------------------
                         BORG INFO APRES   
-------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               43.57 GB             43.38 GB             43.36 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   18171                18229



------------------------------------------------------------------------------
                         TIME GLOBAL   
------------------------------------------------------------------------------
    Command being timed: "sudo yunohost backup create -n test-bigvideo2 --method borg_app --apps my_webapp__2"
	User time (seconds): 0.00
	System time (seconds): 0.01
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 4:20.08
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7552
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 796
	Voluntary context switches: 83
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
                       BORG INFO DE L'ARCHIVE BIG-VIDEO2 auto,zstd,3
 ------------------------------------------------------------------------------
Time (start): Wed, 2026-02-18 12:34:15
Time (end): Wed, 2026-02-18 12:38:30
Duration: 4 minutes 14.54 seconds
Number of files: 34
Command line: /var/www/borg/venv/bin/borg create --compression auto,zstd,3 --exclude-if-present .nobackup --stats '::test-bigvideo2-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               21.92 GB             21.92 GB             21.92 GB
All archives:               43.57 GB             43.38 GB             43.36 GB

                       Unique chunks         Total chunks
Chunk index:                   18171                18229
```
