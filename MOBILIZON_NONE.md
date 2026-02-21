```
https://paste.yunohost.org/raw/irezomotef

args:
  apps:
  - mobilizon
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-mobilizonnone
  output_directory: null
  system: null
ended_at: 2026-02-21 16:53:17.867999
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - mobilizon
started_at: 2026-02-21 16:52:14.413158
started_by: ******
success: true
yunohost_version: 12.1.39

============

------------------------------------------------------------------------------
                         BORG INFO AVANT   
------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               59.54 GB             59.54 GB             59.02 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   41221                42618


 ------------------------------------------------------------------------------
                         TIME BORG CREATE   
 ------------------------------------------------------------------------------
    Command being timed: "/var/www/borg/venv/bin/borg create --compression none --exclude-if-present .nobackup --stats ::test-mobilizonnone-{now} ."
 	User time (seconds): 29.69
 	System time (seconds): 5.88
 	Percent of CPU this job got: 63%
 	Elapsed (wall clock) time (h:mm:ss or m:ss): 0:56.37
 	Average shared text size (kbytes): 0
 	Average unshared data size (kbytes): 0
 	Average stack size (kbytes): 0
 	Average total size (kbytes): 0
 	Maximum resident set size (kbytes): 107996
 	Average resident set size (kbytes): 0
 	Major (requiring I/O) page faults: 0
 	Minor (reclaiming a frame) page faults: 47239
 	Voluntary context switches: 29059
 	Involuntary context switches: 391
 	Swaps: 0
 	File system inputs: 11049050
 	File system outputs: 5752704
 	Socket messages sent: 0
 	Socket messages received: 0
 	Signals delivered: 0
 	Page size (bytes): 4096
 	Exit status: 0


------------------------------------------------------------------------------
                         BORG INFO APRES   
------------------------------------------------------------------------------
2026-02-21 16:53:17,167: DEBUG -                        Original size      Compressed size    Deduplicated size
2026-02-21 16:53:17,169: DEBUG - All archives:               62.46 GB             62.46 GB             61.95 GB
2026-02-21 16:53:17,169: DEBUG - 
2026-02-21 16:53:17,170: DEBUG -                        Unique chunks         Total chunks
2026-02-21 16:53:17,170: DEBUG - Chunk index:                   67903                69582



------------------------------------------------------------------------------
                         TIME GLOBAL   
------------------------------------------------------------------------------
Command being timed: "sudo yunohost backup create -n test-mobilizonnone --method borg_app --apps mobilizon"
	User time (seconds): 0.00
	System time (seconds): 0.00
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 1:03.66
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7424
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 801
	Voluntary context switches: 69
	Involuntary context switches: 1
	Swaps: 0
	File system inputs: 280
	File system outputs: 0
	Socket messages sent: 0
	Socket messages received: 0
	Signals delivered: 0
	Page size (bytes): 4096
	Exit status: 0


------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE MOBILIZON none
 -----------------------------------------------------------------------------
Time (start): Sat, 2026-02-21 16:52:20
Time (end): Sat, 2026-02-21 16:53:15
Duration: 54.98 seconds
Number of files: 26758
Command line: /var/www/borg/venv/bin/borg create --compression none --exclude-if-present .nobackup --stats '::test-mobilizonnone-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:                2.92 GB              2.92 GB              2.91 GB
All archives:               62.46 GB             62.46 GB             61.95 GB

                       Unique chunks         Total chunks
Chunk index:                   67903                69582
```
