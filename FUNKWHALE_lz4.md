```
args:
  apps:
  - funkwhale
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-Funkwhale1
  output_directory: null
  system: null
ended_at: 2026-02-18 10:37:03.703287
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - funkwhale
started_at: 2026-02-18 10:34:06.321610
started_by: ******
success: true
yunohost_version: 12.1.39

============

 ------------------------------------------------------------------------------
                         BORG INFO AVANT   
 ------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               62.46 GB             60.99 GB             60.48 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   67964                69683

 ------------------------------------------------------------------------------
                         TIME BORG CREATE   
 ------------------------------------------------------------------------------
    Command being timed: "/var/www/borg/venv/bin/borg create --exclude-if-present .nobackup --stats ::test-Funkwhale1-{now} ."
 	User time (seconds): 125.51
 	System time (seconds): 18.71
 	Percent of CPU this job got: 84%
 	Elapsed (wall clock) time (h:mm:ss or m:ss): 2:51.41
 	Average shared text size (kbytes): 0
 	Average unshared data size (kbytes): 0
 	Average stack size (kbytes): 0
 	Average total size (kbytes): 0
 	Maximum resident set size (kbytes): 109232
 	Average resident set size (kbytes): 0
 	Major (requiring I/O) page faults: 0
 	Minor (reclaiming a frame) page faults: 168357
 	Voluntary context switches: 39634
 	Involuntary context switches: 2335
 	Swaps: 0
 	File system inputs: 37028698
 	File system outputs: 23809234
 	Socket messages sent: 0
 	Socket messages received: 0
 	Signals delivered: 0
 	Page size (bytes): 4096
 	Exit status: 0


 ------------------------------------------------------------------------------
                         BORG INFO APRES   
 ------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               75.74 GB             73.40 GB             72.64 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   95473               102594



 ------------------------------------------------------------------------------
                         TIME GLOBAL   
 ------------------------------------------------------------------------------
    Command being timed: "sudo yunohost backup create -n test-Funkwhale1 --method borg_app --apps funkwhale"
	User time (seconds): 0.00
	System time (seconds): 0.01
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 2:57.56
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7296
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 794
	Voluntary context switches: 67
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
                       BORG INFO DE L'ARCHIVE FUNKWHALE 1 lz4
 ------------------------------------------------------------------------------
Time (start): Wed, 2026-02-18 10:34:11
Time (end): Wed, 2026-02-18 10:37:01
Duration: 2 minutes 50.16 seconds
Number of files: 28989
Command line: /var/www/borg/venv/bin/borg create --exclude-if-present .nobackup --stats '::test-Funkwhale1-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               13.27 GB             12.41 GB             12.16 GB
All archives:               75.74 GB             73.40 GB             72.64 GB

                       Unique chunks         Total chunks
Chunk index:                   95473               102594
```
