```
https://paste.yunohost.org/raw/afidukafer

args:
  apps:
  - my_webapp__2
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-bigvideonone
  output_directory: null
  system: null
ended_at: 2026-02-21 16:42:02.655184
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - my_webapp__2
started_at: 2026-02-21 16:37:50.349528
started_by: ******
success: true
yunohost_version: 12.1.39

============


------------------------------------------------------------------------------
                         BORG INFO AVANT   
------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               21.65 GB             21.65 GB             21.64 GB
 
                        Unique chunks         Total chunks
 Chunk index:                    9743                 9761

 ------------------------------------------------------------------------------
                         TIME BORG CREATE   
 ------------------------------------------------------------------------------
    Command being timed: "/var/www/borg/venv/bin/borg create --compression none --exclude-if-present .nobackup --stats ::test-bigvideonone-{now} ."
 	User time (seconds): 195.35
 	System time (seconds): 33.88
 	Percent of CPU this job got: 92%
 	Elapsed (wall clock) time (h:mm:ss or m:ss): 4:08.65
 	Average shared text size (kbytes): 0
 	Average unshared data size (kbytes): 0
 	Average stack size (kbytes): 0
 	Average total size (kbytes): 0
 	Maximum resident set size (kbytes): 78556
 	Average resident set size (kbytes): 0
 	Major (requiring I/O) page faults: 0
 	Minor (reclaiming a frame) page faults: 1147978
 	Voluntary context switches: 13668
 	Involuntary context switches: 4182
 	Swaps: 0
 	File system inputs: 49489300
 	File system outputs: 42827269
 	Socket messages sent: 0
 	Socket messages received: 0
 	Signals delivered: 0
 	Page size (bytes): 4096
 	Exit status: 0


------------------------------------------------------------------------------
                         BORG INFO APRES   
------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               43.57 GB             43.57 GB             43.56 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   18284                18325



------------------------------------------------------------------------------
                         TIME GLOBAL   
------------------------------------------------------------------------------
    Command being timed: "sudo yunohost backup create -n test-bigvideonone --method borg_app --apps my_webapp__2"
	User time (seconds): 0.00
	System time (seconds): 0.00
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 4:12.49
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7296
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 798
	Voluntary context switches: 66
	Involuntary context switches: 1
	Swaps: 0
	File system inputs: 280
	File system outputs: 0
	Socket messages sent: 0
	Socket messages received: 0
	Signals delivered: 0
	Page size (bytes): 4096


------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE BIG VID none
 ------------------------------------------------------------------------------
Time (start): Sat, 2026-02-21 16:37:53
Time (end): Sat, 2026-02-21 16:42:00
Duration: 4 minutes 7.41 seconds
Number of files: 34
Command line: /var/www/borg/venv/bin/borg create --compression none --exclude-if-present .nobackup --stats '::test-bigvideonone-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               21.92 GB             21.92 GB             21.92 GB
All archives:               43.57 GB             43.57 GB             43.56 GB

                       Unique chunks         Total chunks
Chunk index:                   18284                18325
```
