```
https://paste.yunohost.org/raw/kidebiyewo

args:
  apps:
  - calibreweb
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-calibrewebzstd3
  output_directory: null
  system: null
ended_at: 2026-02-21 14:39:32.166028
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - calibreweb
started_at: 2026-02-21 14:35:38.078323
started_by: ******
success: true
yunohost_version: 12.1.39

============


------------------------------------------------------------------------------
                         BORG INFO AVANT   
------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               43.57 GB             43.24 GB             43.22 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   18144                18212

 ------------------------------------------------------------------------------
                         TIME BORG CREATE   
 ------------------------------------------------------------------------------
    Command being timed: "/var/www/borg/venv/bin/borg create --compression zstd,3 --exclude-if-present .nobackup --stats ::test-calibrewebzstd3-{now} ."
 	User time (seconds): 180.43
 	System time (seconds): 23.25
 	Percent of CPU this job got: 89%
 	Elapsed (wall clock) time (h:mm:ss or m:ss): 3:48.61
 	Average shared text size (kbytes): 0
 	Average unshared data size (kbytes): 0
 	Average stack size (kbytes): 0
 	Average total size (kbytes): 0
 	Maximum resident set size (kbytes): 105736
 	Average resident set size (kbytes): 0
 	Major (requiring I/O) page faults: 1
 	Minor (reclaiming a frame) page faults: 38866
 	Voluntary context switches: 30753
 	Involuntary context switches: 2442
 	Swaps: 0
 	File system inputs: 38489626
 	File system outputs: 27428550
 	Socket messages sent: 0
 	Socket messages received: 0
 	Signals delivered: 0
 	Page size (bytes): 4096
 	Exit status: 0


------------------------------------------------------------------------------
                         BORG INFO APRES   
------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               59.54 GB             57.76 GB             57.25 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   41268                42715



------------------------------------------------------------------------------
                         TIME GLOBAL   
------------------------------------------------------------------------------
    Command being timed: "sudo yunohost backup create -n test-calibrewebzstd3 --method borg_app --apps calibreweb"
	User time (seconds): 0.00
	System time (seconds): 0.00
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 3:54.28
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7424
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 796
	Voluntary context switches: 63
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
                       BORG INFO DE L'ARCHIVE CALIBRE WEB zstd,3 
 ------------------------------------------------------------------------------
Time (start): Sat, 2026-02-21 14:35:42
Time (end): Sat, 2026-02-21 14:39:29
Duration: 3 minutes 47.07 seconds
Number of files: 18795
Command line: /var/www/borg/venv/bin/borg create --compression zstd,3 --exclude-if-present .nobackup --stats '::test-calibrewebzstd3-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               15.97 GB             14.52 GB             14.03 GB
All archives:               59.54 GB             57.76 GB             57.25 GB

                       Unique chunks         Total chunks
Chunk index:                   41268                42715
```
