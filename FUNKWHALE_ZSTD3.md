```
https://paste.yunohost.org/raw/colulicive

args:
  apps:
  - funkwhale
  description: null
  dry_run: false
  methods:
  - borg_app
  name: test-funkwhalezstd3
  output_directory: null
  system: null
ended_at: 2026-02-21 15:00:14.049031
error: null
interface: cli
operation: backup_create
parent: null
related_to:
- - app
  - funkwhale
started_at: 2026-02-21 14:56:32.647800
started_by: ******
success: true
yunohost_version: 12.1.39

============


------------------------------------------------------------------------------
                         BORG INFO AVANT   
------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               62.46 GB             60.38 GB             59.86 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   67971                69702

 ------------------------------------------------------------------------------
                         TIME BORG CREATE   
 ------------------------------------------------------------------------------
    Command being timed: "/var/www/borg/venv/bin/borg create --compression zstd,3 --exclude-if-present .nobackup --stats ::test-funkwhalezstd3-{now} ."
 	User time (seconds): 160.17
 	System time (seconds): 19.12
 	Percent of CPU this job got: 84%
 	Elapsed (wall clock) time (h:mm:ss or m:ss): 3:31.58
 	Average shared text size (kbytes): 0
 	Average unshared data size (kbytes): 0
 	Average stack size (kbytes): 0
 	Average total size (kbytes): 0
 	Maximum resident set size (kbytes): 113544
 	Average resident set size (kbytes): 0
 	Major (requiring I/O) page faults: 0
 	Minor (reclaiming a frame) page faults: 40958
 	Voluntary context switches: 42756
 	Involuntary context switches: 1992
 	Swaps: 0
 	File system inputs: 37034851
 	File system outputs: 23555222
 	Socket messages sent: 0
 	Socket messages received: 0
 	Signals delivered: 0
 	Page size (bytes): 4096
 	Exit status: 0


------------------------------------------------------------------------------
                         BORG INFO APRES   
------------------------------------------------------------------------------
                        Original size      Compressed size    Deduplicated size
 All archives:               75.72 GB             72.66 GB             71.89 GB
 
                        Unique chunks         Total chunks
 Chunk index:                   95512               102680



------------------------------------------------------------------------------
                         TIME GLOBAL   
------------------------------------------------------------------------------
    Command being timed: "sudo yunohost backup create -n test-funkwhalezstd3 --method borg_app --apps funkwhale"
	User time (seconds): 0.00
	System time (seconds): 0.00
	Percent of CPU this job got: 0%
	Elapsed (wall clock) time (h:mm:ss or m:ss): 3:41.60
	Average shared text size (kbytes): 0
	Average unshared data size (kbytes): 0
	Average stack size (kbytes): 0
	Average total size (kbytes): 0
	Maximum resident set size (kbytes): 7424
	Average resident set size (kbytes): 0
	Major (requiring I/O) page faults: 0
	Minor (reclaiming a frame) page faults: 802
	Voluntary context switches: 57
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
Time (start): Sat, 2026-02-21 14:56:41
Time (end): Sat, 2026-02-21 15:00:11
Duration: 3 minutes 30.01 seconds
Number of files: 29015
Command line: /var/www/borg/venv/bin/borg create --compression zstd,3 --exclude-if-present .nobackup --stats '::test-funkwhalezstd3-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               13.26 GB             12.28 GB             12.03 GB
All archives:               75.72 GB             72.66 GB             71.89 GB

                       Unique chunks         Total chunks
Chunk index:                   95512               102680
```
