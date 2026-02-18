
https://paste.yunohost.org/raw/favemoloqe

args:
  apps:
  - my_webapp
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-smallvideo1-bis
  output_directory: null
  system: null
ended_at: 2026-02-17 21:01:38.660994
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - my_webapp
started_at: 2026-02-17 20:57:08.889588
started_by: ******
success: true
yunohost_version: 12.1.39

============


 ------------------------------------------------------------------------------
                         BORG INFO AVANT   
 ------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               18.89 GB             17.59 GB             17.10 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   49743                51396

 ------------------------------------------------------------------------------
                         TIME BORG CREATE   
 ------------------------------------------------------------------------------
    Command being timed: "/var/www/borg/venv/bin/borg create --exclude-if-present .nobackup --stats ::test-smallvideo1-bis-{now} ."
 	User time (seconds): 206.53
 	System time (seconds): 30.02
 	Percent of CPU this job got: 88%
 	Elapsed (wall clock) time (h:mm:ss or m:ss): 4:26.02
 	Average shared text size (kbytes): 0
 	Average unshared data size (kbytes): 0
 	Average stack size (kbytes): 0
 	Average total size (kbytes): 0
 	Maximum resident set size (kbytes): 101004
 	Average resident set size (kbytes): 0
 	Major (requiring I/O) page faults: 2
 	Minor (reclaiming a frame) page faults: 68273
 	Voluntary context switches: 21401
 	Involuntary context switches: 4836
 	Swaps: 0
 	File system inputs: 54816676
 	File system outputs: 41975607
 	Socket messages sent: 0
 	Socket messages received: 0
 	Signals delivered: 0
 	Page size (bytes): 4096
 	Exit status: 0


-------------------------------------------------------------------------------
                         BORG INFO APRES   
-------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               40.54 GB             39.07 GB             38.56 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   59368                61064



------------------------------------------------------------------------------
                         TIME GLOBAL   
------------------------------------------------------------------------------
	Command being timed: "sudo yunohost backup create -n test-smallvideo1-bis --method borg_app --apps my_webapp"
	User time (seconds): 0.00
	System time (seconds): 0.00
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 4:29.96
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7424
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 792
	Voluntary context switches: 49
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
                       BORG INFO DE L'ARCHIVE SMALL-VIDEO lz4
 ------------------------------------------------------------------------------
Time (start): Tue, 2026-02-17 20:57:11
Time (end): Tue, 2026-02-17 21:01:35
Duration: 4 minutes 24.14 seconds
Number of files: 1555
Command line: /var/www/borg/venv/bin/borg create --exclude-if-present .nobackup --stats '::test-smallvideo1-bis-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               21.65 GB             21.48 GB             21.46 GB
All archives:               40.54 GB             39.07 GB             38.56 GB

                       Unique chunks         Total chunks
Chunk index:                   59368                61064

