```
args:
  apps:
  - calibreweb
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-Calibre2
  output_directory: null
  system: null
ended_at: 2026-02-18 12:56:02.403633
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - calibreweb
started_at: 2026-02-18 12:52:15.750517
started_by: ******
success: true
yunohost_version: 12.1.39

============


 ------------------------------------------------------------------------------
                         BORG INFO AVANT   
 ------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               43.57 GB             43.38 GB             43.36 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   18171                18229

 ------------------------------------------------------------------------------
                         TIME BORG CREATE   
 ------------------------------------------------------------------------------
    Command being timed: "/var/www/borg/venv/bin/borg create --compression auto,zstd,3 --exclude-if-present .nobackup --stats ::test-Calibre2-{now} ."
    User time (seconds): 177.60
 	System time (seconds): 21.67
 	Percent of CPU this job got: 90%
 	Elapsed (wall clock) time (h:mm:ss or m:ss): 3:40.81
 	Average shared text size (kbytes): 0
 	Average unshared data size (kbytes): 0
 	Average stack size (kbytes): 0
 	Average total size (kbytes): 0
 	Maximum resident set size (kbytes): 109836
 	Average resident set size (kbytes): 0
 	Major (requiring I/O) page faults: 2
 	Minor (reclaiming a frame) page faults: 39859
 	Voluntary context switches: 30766
 	Involuntary context switches: 2656
 	Swaps: 0
 	File system inputs: 38385484
 	File system outputs: 27669896
 	Socket messages sent: 0
 	Socket messages received: 0
 	Signals delivered: 0
 	Page size (bytes): 4096
 	Exit status: 0


 ------------------------------------------------------------------------------
                         BORG INFO APRES   
 ------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               59.54 GB             58.01 GB             57.52 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   41233                42664



------------------------------------------------------------------------------
                         TIME GLOBAL   
------------------------------------------------------------------------------
    Command being timed: "sudo yunohost backup create -n test-Calibre2 --method borg_app --apps calibreweb"
	User time (seconds): 0.00
	System time (seconds): 0.00
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 3:46.84
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7424
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 795
	Voluntary context switches: 53
	Involuntary context switches: 0
	Swaps: 0
	File system inputs: 283
	File system outputs: 0
	Socket messages sent: 0
	Socket messages received: 0
	Signals delivered: 0
	Page size (bytes): 4096
	Exit status: 0


 ------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE CALIBREWEB 2 auto,zstd,3 
 ------------------------------------------------------------------------------
Time (start): Wed, 2026-02-18 12:52:20
Time (end): Wed, 2026-02-18 12:56:00
Duration: 3 minutes 39.72 seconds
Number of files: 18795
Command line: /var/www/borg/venv/bin/borg create --compression auto,zstd,3 --exclude-if-present .nobackup --stats '::test-Calibre2-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               15.97 GB             14.64 GB             14.15 GB
All archives:               59.54 GB             58.01 GB             57.52 GB

                       Unique chunks         Total chunks
Chunk index:                   41233                42664
```
