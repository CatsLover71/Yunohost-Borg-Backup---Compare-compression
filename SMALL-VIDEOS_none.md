```
https://paste.yunohost.org/raw/cadijiroki

args:
  apps:
  - my_webapp
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-smallvideonone
  output_directory: null
  system: null
ended_at: 2026-02-21 16:34:06.912132
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - my_webapp
started_at: 2026-02-21 16:29:52.886208
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
    Command being timed: "/var/www/borg/venv/bin/borg create --compression none --exclude-if-present .nobackup --stats ::test-smallvideonone-{now} ."
 	User time (seconds): 189.14
 	System time (seconds): 31.55
 	Percent of CPU this job got: 88%
 	Elapsed (wall clock) time (h:mm:ss or m:ss): 4:10.37
 	Average shared text size (kbytes): 0
 	Average unshared data size (kbytes): 0
 	Average stack size (kbytes): 0
 	Average total size (kbytes): 0
 	Maximum resident set size (kbytes): 81012
 	Average resident set size (kbytes): 0
 	Major (requiring I/O) page faults: 0
 	Minor (reclaiming a frame) page faults: 711178
 	Voluntary context switches: 21560
 	Involuntary context switches: 3384
 	Swaps: 0
 	File system inputs: 54713600
 	File system outputs: 42261479
 	Socket messages sent: 0
 	Socket messages received: 0
 	Signals delivered: 0
 	Page size (bytes): 4096
 	Exit status: 0


------------------------------------------------------------------------------
                         BORG INFO APRES   
------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               21.65 GB             21.65 GB             21.64 GB
 
                        Unique chunks         Total chunks
 Chunk index:                    9743                 9761



------------------------------------------------------------------------------
                         TIME GLOBAL   
------------------------------------------------------------------------------
    Command being timed: "sudo yunohost backup create -n test-smallvideonone --method borg_app --apps my_webapp"
	User time (seconds): 0.00
	System time (seconds): 0.01
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 4:14.20
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7552
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 799
	Voluntary context switches: 64
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
                       BORG INFO DE L'ARCHIVE SMALL VID none
 ------------------------------------------------------------------------------
Time (start): Sat, 2026-02-21 16:29:55
Time (end): Sat, 2026-02-21 16:34:05
Duration: 4 minutes 9.78 seconds
Number of files: 1555
Command line: /var/www/borg/venv/bin/borg create --compression none --exclude-if-present .nobackup --stats '::test-smallvideonone-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               21.65 GB             21.65 GB             21.63 GB
All archives:               21.65 GB             21.65 GB             21.64 GB

                       Unique chunks         Total chunks
Chunk index:                    9743                 9761
```
