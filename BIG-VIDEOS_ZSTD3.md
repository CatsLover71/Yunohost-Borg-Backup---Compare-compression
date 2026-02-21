```
https://paste.yunohost.org/raw/yacayixixi

args:
  apps:
  - my_webapp__2
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-bigvideozstd3
  output_directory: null
  system: null
ended_at: 2026-02-21 14:23:26.309399
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - my_webapp__2
started_at: 2026-02-21 14:19:00.011095
started_by: ******
success: true
yunohost_version: 12.1.39

============


------------------------------------------------------------------------------
                         BORG INFO AVANT   
------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               21.65 GB             21.34 GB             21.32 GB
 
                        Unique chunks         Total chunks
 Chunk index:                    9545                 9590

 ------------------------------------------------------------------------------
                         TIME BORG CREATE   
 ------------------------------------------------------------------------------
    Command being timed: "/var/www/borg/venv/bin/borg create --compression zstd,3 --exclude-if-present .nobackup --stats ::test-bigvideozstd3-{now} ."
 	User time (seconds): 210.60
 	System time (seconds): 31.89
 	Percent of CPU this job got: 92%
 	Elapsed (wall clock) time (h:mm:ss or m:ss): 4:22.44
 	Average shared text size (kbytes): 0
 	Average unshared data size (kbytes): 0
 	Average stack size (kbytes): 0
 	Average total size (kbytes): 0
 	Maximum resident set size (kbytes): 86400
 	Average resident set size (kbytes): 0
 	Major (requiring I/O) page faults: 0
 	Minor (reclaiming a frame) page faults: 33940
 	Voluntary context switches: 13492
 	Involuntary context switches: 4364
 	Swaps: 0
 	File system inputs: 49371052
 	File system outputs: 42799739
 	Socket messages sent: 0
 	Socket messages received: 0
 	Signals delivered: 0
 	Page size (bytes): 4096
 	Exit status: 0


------------------------------------------------------------------------------
                         BORG INFO APRES   
------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               43.57 GB             43.24 GB             43.22 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   18144                18212



------------------------------------------------------------------------------
                         TIME GLOBAL   
------------------------------------------------------------------------------
	Command being timed: "sudo yunohost backup create -n test-bigvideozstd3 --method borg_app --apps my_webapp__2"
	User time (seconds): 0.00
	System time (seconds): 0.01
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 4:26.49
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7552
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 796
	Voluntary context switches: 62
	Involuntary context switches: 3
	Swaps: 0
	File system inputs: 280
	File system outputs: 0
	Socket messages sent: 0
	Socket messages received: 0
	Signals delivered: 0
	Page size (bytes): 4096
	Exit status: 0


 ------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE BIG VID zstd,3 
 ------------------------------------------------------------------------------
Time (start): Sat, 2026-02-21 14:19:02
Time (end): Sat, 2026-02-21 14:23:24
Duration: 4 minutes 21.24 seconds
Number of files: 34
Command line: /var/www/borg/venv/bin/borg create --compression zstd,3 --exclude-if-present .nobackup --stats '::test-bigvideozstd3-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               21.92 GB             21.91 GB             21.91 GB
All archives:               43.57 GB             43.24 GB             43.22 GB

                       Unique chunks         Total chunks
Chunk index:                   18144                18212
```
