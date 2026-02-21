```
https://paste.yunohost.org/raw/tasajumumu

args:
  apps:
  - funkwhale
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-funkwhalenone
  output_directory: null
  system: null
ended_at: 2026-02-21 16:58:20.519964
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - funkwhale
started_at: 2026-02-21 16:55:21.606211
started_by: ******
success: true
yunohost_version: 12.1.39

============

------------------------------------------------------------------------------
                         BORG INFO AVANT   
------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               62.46 GB             62.46 GB             61.95 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   67903                69582


 ------------------------------------------------------------------------------
                         TIME BORG CREATE   
 ------------------------------------------------------------------------------
    Command being timed: "/var/www/borg/venv/bin/borg create --compression none --exclude-if-present .nobackup --stats ::test-funkwhalenone-{now} ."
 	User time (seconds): 121.56
 	System time (seconds): 19.64
 	Percent of CPU this job got: 83%
 	Elapsed (wall clock) time (h:mm:ss or m:ss): 2:49.43
 	Average shared text size (kbytes): 0
 	Average unshared data size (kbytes): 0
 	Average stack size (kbytes): 0
 	Average total size (kbytes): 0
 	Maximum resident set size (kbytes): 104716
 	Average resident set size (kbytes): 0
 	Major (requiring I/O) page faults: 0
 	Minor (reclaiming a frame) page faults: 416762
 	Voluntary context switches: 40878
 	Involuntary context switches: 1807
 	Swaps: 0
 	File system inputs: 37021909
 	File system outputs: 25430371
 	Socket messages sent: 0
 	Socket messages received: 0
 	Signals delivered: 0
 	Page size (bytes): 4096
 	Exit status: 0


------------------------------------------------------------------------------
                         BORG INFO APRES   
------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               75.72 GB             75.72 GB             74.93 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   95451               102556


------------------------------------------------------------------------------
                         TIME GLOBAL   
------------------------------------------------------------------------------
    Command being timed: "sudo yunohost backup create -n test-funkwhalenone --method borg_app --apps funkwhale"
	User time (seconds): 0.00
	System time (seconds): 0.00
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 2:59.10
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7296
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 798
	Voluntary context switches: 62
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
                       BORG INFO DE L'ARCHIVE FUNKWHALE none
 -----------------------------------------------------------------------------
Time (start): Sat, 2026-02-21 16:55:30
Time (end): Sat, 2026-02-21 16:58:18
Duration: 2 minutes 48.06 seconds
Number of files: 29015
Command line: /var/www/borg/venv/bin/borg create --compression none --exclude-if-present .nobackup --stats '::test-funkwhalenone-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               13.26 GB             13.26 GB             12.98 GB
All archives:               75.72 GB             75.72 GB             74.93 GB

                       Unique chunks         Total chunks
Chunk index:                   95451               102556
```
