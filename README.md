# Yunohost-Borg Backup Compare-compression
A compare of default lz4 and auto,zstd,3 compression in Borb backup-Yunohost application

In link to this Yunohost forum discussion, [Question compression des vidéos et fichiers média en général](https://forum.yunohost.org/t/question-compression-des-videos-et-fichiers-media-en-general/41524) we decided to do a compare test of the actual ynh-borg app compression (default lz4) and auto,zstd,3 compression.

## for people in a hurry
If you're in a hurry, spoiler alert, there's no major difference.

## Dataset used

  20.1 GB of 1528 small video files called SMALL-VIDEO
  20.4 GB of 7 big video files called BIG-VIDEO
  A Calibre-web application of 15 Go mainly ePub and PDF files called CALIBRE
  A mobilizon application of 2.96 Go called MOBILIZON
  A Funkwhale app of 13 Go mainly composed of mp3 files called FUNKWHALE

    
## summary results using borg info
Detailed data of the test are present in the different files in this repository. The files named 1 were run with default lz4 and the files named 2 were run with auto,zstd,3. They use the GNU-time command to get some more informations.
The global archive datas application by application are not significant cause tests where not run in the same order.

### Small video
```
 ------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE SMALL-VIDEO lz4
 ------------------------------------------------------------------------------
Time (start): Tue, 2026-02-17 20:57:11
Time (end): Tue, 2026-02-17 21:01:35
Duration: 4 minutes 24.14 seconds
Number of files: 1555
Command line: /var/www/borg/venv/bin/borg create --exclude-if-present .nobackup --stats '::test-smallvideo1-bis-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               21.65 GB             21.48 GB             21.46 GB
All archives:               40.54 GB             39.07 GB             38.56 GB

                       Unique chunks         Total chunks
Chunk index:                   59368                61064
```

```
 ------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE SMALL-VIDEO auto,zstd,3
 ------------------------------------------------------------------------------
Time (start): Wed, 2026-02-18 11:33:03
Time (end): Wed, 2026-02-18 11:37:39
Duration: 4 minutes 35.40 seconds
Number of files: 1555
Command line: /var/www/borg/venv/bin/borg create --compression auto,zstd,3 --exclude-if-present .nobackup --stats '::test-smallvideo2BIS-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               21.65 GB             21.45 GB             21.44 GB
All archives:               21.65 GB             21.46 GB             21.44 GB

                       Unique chunks         Total chunks
Chunk index:                    9673                 9708
```
### Big video
```
 ------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE BIG-VIDEO lz4
 ------------------------------------------------------------------------------
Time (start): Wed, 2026-02-18 09:07:30
Time (end): Wed, 2026-02-18 09:11:52
Duration: 4 minutes 21.99 seconds
Number of files: 34
Command line: /var/www/borg/venv/bin/borg create --exclude-if-present .nobackup --stats '::test-Bigvideo1-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               21.92 GB             21.92 GB             21.92 GB
All archives:               62.46 GB             60.99 GB             60.48 GB

                       Unique chunks         Total chunks
Chunk index:                   67964                69683
```
```
 ------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE BIG-VIDEO2 auto,zstd,3
 ------------------------------------------------------------------------------
Time (start): Wed, 2026-02-18 12:34:15
Time (end): Wed, 2026-02-18 12:38:30
Duration: 4 minutes 14.54 seconds
Number of files: 34
Command line: /var/www/borg/venv/bin/borg create --compression auto,zstd,3 --exclude-if-present .nobackup --stats '::test-bigvideo2-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               21.92 GB             21.92 GB             21.92 GB
All archives:               43.57 GB             43.38 GB             43.36 GB

                       Unique chunks         Total chunks
Chunk index:                   18171                18229
```
### Calibre Web
```
 ------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE CALIBREWEB 1 lz4
 ------------------------------------------------------------------------------
Time (start): Sat, 2026-02-14 17:15:21
Time (end): Sat, 2026-02-14 17:19:04
Duration: 3 minutes 42.47 seconds
Number of files: 18795
Command line: /var/www/borg/venv/bin/borg create --exclude-if-present .nobackup --stats '::test-calibreweb1-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               15.97 GB             14.91 GB             14.42 GB
All archives:               18.90 GB             17.59 GB             17.10 GB

                       Unique chunks         Total chunks
Chunk index:                   49746                51432
```
```
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
### Mobilizon
```
 ------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE MOBILIZON 1 lz4
 ------------------------------------------------------------------------------
Time (start): Sat, 2026-02-14 16:51:30
Time (end): Sat, 2026-02-14 16:52:23
Duration: 53.72 seconds
Number of files: 26758
Command line: /var/www/borg/venv/bin/borg create --exclude-if-present .nobackup --stats '::test-mobilizon1-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:                2.92 GB              2.68 GB              2.67 GB
All archives:               18.90 GB             17.59 GB             17.10 GB

                       Unique chunks         Total chunks
Chunk index:                   49746                51432
```
```
 ------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE MOBILIZON 2 auto,zstd,3
 ------------------------------------------------------------------------------
Time (start): Wed, 2026-02-18 13:06:30
Time (end): Wed, 2026-02-18 13:07:30
Duration: 59.46 seconds
Number of files: 26758
Command line: /var/www/borg/venv/bin/borg create --compression auto,zstd,3 --exclude-if-present .nobackup --stats '::test-Mobilizon2-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:                2.92 GB              2.61 GB              2.61 GB
All archives:               62.46 GB             60.62 GB             60.13 GB

                       Unique chunks         Total chunks
Chunk index:                   67902                69617
```
### Funkwhale
```
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
```
 ------------------------------------------------------------------------------
                       BORG INFO DE L'ARCHIVE FUNKWHALE 2 auto,zstd,3
 ------------------------------------------------------------------------------
Time (start): Wed, 2026-02-18 13:17:41
Time (end): Wed, 2026-02-18 13:20:54
Duration: 3 minutes 12.62 seconds
Number of files: 28989
Command line: /var/www/borg/venv/bin/borg create --compression auto,zstd,3 --exclude-if-present .nobackup --stats '::test-funkwhale2-{now}' .
Utilization of maximum supported archive size: 0%
------------------------------------------------------------------------------
                       Original size      Compressed size    Deduplicated size
This archive:               13.27 GB             12.30 GB             12.06 GB
All archives:               75.74 GB             72.93 GB             72.19 GB

                       Unique chunks         Total chunks
Chunk index:                   95461               102593
```
### Final size of the repository

```
                       Original size      Compressed size    Deduplicated size
All archives:               75.74 GB             73.40 GB             72.64 GB  Defult lz4
All archives:               75.74 GB             72.93 GB             72.19 GB  auto,zstd,3
```
