```
args:
  apps:
  - my_webapp__2
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-Bigvideo1
  output_directory: null
  system: null
ended_at: 2026-02-18 09:11:54.781078
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - my_webapp__2
started_at: 2026-02-18 09:07:27.266200
started_by: ******
success: true
yunohost_version: 12.1.39

============


 ------------------------------------------------------------------------------
                         BORG INFO AVANT   
 ------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               40.54 GB             39.07 GB             38.56 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   59368                61064

 ------------------------------------------------------------------------------
                         TIME BORG CREATE   
 ------------------------------------------------------------------------------
    Command being timed: "/var/www/borg/venv/bin/borg create --exclude-if-present .nobackup --stats ::test-Bigvideo1-{now} ."
 	User time (seconds): 209.40
 	System time (seconds): 35.67
 	Percent of CPU this job got: 93%
 	Elapsed (wall clock) time (h:mm:ss or m:ss): 4:23.44
 	Average shared text size (kbytes): 0
 	Average unshared data size (kbytes): 0
 	Average stack size (kbytes): 0
 	Average total size (kbytes): 0
 	Maximum resident set size (kbytes): 101500
 	Average resident set size (kbytes): 0
 	Major (requiring I/O) page faults: 0
 	Minor (reclaiming a frame) page faults: 1246764
 	Voluntary context switches: 13621
 	Involuntary context switches: 5704
 	Swaps: 0
 	File system inputs: 49537497
 	File system outputs: 42868995
 	Socket messages sent: 0
 	Socket messages received: 0
 	Signals delivered: 0
 	Page size (bytes): 4096
 	Exit status: 0


-------------------------------------------------------------------------------
                         BORG INFO APRES   
-------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               62.46 GB             60.99 GB             60.48 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   67964                69683



------------------------------------------------------------------------------
                         TIME GLOBAL   
------------------------------------------------------------------------------
	Command being timed: "sudo yunohost backup create -n test-Bigvideo1 --method borg_app --apps my_webapp__2"
	User time (seconds): 0.00
	System time (seconds): 0.00
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 4:27.73
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7552
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 797
	Voluntary context switches: 64
	Involuntary context switches: 1
	Swaps: 0
	File system inputs: 267
	File system outputs: 0
	Socket messages sent: 0
	Socket messages received: 0
	Signals delivered: 0
	Page size (bytes): 4096
	Exit status: 0


 ------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE BIG-VIDEO lz4
 ------------------------------------------------------------------------------
Time (start): Wed, 2026-02-18 09:07:30
Time (end): Wed, 2026-02-18 09:11:52
Duration: 4 minutes 21.99 seconds
Number of files: 34
Command line: /var/www/borg/venv/bin/borg create --exclude-if-present .nobackup --stats '::test-Bigvideo1-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               21.92 GB             21.92 GB             21.92 GB
All archives:               62.46 GB             60.99 GB             60.48 GB

                       Unique chunks         Total chunks
Chunk index:                   67964                69683
```
