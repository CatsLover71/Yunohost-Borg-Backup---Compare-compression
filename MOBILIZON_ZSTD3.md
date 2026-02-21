```
https://paste.yunohost.org/raw/uwijevedem

args:
  apps:
  - mobilizon
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-mobilizonzstd3
  output_directory: null
  system: null
ended_at: 2026-02-21 14:50:19.721233
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - mobilizon
started_at: 2026-02-21 14:49:08.641167
started_by: ******
success: true
yunohost_version: 12.1.39

============


------------------------------------------------------------------------------
                         BORG INFO AVANT   
------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               59.54 GB             57.76 GB             57.25 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   41268                42715

 ------------------------------------------------------------------------------
                         TIME BORG CREATE   
 ------------------------------------------------------------------------------
    Command being timed: "/var/www/borg/venv/bin/borg create --compression zstd,3 --exclude-if-present .nobackup --stats ::test-mobilizonzstd3-{now} ."
 	User time (seconds): 36.05
 	System time (seconds): 5.01
 	Percent of CPU this job got: 64%
 	Elapsed (wall clock) time (h:mm:ss or m:ss): 1:04.06
 	Average shared text size (kbytes): 0
 	Average unshared data size (kbytes): 0
 	Average stack size (kbytes): 0
 	Average total size (kbytes): 0
 	Maximum resident set size (kbytes): 109872
 	Average resident set size (kbytes): 0
 	Major (requiring I/O) page faults: 0
 	Minor (reclaiming a frame) page faults: 40370
 	Voluntary context switches: 34779
 	Involuntary context switches: 495
 	Swaps: 0
 	File system inputs: 11116636
 	File system outputs: 5139975
 	Socket messages sent: 0
 	Socket messages received: 0
 	Signals delivered: 0
 	Page size (bytes): 4096
 	Exit status: 0


------------------------------------------------------------------------------
                         BORG INFO APRES   
------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               62.46 GB             60.38 GB             59.86 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   67971                69702



------------------------------------------------------------------------------
                         TIME GLOBAL   
------------------------------------------------------------------------------
    Command being timed: "sudo yunohost backup create -n test-mobilizonzstd3 --method borg_app --apps mobilizon"
	User time (seconds): 0.00
	System time (seconds): 0.01
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 1:11.26
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7552
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 801
	Voluntary context switches: 66
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
                       BORG INFO DE L'ARCHIVE MOBILIZON zstd,3 
 ------------------------------------------------------------------------------
Time (start): Sat, 2026-02-21 14:49:14
Time (end): Sat, 2026-02-21 14:50:17
Duration: 1 minutes 2.41 seconds
Number of files: 26758
Command line: /var/www/borg/venv/bin/borg create --compression zstd,3 --exclude-if-present .nobackup --stats '::test-mobilizonzstd3-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:                2.92 GB              2.61 GB              2.61 GB
All archives:               62.46 GB             60.38 GB             59.86 GB

                       Unique chunks         Total chunks
Chunk index:                   67971                69702
```
