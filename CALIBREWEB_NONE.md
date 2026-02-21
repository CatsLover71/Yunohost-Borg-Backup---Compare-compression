```
https://paste.yunohost.org/raw/ejojuhihos

args:
  apps:
  - calibreweb
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-calibrewebnone
  output_directory: null
  system: null
ended_at: 2026-02-21 16:49:15.938441
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - calibreweb
started_at: 2026-02-21 16:46:00.087768
started_by: ******
success: true
yunohost_version: 12.1.39

============

------------------------------------------------------------------------------
                         BORG INFO AVANT   
------------------------------------------------------------------------------
2026-02-21 16:46:04,406: DEBUG -                        Original size      Compressed size    Deduplicated size
2026-02-21 16:46:04,407: DEBUG - All archives:               43.57 GB             43.57 GB             43.56 GB
2026-02-21 16:46:04,407: DEBUG - 
2026-02-21 16:46:04,407: DEBUG -                        Unique chunks         Total chunks
2026-02-21 16:46:04,407: DEBUG - Chunk index:                   18284                18325


 ------------------------------------------------------------------------------
                         TIME BORG CREATE   
 ------------------------------------------------------------------------------
Command being timed: "/var/www/borg/venv/bin/borg create --compression none --exclude-if-present .nobackup --stats ::test-calibrewebnone-{now} ."
Warning: 	User time (seconds): 142.53
Warning: 	System time (seconds): 25.70
Warning: 	Percent of CPU this job got: 88%
Warning: 	Elapsed (wall clock) time (h:mm:ss or m:ss): 3:10.37
Warning: 	Average shared text size (kbytes): 0
Warning: 	Average unshared data size (kbytes): 0
Warning: 	Average stack size (kbytes): 0
Warning: 	Average total size (kbytes): 0
Warning: 	Maximum resident set size (kbytes): 90956
Warning: 	Average resident set size (kbytes): 0
Warning: 	Major (requiring I/O) page faults: 0
Warning: 	Minor (reclaiming a frame) page faults: 835859
Warning: 	Voluntary context switches: 29161
Warning: 	Involuntary context switches: 2495
Warning: 	Swaps: 0
Warning: 	File system inputs: 38554081
Warning: 	File system outputs: 30229720
Warning: 	Socket messages sent: 0
Warning: 	Socket messages received: 0
Warning: 	Signals delivered: 0
Warning: 	Page size (bytes): 4096
Warning: 	Exit status: 0


------------------------------------------------------------------------------
                         BORG INFO APRES   
------------------------------------------------------------------------------
2026-02-21 16:49:15,349: DEBUG -                        Original size      Compressed size    Deduplicated size
2026-02-21 16:49:15,350: DEBUG - All archives:               59.54 GB             59.54 GB             59.02 GB
2026-02-21 16:49:15,350: DEBUG - 
2026-02-21 16:49:15,351: DEBUG -                        Unique chunks         Total chunks
2026-02-21 16:49:15,351: DEBUG - Chunk index:                   41221                42618



------------------------------------------------------------------------------
                         TIME GLOBAL   
------------------------------------------------------------------------------
Command being timed: "sudo yunohost backup create -n test-calibrewebnone --method borg_app --apps calibreweb"
	User time (seconds): 0.00
	System time (seconds): 0.00
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 3:16.05
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7552
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 799
	Voluntary context switches: 64
	Involuntary context switches: 0
	Swaps: 0
	File system inputs: 280
	File system outputs: 0
	Socket messages sent: 0
	Socket messages received: 0
	Signals delivered: 0
	Page size (bytes): 4096
	Exit status: 0


------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE CALIBRE WEB none
 ------------------------------------------------------------------------------
Time (start): Sat, 2026-02-21 16:46:04
Time (end): Sat, 2026-02-21 16:49:14
Duration: 3 minutes 9.36 seconds
Number of files: 18795
Command line: /var/www/borg/venv/bin/borg create --compression none --exclude-if-present .nobackup --stats '::test-calibrewebnone-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               15.97 GB             15.97 GB             15.46 GB
All archives:               59.54 GB             59.54 GB             59.02 GB

                       Unique chunks         Total chunks
Chunk index:                   41221                42618
```
