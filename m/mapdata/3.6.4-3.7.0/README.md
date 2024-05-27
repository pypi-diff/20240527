# Comparing `tmp/mapdata-3.6.4.tar.gz` & `tmp/mapdata-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapdata-3.6.4.tar", last modified: Fri May 17 21:31:32 2024, max compression
+gzip compressed data, was "mapdata-3.7.0.tar", last modified: Mon May 27 14:16:15 2024, max compression
```

## Comparing `mapdata-3.6.4.tar` & `mapdata-3.7.0.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-17 21:31:32.479142 mapdata-3.6.4/
--rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-3.6.4/LICENSE.txt
--rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-3.6.4/MANIFEST.in
--rw-r--r--   0 dreas     (1000) dreas     (1000)     7898 2024-05-17 21:31:32.479142 mapdata-3.6.4/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)     6421 2024-05-04 17:16:18.000000 mapdata-3.6.4/README.md
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-17 21:31:32.443142 mapdata-3.6.4/mapdata/
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-17 21:31:32.443142 mapdata-3.6.4/mapdata/configfile/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     9002 2024-03-04 21:04:24.000000 mapdata-3.6.4/mapdata/configfile/mapdata.conf
--rwxrwxr-x   0 dreas     (1000) dreas     (1000)   672909 2024-05-17 21:28:58.000000 mapdata-3.6.4/mapdata/mapdata.py
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-17 21:31:32.443142 mapdata-3.6.4/mapdata/symbols/
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-17 21:31:32.475142 mapdata-3.6.4/mapdata/symbols/16x16/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:04:56.000000 mapdata-3.6.4/mapdata/symbols/16x16/0.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:16.000000 mapdata-3.6.4/mapdata/symbols/16x16/1.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:29.000000 mapdata-3.6.4/mapdata/symbols/16x16/2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:40.000000 mapdata-3.6.4/mapdata/symbols/16x16/3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:05:52.000000 mapdata-3.6.4/mapdata/symbols/16x16/4.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:06:03.000000 mapdata-3.6.4/mapdata/symbols/16x16/5.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:28:02.000000 mapdata-3.6.4/mapdata/symbols/16x16/6.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:27.000000 mapdata-3.6.4/mapdata/symbols/16x16/7.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:40.000000 mapdata-3.6.4/mapdata/symbols/16x16/8.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:26:59.000000 mapdata-3.6.4/mapdata/symbols/16x16/9.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:04:26.000000 mapdata-3.6.4/mapdata/symbols/16x16/A.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:07:30.000000 mapdata-3.6.4/mapdata/symbols/16x16/B.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:10:14.000000 mapdata-3.6.4/mapdata/symbols/16x16/C.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:13:27.000000 mapdata-3.6.4/mapdata/symbols/16x16/D.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:14:22.000000 mapdata-3.6.4/mapdata/symbols/16x16/E.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:15:26.000000 mapdata-3.6.4/mapdata/symbols/16x16/F.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 00:14:24.000000 mapdata-3.6.4/mapdata/symbols/16x16/G.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:15:07.000000 mapdata-3.6.4/mapdata/symbols/16x16/H.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:16:00.000000 mapdata-3.6.4/mapdata/symbols/16x16/I.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:18:38.000000 mapdata-3.6.4/mapdata/symbols/16x16/J.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:21:25.000000 mapdata-3.6.4/mapdata/symbols/16x16/K.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:22:10.000000 mapdata-3.6.4/mapdata/symbols/16x16/L.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:24:58.000000 mapdata-3.6.4/mapdata/symbols/16x16/M.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:27:42.000000 mapdata-3.6.4/mapdata/symbols/16x16/N.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 14:04:25.000000 mapdata-3.6.4/mapdata/symbols/16x16/O.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:28:05.000000 mapdata-3.6.4/mapdata/symbols/16x16/P.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:29:12.000000 mapdata-3.6.4/mapdata/symbols/16x16/Q.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:30:16.000000 mapdata-3.6.4/mapdata/symbols/16x16/R.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:34:31.000000 mapdata-3.6.4/mapdata/symbols/16x16/S.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:35:37.000000 mapdata-3.6.4/mapdata/symbols/16x16/T.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:37:27.000000 mapdata-3.6.4/mapdata/symbols/16x16/U.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:40:22.000000 mapdata-3.6.4/mapdata/symbols/16x16/V.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:44:48.000000 mapdata-3.6.4/mapdata/symbols/16x16/W.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:46:24.000000 mapdata-3.6.4/mapdata/symbols/16x16/X.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:47:50.000000 mapdata-3.6.4/mapdata/symbols/16x16/Y.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:49:43.000000 mapdata-3.6.4/mapdata/symbols/16x16/Z.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-21 14:55:41.000000 mapdata-3.6.4/mapdata/symbols/16x16/airplane.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-06-24 15:22:11.000000 mapdata-3.6.4/mapdata/symbols/16x16/anchor.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:00:25.000000 mapdata-3.6.4/mapdata/symbols/16x16/ball.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2024-01-24 20:44:54.000000 mapdata-3.6.4/mapdata/symbols/16x16/ball_small.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-16 13:39:00.000000 mapdata-3.6.4/mapdata/symbols/16x16/bar.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:04:48.000000 mapdata-3.6.4/mapdata/symbols/16x16/bars.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:43:55.000000 mapdata-3.6.4/mapdata/symbols/16x16/binoculars.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:29:19.000000 mapdata-3.6.4/mapdata/symbols/16x16/bird.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      288 2023-04-24 16:37:43.000000 mapdata-3.6.4/mapdata/symbols/16x16/block.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2024-01-26 04:36:33.000000 mapdata-3.6.4/mapdata/symbols/16x16/block_small.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-16 18:31:20.000000 mapdata-3.6.4/mapdata/symbols/16x16/bookmark.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:29:01.000000 mapdata-3.6.4/mapdata/symbols/16x16/box_stack.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-04-30 14:46:15.000000 mapdata-3.6.4/mapdata/symbols/16x16/camera.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 16:51:47.000000 mapdata-3.6.4/mapdata/symbols/16x16/cancel.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-21 15:05:05.000000 mapdata-3.6.4/mapdata/symbols/16x16/car.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-21 15:04:37.000000 mapdata-3.6.4/mapdata/symbols/16x16/car2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-24 01:00:13.000000 mapdata-3.6.4/mapdata/symbols/16x16/center8.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:35:37.000000 mapdata-3.6.4/mapdata/symbols/16x16/check.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 14:51:14.000000 mapdata-3.6.4/mapdata/symbols/16x16/check_circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-16 14:20:03.000000 mapdata-3.6.4/mapdata/symbols/16x16/checkbox.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-04-28 13:31:04.000000 mapdata-3.6.4/mapdata/symbols/16x16/checkerboard.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:29:46.000000 mapdata-3.6.4/mapdata/symbols/16x16/chevrons.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:12:28.000000 mapdata-3.6.4/mapdata/symbols/16x16/circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:22:20.000000 mapdata-3.6.4/mapdata/symbols/16x16/circle_bar.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 14:58:14.000000 mapdata-3.6.4/mapdata/symbols/16x16/circle_plus.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:09:20.000000 mapdata-3.6.4/mapdata/symbols/16x16/circle_stipple.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 14:29:15.000000 mapdata-3.6.4/mapdata/symbols/16x16/circle_triangle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-25 14:40:36.000000 mapdata-3.6.4/mapdata/symbols/16x16/circle_wedge.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-06-24 14:56:37.000000 mapdata-3.6.4/mapdata/symbols/16x16/circle_x.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-07-04 17:10:15.000000 mapdata-3.6.4/mapdata/symbols/16x16/clock.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 14:05:41.000000 mapdata-3.6.4/mapdata/symbols/16x16/columns.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:50:11.000000 mapdata-3.6.4/mapdata/symbols/16x16/contract.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-04-16 17:48:39.000000 mapdata-3.6.4/mapdata/symbols/16x16/cross.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-23 18:45:40.000000 mapdata-3.6.4/mapdata/symbols/16x16/darkeye.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:32.000000 mapdata-3.6.4/mapdata/symbols/16x16/decrease.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-30 12:46:46.000000 mapdata-3.6.4/mapdata/symbols/16x16/deposition.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:47.000000 mapdata-3.6.4/mapdata/symbols/16x16/diag_ll.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:26.000000 mapdata-3.6.4/mapdata/symbols/16x16/diag_lr.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:05.000000 mapdata-3.6.4/mapdata/symbols/16x16/diag_ul.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:17:04.000000 mapdata-3.6.4/mapdata/symbols/16x16/diag_ur.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-20 18:41:19.000000 mapdata-3.6.4/mapdata/symbols/16x16/dialog.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-16 17:38:10.000000 mapdata-3.6.4/mapdata/symbols/16x16/diamond.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 13:47:24.000000 mapdata-3.6.4/mapdata/symbols/16x16/donkey.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 16:45:55.000000 mapdata-3.6.4/mapdata/symbols/16x16/dot.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:00:44.000000 mapdata-3.6.4/mapdata/symbols/16x16/down.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:38:22.000000 mapdata-3.6.4/mapdata/symbols/16x16/drop.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-03 02:15:55.000000 mapdata-3.6.4/mapdata/symbols/16x16/elephant.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 14:33:40.000000 mapdata-3.6.4/mapdata/symbols/16x16/expand.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 15:03:32.000000 mapdata-3.6.4/mapdata/symbols/16x16/eye.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 13:59:48.000000 mapdata-3.6.4/mapdata/symbols/16x16/fire.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:13:54.000000 mapdata-3.6.4/mapdata/symbols/16x16/fish.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:36:11.000000 mapdata-3.6.4/mapdata/symbols/16x16/flag.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-30 15:04:58.000000 mapdata-3.6.4/mapdata/symbols/16x16/flag2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 15:06:07.000000 mapdata-3.6.4/mapdata/symbols/16x16/four_arrows.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:25:14.000000 mapdata-3.6.4/mapdata/symbols/16x16/graph.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 15:18:19.000000 mapdata-3.6.4/mapdata/symbols/16x16/hand.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:04:09.000000 mapdata-3.6.4/mapdata/symbols/16x16/hash.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-03 01:53:41.000000 mapdata-3.6.4/mapdata/symbols/16x16/heart.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2024-01-31 04:51:54.000000 mapdata-3.6.4/mapdata/symbols/16x16/hidden.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:40:09.000000 mapdata-3.6.4/mapdata/symbols/16x16/hourglass.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 22:31:53.000000 mapdata-3.6.4/mapdata/symbols/16x16/house.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:05.000000 mapdata-3.6.4/mapdata/symbols/16x16/increase.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-24 23:05:40.000000 mapdata-3.6.4/mapdata/symbols/16x16/info.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:51:36.000000 mapdata-3.6.4/mapdata/symbols/16x16/leaf.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:02:45.000000 mapdata-3.6.4/mapdata/symbols/16x16/left.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-23 13:36:40.000000 mapdata-3.6.4/mapdata/symbols/16x16/lightbulb.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 16:38:25.000000 mapdata-3.6.4/mapdata/symbols/16x16/lightning.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:14:23.000000 mapdata-3.6.4/mapdata/symbols/16x16/lightning2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-07-04 16:58:13.000000 mapdata-3.6.4/mapdata/symbols/16x16/location_ptr.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:06:42.000000 mapdata-3.6.4/mapdata/symbols/16x16/mine.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 15:07:56.000000 mapdata-3.6.4/mapdata/symbols/16x16/nested_boxes.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:07:35.000000 mapdata-3.6.4/mapdata/symbols/16x16/pennant.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:16:09.000000 mapdata-3.6.4/mapdata/symbols/16x16/pennant2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-18 19:04:36.000000 mapdata-3.6.4/mapdata/symbols/16x16/people.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:26:34.000000 mapdata-3.6.4/mapdata/symbols/16x16/person.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:30:45.000000 mapdata-3.6.4/mapdata/symbols/16x16/person2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 18:43:50.000000 mapdata-3.6.4/mapdata/symbols/16x16/person3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 15:37:42.000000 mapdata-3.6.4/mapdata/symbols/16x16/phone.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:18:45.000000 mapdata-3.6.4/mapdata/symbols/16x16/photo.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-19 22:48:26.000000 mapdata-3.6.4/mapdata/symbols/16x16/picnic.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-19 03:57:15.000000 mapdata-3.6.4/mapdata/symbols/16x16/plus.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:16.000000 mapdata-3.6.4/mapdata/symbols/16x16/point_down.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:58:03.000000 mapdata-3.6.4/mapdata/symbols/16x16/point_left.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      362 2023-05-03 01:57:47.000000 mapdata-3.6.4/mapdata/symbols/16x16/point_right.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      347 2023-05-03 01:56:56.000000 mapdata-3.6.4/mapdata/symbols/16x16/point_up.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:58:38.000000 mapdata-3.6.4/mapdata/symbols/16x16/pointer_ne.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:59:20.000000 mapdata-3.6.4/mapdata/symbols/16x16/pointer_nw.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:54.000000 mapdata-3.6.4/mapdata/symbols/16x16/pointer_se.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:59:07.000000 mapdata-3.6.4/mapdata/symbols/16x16/pointer_sw.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 18:51:06.000000 mapdata-3.6.4/mapdata/symbols/16x16/puzzle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:52:56.000000 mapdata-3.6.4/mapdata/symbols/16x16/q1.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:57:59.000000 mapdata-3.6.4/mapdata/symbols/16x16/q1_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:25.000000 mapdata-3.6.4/mapdata/symbols/16x16/q2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:55.000000 mapdata-3.6.4/mapdata/symbols/16x16/q2_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:46.000000 mapdata-3.6.4/mapdata/symbols/16x16/q3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:28.000000 mapdata-3.6.4/mapdata/symbols/16x16/q3_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:57.000000 mapdata-3.6.4/mapdata/symbols/16x16/q4.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:13.000000 mapdata-3.6.4/mapdata/symbols/16x16/q4_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-05-20 18:36:19.000000 mapdata-3.6.4/mapdata/symbols/16x16/qmark_circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-20 18:37:52.000000 mapdata-3.6.4/mapdata/symbols/16x16/qmark_circle2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:43:45.000000 mapdata-3.6.4/mapdata/symbols/16x16/raincloud.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 16:39:34.000000 mapdata-3.6.4/mapdata/symbols/16x16/right.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 17:23:57.000000 mapdata-3.6.4/mapdata/symbols/16x16/rocket.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 17:25:43.000000 mapdata-3.6.4/mapdata/symbols/16x16/rocket2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-23 16:07:27.000000 mapdata-3.6.4/mapdata/symbols/16x16/rose.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-28 14:05:56.000000 mapdata-3.6.4/mapdata/symbols/16x16/rows.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 14:27:34.000000 mapdata-3.6.4/mapdata/symbols/16x16/scales.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-07-04 17:07:45.000000 mapdata-3.6.4/mapdata/symbols/16x16/search.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-07-04 17:08:06.000000 mapdata-3.6.4/mapdata/symbols/16x16/search2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-01 15:46:45.000000 mapdata-3.6.4/mapdata/symbols/16x16/skull.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-17 02:43:53.000000 mapdata-3.6.4/mapdata/symbols/16x16/square.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:26:56.000000 mapdata-3.6.4/mapdata/symbols/16x16/star.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:07:07.000000 mapdata-3.6.4/mapdata/symbols/16x16/stipple.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-03 02:10:57.000000 mapdata-3.6.4/mapdata/symbols/16x16/stop.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 15:31:50.000000 mapdata-3.6.4/mapdata/symbols/16x16/surprise_circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:22:10.000000 mapdata-3.6.4/mapdata/symbols/16x16/swamp.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:27:50.000000 mapdata-3.6.4/mapdata/symbols/16x16/target.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:37:09.000000 mapdata-3.6.4/mapdata/symbols/16x16/target2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-06-24 15:27:04.000000 mapdata-3.6.4/mapdata/symbols/16x16/ten.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 14:54:31.000000 mapdata-3.6.4/mapdata/symbols/16x16/trash.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-09 17:01:43.000000 mapdata-3.6.4/mapdata/symbols/16x16/tree.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 12:59:30.000000 mapdata-3.6.4/mapdata/symbols/16x16/tree2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:26:26.000000 mapdata-3.6.4/mapdata/symbols/16x16/tree3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-09 16:59:51.000000 mapdata-3.6.4/mapdata/symbols/16x16/triangle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-09 17:08:13.000000 mapdata-3.6.4/mapdata/symbols/16x16/triangle_open.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-05-20 17:46:38.000000 mapdata-3.6.4/mapdata/symbols/16x16/triangle_sm.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-04-16 18:01:12.000000 mapdata-3.6.4/mapdata/symbols/16x16/up.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-30 12:50:50.000000 mapdata-3.6.4/mapdata/symbols/16x16/vapor.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 03:55:52.000000 mapdata-3.6.4/mapdata/symbols/16x16/warning.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 20:02:51.000000 mapdata-3.6.4/mapdata/symbols/16x16/wave.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:01.000000 mapdata-3.6.4/mapdata/symbols/16x16/wave2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:43.000000 mapdata-3.6.4/mapdata/symbols/16x16/wave3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-30 14:42:04.000000 mapdata-3.6.4/mapdata/symbols/16x16/weather.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 16:37:24.000000 mapdata-3.6.4/mapdata/symbols/16x16/wedge.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:53:34.000000 mapdata-3.6.4/mapdata/symbols/16x16/wedge_sm.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-29 15:40:02.000000 mapdata-3.6.4/mapdata/symbols/16x16/wedges_3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:23:44.000000 mapdata-3.6.4/mapdata/symbols/16x16/well.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:20:04.000000 mapdata-3.6.4/mapdata/symbols/16x16/whale.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 12:54:47.000000 mapdata-3.6.4/mapdata/symbols/16x16/whale2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-24 15:49:53.000000 mapdata-3.6.4/mapdata/symbols/16x16/wheelchair.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:04:57.000000 mapdata-3.6.4/mapdata/symbols/16x16/zigzags.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-19 04:39:05.000000 mapdata-3.6.4/mapdata/symbols/16x16/zigzags2.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-17 21:31:32.479142 mapdata-3.6.4/mapdata/symbols/20x20/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      464 2023-06-24 14:14:12.000000 mapdata-3.6.4/mapdata/symbols/20x20/ball20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      467 2023-06-24 14:24:29.000000 mapdata-3.6.4/mapdata/symbols/20x20/block20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:13:06.000000 mapdata-3.6.4/mapdata/symbols/20x20/circle20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:11.000000 mapdata-3.6.4/mapdata/symbols/20x20/q1_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:22.000000 mapdata-3.6.4/mapdata/symbols/20x20/q2_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:35.000000 mapdata-3.6.4/mapdata/symbols/20x20/q3_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:54.000000 mapdata-3.6.4/mapdata/symbols/20x20/q4_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:24:00.000000 mapdata-3.6.4/mapdata/symbols/20x20/square20.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-17 21:31:32.479142 mapdata-3.6.4/mapdata/symbols/24x24/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      539 2023-06-24 14:20:48.000000 mapdata-3.6.4/mapdata/symbols/24x24/ball24.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      542 2023-06-24 14:25:39.000000 mapdata-3.6.4/mapdata/symbols/24x24/block24.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:20:00.000000 mapdata-3.6.4/mapdata/symbols/24x24/circle24.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:22:10.000000 mapdata-3.6.4/mapdata/symbols/24x24/square24.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-17 21:31:32.479142 mapdata-3.6.4/mapdata/symbols/28x28/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      793 2023-06-24 14:41:23.000000 mapdata-3.6.4/mapdata/symbols/28x28/ball28.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      794 2023-06-24 14:42:33.000000 mapdata-3.6.4/mapdata/symbols/28x28/block28.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:41:39.000000 mapdata-3.6.4/mapdata/symbols/28x28/circle28.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:42:15.000000 mapdata-3.6.4/mapdata/symbols/28x28/square28.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-17 21:31:32.479142 mapdata-3.6.4/mapdata.egg-info/
--rw-r--r--   0 dreas     (1000) dreas     (1000)     7898 2024-05-17 21:31:32.000000 mapdata-3.6.4/mapdata.egg-info/PKG-INFO
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     6598 2024-05-17 21:31:32.000000 mapdata-3.6.4/mapdata.egg-info/SOURCES.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2024-05-17 21:31:32.000000 mapdata-3.6.4/mapdata.egg-info/dependency_links.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      143 2024-05-17 21:31:32.000000 mapdata-3.6.4/mapdata.egg-info/requires.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        8 2024-05-17 21:31:32.000000 mapdata-3.6.4/mapdata.egg-info/top_level.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2024-05-17 21:31:32.479142 mapdata-3.6.4/setup.cfg
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     1813 2024-05-17 21:30:43.000000 mapdata-3.6.4/setup.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-27 14:16:15.613886 mapdata-3.7.0/
+-rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-3.7.0/LICENSE.txt
+-rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-3.7.0/MANIFEST.in
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     7898 2024-05-27 14:16:15.613886 mapdata-3.7.0/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     6421 2024-05-04 17:16:18.000000 mapdata-3.7.0/README.md
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-27 14:16:15.569886 mapdata-3.7.0/mapdata/
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-27 14:16:15.569886 mapdata-3.7.0/mapdata/configfile/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     9002 2024-03-04 21:04:24.000000 mapdata-3.7.0/mapdata/configfile/mapdata.conf
+-rwxrwxr-x   0 dreas     (1000) dreas     (1000)   690920 2024-05-26 14:04:39.000000 mapdata-3.7.0/mapdata/mapdata.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-27 14:16:15.565885 mapdata-3.7.0/mapdata/symbols/
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-27 14:16:15.609886 mapdata-3.7.0/mapdata/symbols/16x16/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:04:56.000000 mapdata-3.7.0/mapdata/symbols/16x16/0.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:16.000000 mapdata-3.7.0/mapdata/symbols/16x16/1.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:29.000000 mapdata-3.7.0/mapdata/symbols/16x16/2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:40.000000 mapdata-3.7.0/mapdata/symbols/16x16/3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:05:52.000000 mapdata-3.7.0/mapdata/symbols/16x16/4.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:06:03.000000 mapdata-3.7.0/mapdata/symbols/16x16/5.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:28:02.000000 mapdata-3.7.0/mapdata/symbols/16x16/6.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:27.000000 mapdata-3.7.0/mapdata/symbols/16x16/7.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:40.000000 mapdata-3.7.0/mapdata/symbols/16x16/8.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:26:59.000000 mapdata-3.7.0/mapdata/symbols/16x16/9.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:04:26.000000 mapdata-3.7.0/mapdata/symbols/16x16/A.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:07:30.000000 mapdata-3.7.0/mapdata/symbols/16x16/B.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:10:14.000000 mapdata-3.7.0/mapdata/symbols/16x16/C.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:13:27.000000 mapdata-3.7.0/mapdata/symbols/16x16/D.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:14:22.000000 mapdata-3.7.0/mapdata/symbols/16x16/E.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:15:26.000000 mapdata-3.7.0/mapdata/symbols/16x16/F.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 00:14:24.000000 mapdata-3.7.0/mapdata/symbols/16x16/G.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:15:07.000000 mapdata-3.7.0/mapdata/symbols/16x16/H.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:16:00.000000 mapdata-3.7.0/mapdata/symbols/16x16/I.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:18:38.000000 mapdata-3.7.0/mapdata/symbols/16x16/J.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:21:25.000000 mapdata-3.7.0/mapdata/symbols/16x16/K.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:22:10.000000 mapdata-3.7.0/mapdata/symbols/16x16/L.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:24:58.000000 mapdata-3.7.0/mapdata/symbols/16x16/M.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:27:42.000000 mapdata-3.7.0/mapdata/symbols/16x16/N.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 14:04:25.000000 mapdata-3.7.0/mapdata/symbols/16x16/O.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:28:05.000000 mapdata-3.7.0/mapdata/symbols/16x16/P.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:29:12.000000 mapdata-3.7.0/mapdata/symbols/16x16/Q.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:30:16.000000 mapdata-3.7.0/mapdata/symbols/16x16/R.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:34:31.000000 mapdata-3.7.0/mapdata/symbols/16x16/S.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:35:37.000000 mapdata-3.7.0/mapdata/symbols/16x16/T.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:37:27.000000 mapdata-3.7.0/mapdata/symbols/16x16/U.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:40:22.000000 mapdata-3.7.0/mapdata/symbols/16x16/V.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:44:48.000000 mapdata-3.7.0/mapdata/symbols/16x16/W.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:46:24.000000 mapdata-3.7.0/mapdata/symbols/16x16/X.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:47:50.000000 mapdata-3.7.0/mapdata/symbols/16x16/Y.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:49:43.000000 mapdata-3.7.0/mapdata/symbols/16x16/Z.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-21 14:55:41.000000 mapdata-3.7.0/mapdata/symbols/16x16/airplane.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-06-24 15:22:11.000000 mapdata-3.7.0/mapdata/symbols/16x16/anchor.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:00:25.000000 mapdata-3.7.0/mapdata/symbols/16x16/ball.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2024-01-24 20:44:54.000000 mapdata-3.7.0/mapdata/symbols/16x16/ball_small.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-16 13:39:00.000000 mapdata-3.7.0/mapdata/symbols/16x16/bar.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:04:48.000000 mapdata-3.7.0/mapdata/symbols/16x16/bars.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:43:55.000000 mapdata-3.7.0/mapdata/symbols/16x16/binoculars.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:29:19.000000 mapdata-3.7.0/mapdata/symbols/16x16/bird.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      288 2023-04-24 16:37:43.000000 mapdata-3.7.0/mapdata/symbols/16x16/block.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2024-01-26 04:36:33.000000 mapdata-3.7.0/mapdata/symbols/16x16/block_small.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-16 18:31:20.000000 mapdata-3.7.0/mapdata/symbols/16x16/bookmark.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:29:01.000000 mapdata-3.7.0/mapdata/symbols/16x16/box_stack.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-04-30 14:46:15.000000 mapdata-3.7.0/mapdata/symbols/16x16/camera.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 16:51:47.000000 mapdata-3.7.0/mapdata/symbols/16x16/cancel.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-21 15:05:05.000000 mapdata-3.7.0/mapdata/symbols/16x16/car.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-21 15:04:37.000000 mapdata-3.7.0/mapdata/symbols/16x16/car2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-24 01:00:13.000000 mapdata-3.7.0/mapdata/symbols/16x16/center8.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:35:37.000000 mapdata-3.7.0/mapdata/symbols/16x16/check.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 14:51:14.000000 mapdata-3.7.0/mapdata/symbols/16x16/check_circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-16 14:20:03.000000 mapdata-3.7.0/mapdata/symbols/16x16/checkbox.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-04-28 13:31:04.000000 mapdata-3.7.0/mapdata/symbols/16x16/checkerboard.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:29:46.000000 mapdata-3.7.0/mapdata/symbols/16x16/chevrons.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:12:28.000000 mapdata-3.7.0/mapdata/symbols/16x16/circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:22:20.000000 mapdata-3.7.0/mapdata/symbols/16x16/circle_bar.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 14:58:14.000000 mapdata-3.7.0/mapdata/symbols/16x16/circle_plus.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:09:20.000000 mapdata-3.7.0/mapdata/symbols/16x16/circle_stipple.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 14:29:15.000000 mapdata-3.7.0/mapdata/symbols/16x16/circle_triangle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-25 14:40:36.000000 mapdata-3.7.0/mapdata/symbols/16x16/circle_wedge.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-06-24 14:56:37.000000 mapdata-3.7.0/mapdata/symbols/16x16/circle_x.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-07-04 17:10:15.000000 mapdata-3.7.0/mapdata/symbols/16x16/clock.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 14:05:41.000000 mapdata-3.7.0/mapdata/symbols/16x16/columns.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:50:11.000000 mapdata-3.7.0/mapdata/symbols/16x16/contract.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-04-16 17:48:39.000000 mapdata-3.7.0/mapdata/symbols/16x16/cross.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-23 18:45:40.000000 mapdata-3.7.0/mapdata/symbols/16x16/darkeye.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:32.000000 mapdata-3.7.0/mapdata/symbols/16x16/decrease.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-30 12:46:46.000000 mapdata-3.7.0/mapdata/symbols/16x16/deposition.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:47.000000 mapdata-3.7.0/mapdata/symbols/16x16/diag_ll.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:26.000000 mapdata-3.7.0/mapdata/symbols/16x16/diag_lr.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:05.000000 mapdata-3.7.0/mapdata/symbols/16x16/diag_ul.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:17:04.000000 mapdata-3.7.0/mapdata/symbols/16x16/diag_ur.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-20 18:41:19.000000 mapdata-3.7.0/mapdata/symbols/16x16/dialog.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-16 17:38:10.000000 mapdata-3.7.0/mapdata/symbols/16x16/diamond.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 13:47:24.000000 mapdata-3.7.0/mapdata/symbols/16x16/donkey.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 16:45:55.000000 mapdata-3.7.0/mapdata/symbols/16x16/dot.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:00:44.000000 mapdata-3.7.0/mapdata/symbols/16x16/down.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:38:22.000000 mapdata-3.7.0/mapdata/symbols/16x16/drop.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-03 02:15:55.000000 mapdata-3.7.0/mapdata/symbols/16x16/elephant.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 14:33:40.000000 mapdata-3.7.0/mapdata/symbols/16x16/expand.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 15:03:32.000000 mapdata-3.7.0/mapdata/symbols/16x16/eye.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 13:59:48.000000 mapdata-3.7.0/mapdata/symbols/16x16/fire.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:13:54.000000 mapdata-3.7.0/mapdata/symbols/16x16/fish.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:36:11.000000 mapdata-3.7.0/mapdata/symbols/16x16/flag.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-30 15:04:58.000000 mapdata-3.7.0/mapdata/symbols/16x16/flag2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 15:06:07.000000 mapdata-3.7.0/mapdata/symbols/16x16/four_arrows.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:25:14.000000 mapdata-3.7.0/mapdata/symbols/16x16/graph.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 15:18:19.000000 mapdata-3.7.0/mapdata/symbols/16x16/hand.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:04:09.000000 mapdata-3.7.0/mapdata/symbols/16x16/hash.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-03 01:53:41.000000 mapdata-3.7.0/mapdata/symbols/16x16/heart.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2024-01-31 04:51:54.000000 mapdata-3.7.0/mapdata/symbols/16x16/hidden.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:40:09.000000 mapdata-3.7.0/mapdata/symbols/16x16/hourglass.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 22:31:53.000000 mapdata-3.7.0/mapdata/symbols/16x16/house.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:05.000000 mapdata-3.7.0/mapdata/symbols/16x16/increase.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-24 23:05:40.000000 mapdata-3.7.0/mapdata/symbols/16x16/info.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:51:36.000000 mapdata-3.7.0/mapdata/symbols/16x16/leaf.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:02:45.000000 mapdata-3.7.0/mapdata/symbols/16x16/left.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-23 13:36:40.000000 mapdata-3.7.0/mapdata/symbols/16x16/lightbulb.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 16:38:25.000000 mapdata-3.7.0/mapdata/symbols/16x16/lightning.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:14:23.000000 mapdata-3.7.0/mapdata/symbols/16x16/lightning2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-07-04 16:58:13.000000 mapdata-3.7.0/mapdata/symbols/16x16/location_ptr.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:06:42.000000 mapdata-3.7.0/mapdata/symbols/16x16/mine.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 15:07:56.000000 mapdata-3.7.0/mapdata/symbols/16x16/nested_boxes.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:07:35.000000 mapdata-3.7.0/mapdata/symbols/16x16/pennant.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:16:09.000000 mapdata-3.7.0/mapdata/symbols/16x16/pennant2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-18 19:04:36.000000 mapdata-3.7.0/mapdata/symbols/16x16/people.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:26:34.000000 mapdata-3.7.0/mapdata/symbols/16x16/person.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:30:45.000000 mapdata-3.7.0/mapdata/symbols/16x16/person2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 18:43:50.000000 mapdata-3.7.0/mapdata/symbols/16x16/person3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 15:37:42.000000 mapdata-3.7.0/mapdata/symbols/16x16/phone.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:18:45.000000 mapdata-3.7.0/mapdata/symbols/16x16/photo.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-19 22:48:26.000000 mapdata-3.7.0/mapdata/symbols/16x16/picnic.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-19 03:57:15.000000 mapdata-3.7.0/mapdata/symbols/16x16/plus.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:16.000000 mapdata-3.7.0/mapdata/symbols/16x16/point_down.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:58:03.000000 mapdata-3.7.0/mapdata/symbols/16x16/point_left.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      362 2023-05-03 01:57:47.000000 mapdata-3.7.0/mapdata/symbols/16x16/point_right.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      347 2023-05-03 01:56:56.000000 mapdata-3.7.0/mapdata/symbols/16x16/point_up.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:58:38.000000 mapdata-3.7.0/mapdata/symbols/16x16/pointer_ne.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:59:20.000000 mapdata-3.7.0/mapdata/symbols/16x16/pointer_nw.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:54.000000 mapdata-3.7.0/mapdata/symbols/16x16/pointer_se.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:59:07.000000 mapdata-3.7.0/mapdata/symbols/16x16/pointer_sw.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 18:51:06.000000 mapdata-3.7.0/mapdata/symbols/16x16/puzzle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:52:56.000000 mapdata-3.7.0/mapdata/symbols/16x16/q1.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:57:59.000000 mapdata-3.7.0/mapdata/symbols/16x16/q1_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:25.000000 mapdata-3.7.0/mapdata/symbols/16x16/q2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:55.000000 mapdata-3.7.0/mapdata/symbols/16x16/q2_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:46.000000 mapdata-3.7.0/mapdata/symbols/16x16/q3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:28.000000 mapdata-3.7.0/mapdata/symbols/16x16/q3_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:57.000000 mapdata-3.7.0/mapdata/symbols/16x16/q4.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:13.000000 mapdata-3.7.0/mapdata/symbols/16x16/q4_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-05-20 18:36:19.000000 mapdata-3.7.0/mapdata/symbols/16x16/qmark_circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-20 18:37:52.000000 mapdata-3.7.0/mapdata/symbols/16x16/qmark_circle2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:43:45.000000 mapdata-3.7.0/mapdata/symbols/16x16/raincloud.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 16:39:34.000000 mapdata-3.7.0/mapdata/symbols/16x16/right.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 17:23:57.000000 mapdata-3.7.0/mapdata/symbols/16x16/rocket.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 17:25:43.000000 mapdata-3.7.0/mapdata/symbols/16x16/rocket2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-23 16:07:27.000000 mapdata-3.7.0/mapdata/symbols/16x16/rose.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-28 14:05:56.000000 mapdata-3.7.0/mapdata/symbols/16x16/rows.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 14:27:34.000000 mapdata-3.7.0/mapdata/symbols/16x16/scales.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-07-04 17:07:45.000000 mapdata-3.7.0/mapdata/symbols/16x16/search.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-07-04 17:08:06.000000 mapdata-3.7.0/mapdata/symbols/16x16/search2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-01 15:46:45.000000 mapdata-3.7.0/mapdata/symbols/16x16/skull.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-17 02:43:53.000000 mapdata-3.7.0/mapdata/symbols/16x16/square.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:26:56.000000 mapdata-3.7.0/mapdata/symbols/16x16/star.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:07:07.000000 mapdata-3.7.0/mapdata/symbols/16x16/stipple.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-03 02:10:57.000000 mapdata-3.7.0/mapdata/symbols/16x16/stop.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 15:31:50.000000 mapdata-3.7.0/mapdata/symbols/16x16/surprise_circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:22:10.000000 mapdata-3.7.0/mapdata/symbols/16x16/swamp.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:27:50.000000 mapdata-3.7.0/mapdata/symbols/16x16/target.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:37:09.000000 mapdata-3.7.0/mapdata/symbols/16x16/target2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-06-24 15:27:04.000000 mapdata-3.7.0/mapdata/symbols/16x16/ten.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 14:54:31.000000 mapdata-3.7.0/mapdata/symbols/16x16/trash.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-09 17:01:43.000000 mapdata-3.7.0/mapdata/symbols/16x16/tree.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 12:59:30.000000 mapdata-3.7.0/mapdata/symbols/16x16/tree2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:26:26.000000 mapdata-3.7.0/mapdata/symbols/16x16/tree3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-09 16:59:51.000000 mapdata-3.7.0/mapdata/symbols/16x16/triangle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-09 17:08:13.000000 mapdata-3.7.0/mapdata/symbols/16x16/triangle_open.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-05-20 17:46:38.000000 mapdata-3.7.0/mapdata/symbols/16x16/triangle_sm.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-04-16 18:01:12.000000 mapdata-3.7.0/mapdata/symbols/16x16/up.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-30 12:50:50.000000 mapdata-3.7.0/mapdata/symbols/16x16/vapor.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 03:55:52.000000 mapdata-3.7.0/mapdata/symbols/16x16/warning.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 20:02:51.000000 mapdata-3.7.0/mapdata/symbols/16x16/wave.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:01.000000 mapdata-3.7.0/mapdata/symbols/16x16/wave2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:43.000000 mapdata-3.7.0/mapdata/symbols/16x16/wave3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-30 14:42:04.000000 mapdata-3.7.0/mapdata/symbols/16x16/weather.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 16:37:24.000000 mapdata-3.7.0/mapdata/symbols/16x16/wedge.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:53:34.000000 mapdata-3.7.0/mapdata/symbols/16x16/wedge_sm.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-29 15:40:02.000000 mapdata-3.7.0/mapdata/symbols/16x16/wedges_3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:23:44.000000 mapdata-3.7.0/mapdata/symbols/16x16/well.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:20:04.000000 mapdata-3.7.0/mapdata/symbols/16x16/whale.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 12:54:47.000000 mapdata-3.7.0/mapdata/symbols/16x16/whale2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-24 15:49:53.000000 mapdata-3.7.0/mapdata/symbols/16x16/wheelchair.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:04:57.000000 mapdata-3.7.0/mapdata/symbols/16x16/zigzags.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-19 04:39:05.000000 mapdata-3.7.0/mapdata/symbols/16x16/zigzags2.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-27 14:16:15.609886 mapdata-3.7.0/mapdata/symbols/20x20/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      464 2023-06-24 14:14:12.000000 mapdata-3.7.0/mapdata/symbols/20x20/ball20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      467 2023-06-24 14:24:29.000000 mapdata-3.7.0/mapdata/symbols/20x20/block20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:13:06.000000 mapdata-3.7.0/mapdata/symbols/20x20/circle20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:11.000000 mapdata-3.7.0/mapdata/symbols/20x20/q1_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:22.000000 mapdata-3.7.0/mapdata/symbols/20x20/q2_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:35.000000 mapdata-3.7.0/mapdata/symbols/20x20/q3_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:54.000000 mapdata-3.7.0/mapdata/symbols/20x20/q4_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:24:00.000000 mapdata-3.7.0/mapdata/symbols/20x20/square20.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-27 14:16:15.613886 mapdata-3.7.0/mapdata/symbols/24x24/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      539 2023-06-24 14:20:48.000000 mapdata-3.7.0/mapdata/symbols/24x24/ball24.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      542 2023-06-24 14:25:39.000000 mapdata-3.7.0/mapdata/symbols/24x24/block24.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:20:00.000000 mapdata-3.7.0/mapdata/symbols/24x24/circle24.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:22:10.000000 mapdata-3.7.0/mapdata/symbols/24x24/square24.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-27 14:16:15.613886 mapdata-3.7.0/mapdata/symbols/28x28/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      793 2023-06-24 14:41:23.000000 mapdata-3.7.0/mapdata/symbols/28x28/ball28.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      794 2023-06-24 14:42:33.000000 mapdata-3.7.0/mapdata/symbols/28x28/block28.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:41:39.000000 mapdata-3.7.0/mapdata/symbols/28x28/circle28.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:42:15.000000 mapdata-3.7.0/mapdata/symbols/28x28/square28.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-05-27 14:16:15.613886 mapdata-3.7.0/mapdata.egg-info/
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     7898 2024-05-27 14:16:15.000000 mapdata-3.7.0/mapdata.egg-info/PKG-INFO
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     6598 2024-05-27 14:16:15.000000 mapdata-3.7.0/mapdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2024-05-27 14:16:15.000000 mapdata-3.7.0/mapdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      143 2024-05-27 14:16:15.000000 mapdata-3.7.0/mapdata.egg-info/requires.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        8 2024-05-27 14:16:15.000000 mapdata-3.7.0/mapdata.egg-info/top_level.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2024-05-27 14:16:15.613886 mapdata-3.7.0/setup.cfg
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     1813 2024-05-20 01:05:31.000000 mapdata-3.7.0/setup.py
```

### Comparing `mapdata-3.6.4/LICENSE.txt` & `mapdata-3.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapdata-3.6.4/PKG-INFO` & `mapdata-3.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 3.6.4
+Version: 3.7.0
 Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: cortice@tutanota.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,Spreadsheet,Database,PNG,JPG,Postscript
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mapdata-3.6.4/README.md` & `mapdata-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `mapdata-3.6.4/mapdata/configfile/mapdata.conf` & `mapdata-3.7.0/mapdata/configfile/mapdata.conf`

 * *Files identical despite different names*

### Comparing `mapdata-3.6.4/mapdata/mapdata.py` & `mapdata-3.7.0/mapdata/mapdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 # 	The GNU General Public License is available at <http://www.gnu.org/licenses/>
 #
 # AUTHOR
 #	Dreas Nielsen (RDN)
 #
 # ==================================================================
 
-version = "3.6.4"
-vdate = "2024-05-17"
+version = "3.7.1"
+vdate = "2024-05-25"
 
 copyright = "2023-2024"
 
 
 import sys
 import os.path
 import io
@@ -2378,15 +2378,15 @@
 		cur = data_db.cursor()
 		cur.execute("drop table if exists mapdata;")
 		colnames = db_colnames([r[0] for r in self.data_types])
 		colnames.append("treeviewid")
 		coltypes = [r[1] for r in self.data_types]
 		coltypes.append("int")
 		db_coltypes = [sqlite_type_x[t] for t in coltypes]
-		coldecs = ", ".join([c[0]+' '+c[1] for c in list(zip(colnames, db_coltypes))])
+		coldecs = ", ".join([dquote(c[0])+' '+c[1] for c in list(zip(colnames, db_coltypes))])
 		colrange = range(len(coltypes))
 		cur.execute("create table mapdata (%s);" % coldecs)
 		tbldata = []
 		castfuncs = [data_type_cast_fn(t) for t in coltypes]
 		for row_id in tv_table.get_children():
 			row = tv_table.item(row_id)["values"]
 			row.append(row_id)
@@ -2844,15 +2844,15 @@
 		clone.scatter_x_breaks = plot_obj.scatter_x_breaks
 		clone.scatter_y_breaks = plot_obj.scatter_y_breaks
 		clone.lineplot_breaks = plot_obj.lineplot_breaks
 		clone.lineplot_x_breaks = plot_obj.lineplot_x_breaks
 		clone.loess = plot_obj.loess
 		clone.linreg = plot_obj.linreg
 		clone.theilsen = plot_obj.theilsen
-		close.anot = plot_obj.annot
+		clone.anot = plot_obj.annot
 		clone.numeric_columns = copy.copy(plot_obj.numeric_columns)
 		clone.dataset = copy.copy(plot_obj.dataset)
 		clone.n_dataset_columns = copy.copy(plot_obj.n_dataset_columns)
 		clone.plot_data = copy.copy(plot_obj.plot_data)
 		clone.data_labels = copy.copy(plot_obj.data_labels)
 		clone.plot_data_labels = copy.copy(plot_obj.plot_data_labels)
 		clone.q_redraw(get_data=False)
@@ -3250,14 +3250,23 @@
 		dlg = PlotDialog(self, self.data_types)
 		self.plot_list.append(dlg)
 		dlg.show()
 	def pairplot(self, args=None):
 		dlg = PairPlotDialog(self, self.data_types)
 		self.plot_list.append(dlg)
 		dlg.show()
+	def rankabundplot(self, args=None):
+		bad_cols = [self.lat_col, self.lon_col]
+		if self.src_lat_col is not None:
+			bad_cols.extend([self.src_lat_col, self.src_lon_col])
+		if self.lat_4326_col is not None:
+			bad_cols.extend([self.lat_4326_col, self.lon_4326_col])
+		dlg = RankAbundDialog(self, self.data_types, bad_cols)
+		self.plot_list.append(dlg)
+		dlg.show()
 	def select_colocated(self, args=None):
 		dlg = ColocatedDialog()
 		matchstr, num, merge = dlg.show()
 		if matchstr is not None:
 			if matchstr == "more than":
 				comp = ">"
 			elif matchstr == "less than":
@@ -3562,16 +3571,17 @@
 		map_menu.add_command(label="Export", command = save_map, underline=1)
 		map_menu.add_command(label="Settings", command = change_map_settings, underline=0)
 		sel_menu.add_command(label="Invert", command = invert_selections, underline=0)
 		sel_menu.add_command(label="Un-select all", command = self.unselect_map, underline=0)
 		sel_menu.add_command(label="Data query", command = self.run_query, underline=5)
 		sel_menu.add_command(label="Co-located data", command = self.select_colocated, underline=0)
 		sel_menu.add_command(label="Random", command = self.select_random, underline=0)
-		plot_menu.add_command(label="New", command = self.new_plot, underline=0)
+		plot_menu.add_command(label="General", command = self.new_plot, underline=2)
 		plot_menu.add_command(label="Pair plot", command = self.pairplot, underline=0)
+		plot_menu.add_command(label="Rank-abundance plot", command = self.rankabundplot, underline=0)
 		plot_menu.add_command(label="Close all", command = self.close_all_plots, underline=0)
 		plot_menu.add_command(label="Settings", command = self.get_plot_config, underline=0)
 		stats_menu.add_command(label="Univariate statistics", command = univar_stats, underline=0)
 		stats_menu.add_command(label="Fit univariate distribution", command = fitdist_stats, underline=0)
 		stats_menu.add_command(label="Bivariate statistics", command = bivar_stats, underline=0)
 		stats_menu.add_command(label="Correlation matrix", command = corr_matrix, underline=0)
 		stats_menu.add_command(label="Contingency table", command = cont_table, underline=2)
@@ -6502,15 +6512,15 @@
 				self.bins = num_bins
 				self.q_redraw()
 	def set_alpha(self, *args):
 		if self.type_var.get() in ("Box plot", "Bubble plot", "Scatter plot", "Kernel density (KD) plot", "Line plot", "Normal Q-Q plot", "Stripchart", "Violin plot"):
 			dlg = OneFloatDialog(self.dlg, "Transparency", "Enter the transparency (alpha) value", min_value=0.0, max_value=1.0, initial=self.alpha)
 			new_alpha = dlg.show()
 			if new_alpha is not None:
-				self.alpha = new_alpha
+				self.alpha = min(1.0, max(new_alpha, 0.0))
 				self.q_redraw()
 	def set_scatter_breaks(self, *args):
 		# Toggle display of vertical and horizontal lines at natural breaks values on a scatter plot.
 		if self.type_var.get() == "Scatter plot":
 			self.scatter_breaks = not self.scatter_breaks
 			self.q_redraw()
 	def set_lineplot_breaks(self, *args):
@@ -6849,27 +6859,349 @@
 			matplotlib.rcParams['xtick.labelsize'] = orig_xsize
 			matplotlib.rcParams['ytick.labelsize'] = orig_ysize
 
 	def set_alpha(self, *args):
 		dlg = OneFloatDialog(self.dlg, "Transparency", "Enter the opacity (alpha) value", min_value=0.0, max_value=1.0, initial=self.alpha)
 		new_alpha = dlg.show()
 		if new_alpha is not None:
-			self.alpha = new_alpha
+			self.alpha = min(1.0, max(new_alpha, 0.0))
 			self.q_redraw()
 	def show(self):
 		self.dlg.wait_window(self.dlg)
 	def do_close(self, *args):
 		self.parent.remove_plot(self)
 		try:
 			self.dlg.destroy()
 		except:
 			pass
 
 
 
+class RankAbundDialog(object):
+	def __init__(self, parent, column_specs, prohibited_columns):
+		self.parent = parent
+		self.column_specs = column_specs
+		self.prohibited_columns = prohibited_columns
+		self.numeric_columns = [c[0] for c in self.column_specs if c[1] in ("int", "float") and not c[1] in prohibited_columns]
+		self.numeric_columns.sort()
+		self.string_columns = [c[0] for c in self.column_specs if c[1] == "string" and not c[1] in prohibited_columns]
+		self.string_columns.sort()
+		self.auto_update = True
+		self.alpha = 0.45
+		self.plot_title = None
+		self.xlabel = None
+		self.ylabel = None
+		self.dlg = tk.Toplevel()
+		self.dlg.title("Rank Abundance Plot")
+		self.loading_dlg = LoadingDialog(self.dlg)
+		self.alpha = 0.45
+		# Data
+		self.dataset = None
+		self.data_labels = None
+		self.plot_data = None
+		self.plot_data_labels = None
+		# Message
+		prompt_frame = tk.Frame(self.dlg, borderwidth=5)
+		prompt_frame.grid(row=0, column=0, sticky=tk.N+tk.EW, pady=(3,3))
+		prompt_frame.columnconfigure(0, weight=1)
+		msg_lbl = ttk.Label(prompt_frame, width=80, text="Select two or more variables from the list below, and a row identifier.")
+		msg_lbl.grid(row=0, column=0, sticky=tk.W, padx=(6,6), pady=(3,3))
+		def wrap_msg(event):
+			msg_lbl.configure(wraplength=event.width - 5)
+		msg_lbl.bind("<Configure>", wrap_msg)
+
+		# Controls
+		ctrl_frame = tk.Frame(self.dlg, borderwidth=5)
+		ctrl_frame.grid(row=1, column=0, sticky=tk.N+tk.EW)
+
+		self.sel_only_var = tk.StringVar(ctrl_frame, "0")
+		self.sel_only_ck = ttk.Checkbutton(ctrl_frame, text="Selected data only", variable=self.sel_only_var, command=self.q_redraw,
+				onvalue="1", offvalue="0")
+		self.sel_only_ck.grid(row=0, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
+
+		self.autoupdate_var = tk.StringVar(ctrl_frame, "1")
+		self.autoupdate_ck = ttk.Checkbutton(ctrl_frame, text="Auto-update", command=self.set_autoupdate, variable=self.autoupdate_var,
+				onvalue="1", offvalue="0")
+		self.autoupdate_ck.grid(row=0, column=1, sticky=tk.W, padx=(3,3), pady=(3,3))
+
+		self.ylog_var = tk.StringVar(ctrl_frame, "0")
+		self.ylog_ck = ttk.Checkbutton(ctrl_frame, text="Log Y axis", state=tk.NORMAL, command=self.q_redraw, variable=self.ylog_var,
+				onvalue="1", offvalue="0")
+		self.ylog_ck.grid(row=0, column=3, sticky=tk.W, padx=(6,6), pady=(3,3))
+
+		# Frame for input selection and output plot
+		self.content_frame = tk.Frame(self.dlg)
+		self.content_frame.grid(row=2, column=0, sticky=tk.NSEW)
+		self.dlg.rowconfigure(2, weight=1)
+		self.dlg.columnconfigure(0, weight=1)
+		self.content_frame.rowconfigure(0, weight=1)
+		self.content_frame.columnconfigure(0, weight=1)
+
+		# PanedWindow within content_frame: left is input listbox and other data selection controls, right is plot
+		io_panes = ttk.PanedWindow(self.content_frame, orient=tk.HORIZONTAL)
+		io_panes.grid(row=0, column=0, sticky=tk.NSEW)
+
+		self.inp_frame = tk.Frame(io_panes, borderwidth=3, relief=tk.RIDGE)
+		self.inp_frame.grid(row=0, column=0, sticky=tk.NSEW)
+		self.inp_frame.rowconfigure(0, weight=1)
+		self.inp_frame.columnconfigure(0, weight=1)
+		io_panes.add(self.inp_frame, weight=1)
+
+		self.output_frame = tk.Frame(io_panes, borderwidth=3, relief=tk.RIDGE)
+		self.output_frame.grid(row=0, column=1, sticky=tk.NSEW)
+		self.output_frame.rowconfigure(0, weight=1)
+		self.output_frame.columnconfigure(0, weight=1)
+		io_panes.add(self.output_frame, weight=4)
+
+		# Variable selection
+		# Add multi-select list of numeric variables to the leftmost pane
+		var_frame = tk.Frame(self.inp_frame)
+		var_frame.grid(row=0, column=0, columnspan=2, sticky=tk.NSEW)
+		var_frame.rowconfigure(0, weight=1)
+		var_frame.columnconfigure(0, weight=1)
+		self.column_frame, self.column_table = treeview_table(var_frame, rowset=[[v] for v in self.numeric_columns], \
+				column_headers=['Variable'], select_mode=tk.EXTENDED, nrows=min(10, len(self.numeric_columns)))
+		self.column_frame.grid(row=0, column=0, sticky=tk.NSEW)
+		self.column_table.bind('<ButtonRelease-1>', self.q_redraw)
+
+		# Grouping selection
+		self.groupby_var = tk.StringVar(self.inp_frame, "")
+		groupby_lbl = ttk.Label(self.inp_frame, text="Group by:")
+		groupby_lbl.grid(row=1, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
+		self.groupby_sel = ttk.Combobox(self.inp_frame, state=tk.NORMAL, textvariable=self.groupby_var, values=[""]+self.string_columns, width=24)
+		self.groupby_sel.grid(row=1, column=1, sticky=tk.W, padx=(3,6), pady=(3,3))
+		self.groupby_sel.bind("<<ComboboxSelected>>", self.q_redraw)
+
+		# Output plot
+		plot_frame = tk.Frame(self.output_frame)
+		plot_frame.rowconfigure(0, weight=1)
+		plot_frame.columnconfigure(0, weight=1)
+		plot_frame.pack(side=tk.TOP, fill=tk.BOTH, expand=1)
+		self.plotfig = Figure(dpi=100)
+		self.plotfig.set_figheight(3.5)
+		self.plotfig.set_figwidth(3.5)
+		self.plotfig_canvas = FigureCanvasTkAgg(self.plotfig, plot_frame)
+		self.plot_nav = NavigationToolbar2Tk(self.plotfig_canvas, plot_frame)
+		self.plot_axes = self.plotfig.add_subplot(111)
+		self.plotfig_canvas.get_tk_widget().pack(side=tk.TOP, fill=tk.BOTH, expand=1)
+		self.plot_nav.update()
+
+		# Buttons
+		btn_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
+		btn_frame.columnconfigure(0, weight=1)
+		btn_frame.grid(row=3, column=0, sticky=tk.EW, pady=(3,3))
+		btn_frame.columnconfigure(0, weight=0)
+		btn_frame.columnconfigure(1, weight=0)
+		btn_frame.columnconfigure(2, weight=1)
+		self.canceled = False
+		self.help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help, underline=0)
+		self.help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
+		self.dlg.bind("<Alt-h>", self.do_help)
+		self.data_btn = ttk.Button(btn_frame, text="Source Data", state=tk.DISABLED, command=self.show_data, underline=0)
+		self.data_btn.grid(row=0, column=1, sticky=tk.W, padx=(3,3))
+		self.plot_data_btn = ttk.Button(btn_frame, text="Plot Data", state=tk.DISABLED, command=self.show_plot_data, underline=0)
+		self.plot_data_btn.grid(row=0, column=2, sticky=tk.W, padx=(3,3))
+		close_btn = ttk.Button(btn_frame, text="Close", command=self.do_close, underline=0)
+		close_btn.grid(row=0, column=2, sticky=tk.E, padx=(6,6))
+		self.dlg.bind("<Alt-c>", self.do_close)
+		self.dlg.bind("<Escape>", self.do_close)
+
+		# Initialize output frames
+		self.clear_output()
+
+		center_window(self.dlg)
+		raise_window(self.dlg)
+
+	def do_help(self, *args):
+		webbrowser.open("https://mapdata.readthedocs.io/en/latest/dialogs.html#rank-abundance-plot", new=2, autoraise=True)
+
+	def set_autoupdate(self):
+		if self.autoupdate_var.get() == "1":
+			self.auto_update = True
+		else:
+			self.auto_update = False
+
+	def q_redraw(self, *args):
+		# At least two variables must be selected
+		self.clear_output()
+		curr_selections = self.column_table.selection()
+		if len(curr_selections) > 1:
+			self.get_data()
+			if self.dataset is not None:
+				self.redraw()
+
+	def get_data(self):
+		self.data_btn["state"] = tk.DISABLED
+		self.plot_data_btn["state"] = tk.DISABLED
+		self.dataset = None
+		column_list = []
+		for sel_row in self.column_table.selection():
+			datarow = self.column_table.item(sel_row)["values"]
+			column_list.append(datarow[0])
+		# Record the number of data columns without labels.
+		self.n_dataset_columns = len(column_list)
+		# Add the grouping column -- ALWAYS immediately after the variable columns for indexing consistency
+		if self.groupby_var.get() != "":
+			column_list.append(self.groupby_var.get())
+		# Get additional map labeling column if specified
+		if map_settings.label_col is not None:
+			column_list.append(map_settings.label_col)
+		# Get the selected data.
+		if self.sel_only_var.get() == "1":
+			dataset = self.parent.get_sel_data(column_list)
+		else:
+			dataset = self.parent.get_all_data(column_list)
+		if dataset is None:
+			self.dataset = None
+			self.data_labels = None
+		else:
+			# Convert to floats for numeric data columns only
+			for i in range(self.n_dataset_columns):
+				if column_list[i] in self.numeric_columns:
+					dataset[i] = [conv_float(v) for v in dataset[i]]
+			self.dataset = dataset
+			self.data_labels = column_list
+			self.data_btn["state"] = tk.NORMAL
+			self.dlg.bind("<Alt-x>", self.set_xlabel)
+			self.dlg.bind("<Alt-y>", self.set_ylabel)
+
+	def clear_output(self):
+		self.dlg.bind("<Alt-a>")
+		self.dlg.bind("<Alt-s>")
+		self.dlg.bind("<Alt-x>")
+		self.dlg.bind("<Alt-y>")
+		self.dlg.bind("<Control-s>")
+		self.plot_data_btn["state"] = tk.DISABLED
+		self.plotfig.clear()
+		self.plot_axes = self.plotfig.add_subplot(111)
+		self.plotfig_canvas.draw()
+
+	def redraw(self):
+		self.clear_output()
+		ranks = list(range(1, self.n_dataset_columns+1))
+		# Sum abundances for each selected variable column, across all rows or across groups
+		ylbl = "Relative Abundance (Value)"
+		if self.ylog_var.get() == '1':
+			ylbl = "Log10 of Relative Abundance (Value)"
+		groupvar = self.groupby_var.get()
+		if groupvar != "":
+			# Sum each column by the grouping variable, producing a dictionary of lists
+			grps = sorted(list(set(self.dataset[self.n_dataset_columns])))
+			grpsums = {}
+			for g in grps:
+				grpsums[g] = [0] * self.n_dataset_columns
+			for i in range(len(self.dataset[0])):
+				grp = self.dataset[self.n_dataset_columns][i]
+				for j in range(self.n_dataset_columns):
+					if self.dataset[j][i] is not None:
+						grpsums[grp][j] = grpsums[grp][j] + self.dataset[j][i]
+			# For each group, calculate the total for the list, standardize each value, and sort from largest to smallest
+			dictstd = {}
+			for k in grpsums.keys():
+				dsums = grpsums[k]
+				dsumsum = sum(dsums)
+				if dsumsum > 0:
+					dstd = [d/dsumsum for d in dsums]
+					dstd.sort(reverse=True)
+					if self.ylog_var.get() == '1':
+						dstd = [math.log10(d) if d > 0 else None for d in dstd]
+					dictstd[k] = dstd
+			if len(dictstd) > 0:
+				# Create the plotdata set
+				self.plot_data_labels = ["Rank"] + list(dictstd.keys())
+				self.plot_data = [ranks] + [dictstd[k] for k in dictstd.keys()]
+				self.plot_data_btn["state"] = tk.NORMAL
+				# Legend
+				# Create a line plot for each row
+				for i in range(len(self.plot_data_labels)-1):
+					self.plot_axes.plot(self.plot_data[0], self.plot_data[i+1], label=self.plot_data_labels[i+1], alpha=self.alpha)
+				if len(self.plot_data_labels)-1 > 1:
+					self.plot_axes.legend()
+		else:
+			# Sum each column across all rows, producing a list
+			dsums = [0] * self.n_dataset_columns
+			for i in range(len(self.dataset[0])):
+				for j in range(self.n_dataset_columns):
+					if self.dataset[j][i] is not None:
+						dsums[j] = dsums[j] + self.dataset[j][i]
+			# Calculate the total for the list, standardize each value, and sort from largest to smallest
+			dsumsum = sum(dsums)
+			if dsumsum > 0:
+				dstd = [d/dsumsum for d in dsums]
+				dstd.sort(reverse=True)
+				if self.ylog_var.get() == '1':
+					dstd = [math.log10(d) if d > 0 else None for d in dstd]
+				# Create the plotdata set
+				self.plot_data = [ranks, dstd]
+				self.plot_data_labels = ["Rank", ylbl]
+				self.plot_data_btn["state"] = tk.NORMAL
+				# Create a line plot
+				self.plot_axes.plot(self.plot_data[0], self.plot_data[1], alpha=self.alpha)
+		self.plot_axes.set_xlabel(self.xlabel or self.plot_data_labels[0])
+		self.plot_axes.set_ylabel(self.ylabel or ylbl)
+		if self.plot_title is not None:
+			self.plot_axes.set_title(self.plot_title)
+		self.plotfig_canvas.draw()
+		self.plot_nav.update()
+		self.dlg.bind("<Alt-a>", self.set_alpha)
+
+	def show_data(self, *args):
+		if self.dataset is not None:
+			show_columnar_table(self.dlg, "Source Data", "Selected data:", self.dataset, self.data_labels, "Data for Rank-Value Plot")
+			self.dlg.lift()
+
+	def show_plot_data(self, *args):
+		# Show data as summarized for a particular plot type.
+		if self.plot_data is not None:
+			show_columnar_table(self.dlg, "Data for Plotting", "Data to be plotted:", self.plot_data, \
+					self.plot_data_labels, "Plot data")
+			self.dlg.lift()
+	
+	def set_alpha(self, *args):
+		dlg = OneFloatDialog(self.dlg, "Transparency", "Enter the transparency (alpha) value", min_value=0.0, max_value=1.0, initial=self.alpha)
+		new_alpha = dlg.show()
+		if new_alpha is not None:
+			self.alpha = min(1.0, max(new_alpha, 0.0))
+			self.q_redraw()
+	def set_title(self, *args):
+		dlg = OneEntryDialog(self.dlg, "Plot Title", "Enter a title for the plot:")
+		title = dlg.show()
+		if title is not None:
+			self.plot_title = title
+			self.plot_axes.set_title(title)
+			self.plot_axes.title.set_visible(True)
+			self.plotfig_canvas.draw()
+	def set_xlabel(self, *args):
+		dlg = OneEntryDialog(self.dlg, "X-Axis Label", "Enter a label for the X-axis:")
+		xlabel = dlg.show()
+		if xlabel is not None:
+			self.xlabel = xlabel
+			self.plot_axes.set_xlabel(xlabel)
+			self.plotfig_canvas.draw()
+	def set_ylabel(self, *args):
+		dlg = OneEntryDialog(self.dlg, "Y-Axis Label", "Enter a label for the Y-axis label:")
+		ylabel = dlg.show()
+		if ylabel is not None:
+			self.ylabel = ylabel
+			self.plot_axes.set_ylabel(ylabel)
+			self.plotfig_canvas.draw()
+
+	def show(self):
+		center_window(self.dlg)
+		self.dlg.deiconify()
+		raise_window(self.dlg)
+		self.dlg.wait_window(self.dlg)
+	def do_close(self, *args):
+		self.parent.remove_plot(self)
+		try:
+			self.dlg.destroy()
+		except:
+			pass
+
+
 
 class UnivarStatsDialog(object):
 	def __init__(self, parent, column_specs):
 		self.parent = parent
 		self.column_specs = column_specs
 		self.dlg = tk.Toplevel()
 		self.dlg.title("Univariate Statistics")
@@ -7620,15 +7952,15 @@
 			self.dlg.bind("<Control-s>", self.save_table)
 			self.dlg.minsize(width=900, height=500)
 
 	def set_alpha(self, *args):
 		dlg = OneFloatDialog(self.dlg, "Transparency", "Enter the opacity (alpha) value", min_value=0.0, max_value=1.0, initial=self.alpha)
 		new_alpha = dlg.show()
 		if new_alpha is not None:
-			self.alpha = new_alpha
+			self.alpha = min(1.0, max(new_alpha, 0.0))
 			self.q_recalc()
 	def set_title(self, *args):
 		dlg = OneEntryDialog(self.dlg, "Plot Title", "Enter a title for the plot:")
 		title = dlg.show()
 		if title is not None:
 			self.plot_title = title
 			self.plot_axes.set_title(title)
@@ -7674,14 +8006,16 @@
 		self.dlg.columnconfigure(0, weight=1)
 		#self.dlg.bind("<FocusIn>", self.q_redraw)
 		# Data
 		self.dataset = None
 		self.data_labels = None
 		self.numeric_columns = [c[0] for c in self.column_specs if c[1] in ("int", "float")]
 		self.numeric_columns.sort()
+		self.show_labels = True
+		self.dlg.bind("<Alt-l>")
 		self.dlg.bind("<Control-s>")
 		# Message
 		prompt_frame = tk.Frame(self.dlg, borderwidth=5)
 		prompt_frame.grid(row=0, column=0, sticky=tk.N+tk.EW, pady=(3,3))
 		prompt_frame.columnconfigure(0, weight=1)
 		msg_lbl = ttk.Label(prompt_frame, width=65, text="Select two or more variables from the left to see the correlation matrix.  Use Ctrl-click or Shift-click to select multiple rows.")
 		msg_lbl.grid(row=0, column=0, sticky=tk.W, padx=(6,6), pady=(3,3))
@@ -7776,25 +8110,25 @@
 
 	def clear_output(self):
 		self.plotfig.clear()
 		self.plot_axes = self.plotfig.add_subplot(111)
 		self.plotfig_canvas.draw()
 
 	def q_redraw(self, get_data=True, *args):
+		self.clear_output()
 		if self.dataset is None or get_data:
-			self.clear_output()
 			self.get_data()
 		if self.dataset is not None and len(self.dataset) > 1 and len(self.dataset[0]) > 1:
 			self.redraw()
 		else:
-			self.clear_output()
 			self.data_btn["state"] = tk.DISABLED
 
 	def get_data(self):
 		# Get the selected data into 'dataset'
+		self.clear_output()
 		self.dataset = None
 		column_list = []
 		for sel_row in self.column_table.selection():
 			datarow = self.column_table.item(sel_row)["values"]
 			column_list.append(datarow[0])
 		if len(column_list) > 0:
 			# Get either only the selected data or all data.
@@ -7849,14 +8183,15 @@
 			self.data_labels = clean_labels
 			self.data_btn["state"] = tk.NORMAL
 
 
 	def redraw(self):
 		# (Re)draw the correlation matrix
 		if self.data_labels is not None and len(self.data_labels) > 1:
+			self.dlg.bind("<Alt-l>", self.set_labeling)
 			nvar = len(self.data_labels)
 			corrmat = np.eye(nvar)
 			corrtype = self.corr_type_var.get()
 			if corrtype == "Pearson r":
 				corrfn = pearsonstat
 			elif corrtype == "Spearman rho":
 				corrfn = spearmanstat
@@ -7871,22 +8206,26 @@
 						corrcoeff = corrfn(dmat[i], dmat[j])
 						corrmat[i][j] = corrcoeff
 						corrmat[j][i] = corrcoeff
 			caxes = self.plot_axes.matshow(corrmat, cmap="BrBG", vmin=-1.0, vmax=1.0)
 			self.plotfig.colorbar(caxes)
 			self.plot_axes.set_xticks(range(nvar), labels=self.data_labels, rotation=25)
 			self.plot_axes.set_yticks(range(nvar), labels=self.data_labels)
-			for i in range(nvar):
-				for j in range(nvar):
-					v = corrmat[i,j]
-					c = "white" if abs(v) > 0.40 else "black"
-					self.plot_axes.text(j, i, f"{corrmat[i,j]:.2f}", ha="center", va="center", color=c)
+			if self.show_labels:
+				for i in range(nvar):
+					for j in range(nvar):
+						v = corrmat[i,j]
+						c = "white" if abs(v) > 0.40 else "black"
+						self.plot_axes.text(j, i, f"{corrmat[i,j]:.2f}", ha="center", va="center", color=c)
 			self.plot_axes.set_title(corrtype)
 			self.plotfig_canvas.draw()
 
+	def set_labeling(self, *args):
+		self.show_labels = not self.show_labels
+		self.q_redraw(get_data=False)
 	def show(self):
 		self.dlg.wait_window(self.dlg)
 	def do_close(self, *args):
 		self.parent.remove_corrmat(self)
 		try:
 			self.dlg.destroy()
 		except:
@@ -7904,14 +8243,17 @@
 		self.plot_title = None
 		self.dlg = tk.Toplevel()
 		self.dlg.title("t-SNE Analysis")
 		self.loading_dlg = LoadingDialog(self.dlg)
 		self.alpha = 0.45
 		self.tsne_coords = None
 		self.tsne_labels = None
+		# Hover annotation for scatter plots
+		self.annot = None
+		self.canvas_conn_id = None
 		# Data
 		self.dataset = None
 		self.data_labels = None
 		self.numeric_columns = [c[0] for c in self.column_specs if c[1] in ("int", "float")]
 		self.numeric_columns.sort()
 		self.categ_columns = [c[0] for c in self.column_specs if c[1] == "string"]
 		self.categ_columns.sort()
@@ -7935,14 +8277,23 @@
 		self.sel_only_ck.grid(row=0, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
 
 		self.autoupdate_var = tk.StringVar(ctrl_frame, "1")
 		self.autoupdate_ck = ttk.Checkbutton(ctrl_frame, text="Auto-update", command=self.set_autoupdate, variable=self.autoupdate_var,
 				onvalue="1", offvalue="0")
 		self.autoupdate_ck.grid(row=0, column=1, sticky=tk.W, padx=(3,3), pady=(3,3))
 
+		cleantype_frame = tk.Frame(ctrl_frame)
+		cleantype_frame.grid(row=1, column=0, columnspan=2, sticky=tk.NSEW)
+		self.cleantype_var = tk.StringVar(cleantype_frame, "Variables")
+		ttk.Label(cleantype_frame, text="Remove missing values by").grid(row=0, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
+		self.cleantype_sel = ttk.Combobox(cleantype_frame, state=tk.NORMAL, textvariable=self.cleantype_var, values=["Cases","Variables"], width=10)
+		self.cleantype_sel.bind('<<ComboboxSelected>>', self.q_recalc)
+		self.cleantype_sel.grid(row=0, column=1, sticky=tk.W, padx=(3,6), pady=(3,3))
+		cleantype_frame.columnconfigure(1, weight=1)
+
 		# Frame for input selection and output plot
 		self.content_frame = tk.Frame(self.dlg)
 		self.content_frame.grid(row=2, column=0, sticky=tk.NSEW)
 		self.dlg.rowconfigure(2, weight=1)
 		self.dlg.columnconfigure(0, weight=1)
 		self.content_frame.rowconfigure(0, weight=1)
 		self.content_frame.columnconfigure(0, weight=1)
@@ -7957,15 +8308,15 @@
 		self.inp_frame.columnconfigure(0, weight=1)
 		io_panes.add(self.inp_frame, weight=1)
 
 		self.output_frame = tk.Frame(io_panes, borderwidth=3, relief=tk.RIDGE)
 		self.output_frame.grid(row=0, column=1, sticky=tk.NSEW)
 		self.output_frame.rowconfigure(0, weight=1)
 		self.output_frame.columnconfigure(0, weight=1)
-		io_panes.add(self.output_frame, weight=1)
+		io_panes.add(self.output_frame, weight=4)
 
 		# Variable selection
 		# Add multi-select list of variables to the leftmost pane
 		var_frame = tk.Frame(self.inp_frame)
 		var_frame.grid(row=0, column=0, sticky=tk.NSEW)
 		var_frame.rowconfigure(0, weight=1)
 		var_frame.columnconfigure(0, weight=1)
@@ -8100,39 +8451,64 @@
 			self.data_rowids = self.parent.get_all_rowids()
 		if dataset is None or len(dataset[0]) < 6:
 			self.dataset = None
 			self.data_labels = None
 			self.data_btn["state"] = tk.DISABLED
 			self.calc_btn["state"] = tk.DISABLED
 		else:
-			# Remove missing data
-			column_indexes = range(len(dataset))
-			clean_data = [[] for _ in dataset]
-			clean_rowids = []
-			for i in range(len(dataset[0])):
-				ok = True
-				for col in column_indexes:
-					if dataset[col][i] is None or dataset[col][i] == '':
-						ok = False
-				if ok:
+			# Remove missing data, either by variables or cases.  This may lead to eliminating the data set.
+			if self.cleantype_var.get() == "Cases":
+				column_indexes = range(len(dataset))
+				clean_data = [[] for _ in dataset]
+				clean_rowids = []
+				for i in range(len(dataset[0])):
+					ok = True
 					for col in column_indexes:
-						clean_data[col].append(dataset[col][i])
-					clean_rowids.append(self.data_rowids[i])
-			self.data_rowids = clean_rowids
-			dataset = None
-			# Convert to floats for numeric data only
-			for i in range(len(clean_data)):
-				if column_list[i] in self.numeric_columns:
-					clean_data[i] = [conv_float(v) for v in clean_data[i]]
-			#
-			self.dataset = sort_columns(clean_data)
-			self.data_labels = column_list
-			self.data_btn["state"] = tk.NORMAL
-			self.calc_btn["state"] = tk.NORMAL
-			self.dtable_btn["state"] = tk.DISABLED
+						if dataset[col][i] is None or dataset[col][i] == '':
+							ok = False
+					if ok:
+						for col in column_indexes:
+							clean_data[col].append(dataset[col][i])
+						clean_rowids.append(self.data_rowids[i])
+				self.data_rowids = clean_rowids
+				dataset = clean_data
+			else:
+				badcols = []
+				for col in range(self.n_dataset_columns):
+					if not all(dataset[col]):
+						badcols.append(col)
+				if len(badcols) > 0:
+					badcols.reverse()
+					for bc in badcols:
+						del dataset[bc]
+						del column_list[bc]
+						if self.label_col is not None:
+							self.label_col -= 1
+					if self.groupby_col is not None:
+						self.groupby_col = len(column_list)
+					self.n_dataset_columns = self.n_dataset_columns - len(badcols)
+			if dataset is not None and len(dataset) > 0 and self.n_dataset_columns > 0:
+				# Convert to floats for numeric data only
+				for i in range(self.n_dataset_columns):
+					if column_list[i] in self.numeric_columns:
+						dataset[i] = [conv_float(v) for v in dataset[i]]
+			if dataset is None or self.n_dataset_columns < 3 or len(dataset[0]) < 6:
+				self.dataset = None
+				self.data_labels = None
+				self.data_btn["state"] = tk.DISABLED
+				self.calc_btn["state"] = tk.DISABLED
+				self.loading_dlg.hide()
+				warning("The dataset must have at least 3 variables and 6 cases for t-SNE analysis", {'parent':self.dlg})
+			else:
+				self.dataset = sort_columns(dataset)
+				self.data_labels = column_list
+				self.data_btn["state"] = tk.NORMAL
+				self.calc_btn["state"] = tk.NORMAL
+				self.dtable_btn["state"] = tk.DISABLED
+
 
 	def clear_output(self):
 		self.dlg.bind("<Alt-a>")
 		self.dlg.bind("<Alt-s>")
 		self.dlg.bind("<Control-s>")
 		self.data_btn["state"] = tk.DISABLED
 		self.dtable_btn["state"] = tk.DISABLED
@@ -8141,82 +8517,83 @@
 		self.plotfig_canvas.draw()
 
 	def recalculate(self):
 		self.loading_dlg.display("Calculating t-SNE")
 		self.clear_output()
 		from sklearn.manifold import TSNE
 		self.get_data()
-		d = np.array(columns_to_rows(self.dataset[0:self.n_dataset_columns]))
-		perp = self.perp_var.get()
-		if perp > len(self.dataset[0]) - 1:
-			perp = min(50, math.floor(len(self.dataset[0])/2))
-			self.perp_var.set(perp)
-		tsne = TSNE(n_components=2, perplexity=perp)
-		tsne_result = tsne.fit_transform(d)
-		self.tsne_coords = [tsne_result[:,0], tsne_result[:,1]]
-		self.tsne_labels = ["Dimension 1", "Dimension 2"]
-		self.dtable_btn["state"] = tk.NORMAL
-		# Single or grouped scatter plot
-		if self.groupby_col is None:
-			splot = self.plot_axes.scatter(self.tsne_coords[0], self.tsne_coords[1], alpha=self.alpha)
-			self.plot_handle_list = []
-			self.plot_label_list = []
-		else:
-			groups = sorted([str(x) for x in list(set(self.dataset[self.groupby_col-1]))])
-			cmap = map_colors(groups)
-			colors = [cmap[str(g)] for g in self.dataset[self.groupby_col-1]]
-			splot = self.plot_axes.scatter(self.tsne_coords[0], self.tsne_coords[1], c=colors, alpha=self.alpha)
-			# Custom legend handle for grouped scatter plot
-			lbls = list(cmap.keys())
-			if wrap_at_underscores:
-				lbls = [l.replace("_", " ") for l in lbls]
-			lbls = ["\n".join(textwrap.wrap(l, width=wrapwidth)) for l in lbls]
-			colkey = list(cmap.values())
-			symbs = [matplotlib.lines.Line2D([], [], marker='o', color=colkey[i], label=lbls[i], linestyle='None') for i in range(len(lbls))]
-			self.plot_handle_list = symbs
-			self.plot_label_list = lbls
-		# Hover annotation
-		def update_annot(ind):
-			pos = splot.get_offsets()[ind["ind"][0]]
-			self.annot.xy = pos
-			text = ", ".join([str(self.dataset[self.label_col-1][n]) for n in ind["ind"]])
-			self.annot.set_text(text)
-			self.annot.get_bbox_patch().set_facecolor("wheat")
-			self.annot.get_bbox_patch().set_alpha(0.8)
-		def hover(event):
-			vis = self.annot.get_visible()
-			if event.inaxes == self.plot_axes:
-				cont, ind = splot.contains(event)
-				if cont:
-					update_annot(ind)
-					self.annot.set_visible(True)
-				else:
-					if vis:
-						self.annot.set_visible(False)
-				self.plotfig_canvas.draw_idle()
-		if self.label_col is not None:
-			self.annot = self.plot_axes.annotate("", xy=(0,0), xytext=(8,12), textcoords="offset points", \
-					bbox={"boxstyle": "round", "fc": "w"}, arrowprops={"arrowstyle": "->"})
-			self.annot.set_visible(False)
-			self.canvas_conn_id = self.plotfig_canvas.mpl_connect("motion_notify_event", hover)
-		else:
-			if self.canvas_conn_id is not None:
-				self.plotfig_canvas.mpl_disconnect(self.canvas_conn_id)
-		# Legend
-		if len(self.plot_handle_list) > 0:
-			self.plot_axes.legend(handles=self.plot_handle_list, labels=self.plot_label_list)
+		if self.dataset is not None and len(self.dataset[0]) > 5:
+			d = np.array(columns_to_rows(self.dataset[0:self.n_dataset_columns]))
+			perp = self.perp_var.get()
+			if perp > len(self.dataset[0]) - 1:
+				perp = min(50, math.floor(len(self.dataset[0])/2))
+				self.perp_var.set(perp)
+			tsne = TSNE(n_components=2, perplexity=perp)
+			tsne_result = tsne.fit_transform(d)
+			self.tsne_coords = [tsne_result[:,0], tsne_result[:,1]]
+			self.tsne_labels = ["Dimension 1", "Dimension 2"]
+			self.dtable_btn["state"] = tk.NORMAL
+			# Single or grouped scatter plot
+			if self.groupby_col is None:
+				splot = self.plot_axes.scatter(self.tsne_coords[0], self.tsne_coords[1], alpha=self.alpha)
+				self.plot_handle_list = []
+				self.plot_label_list = []
+			else:
+				groups = sorted([str(x) for x in list(set(self.dataset[self.groupby_col-1]))])
+				cmap = map_colors(groups)
+				colors = [cmap[str(g)] for g in self.dataset[self.groupby_col-1]]
+				splot = self.plot_axes.scatter(self.tsne_coords[0], self.tsne_coords[1], c=colors, alpha=self.alpha)
+				# Custom legend handle for grouped scatter plot
+				lbls = list(cmap.keys())
+				if wrap_at_underscores:
+					lbls = [l.replace("_", " ") for l in lbls]
+				lbls = ["\n".join(textwrap.wrap(l, width=wrapwidth)) for l in lbls]
+				colkey = list(cmap.values())
+				symbs = [matplotlib.lines.Line2D([], [], marker='o', color=colkey[i], label=lbls[i], linestyle='None') for i in range(len(lbls))]
+				self.plot_handle_list = symbs
+				self.plot_label_list = lbls
+			# Hover annotation
+			def update_annot(ind):
+				pos = splot.get_offsets()[ind["ind"][0]]
+				self.annot.xy = pos
+				text = ", ".join([str(self.dataset[self.label_col-1][n]) for n in ind["ind"]])
+				self.annot.set_text(text)
+				self.annot.get_bbox_patch().set_facecolor("wheat")
+				self.annot.get_bbox_patch().set_alpha(0.8)
+			def hover(event):
+				vis = self.annot.get_visible()
+				if event.inaxes == self.plot_axes:
+					cont, ind = splot.contains(event)
+					if cont:
+						update_annot(ind)
+						self.annot.set_visible(True)
+					else:
+						if vis:
+							self.annot.set_visible(False)
+					self.plotfig_canvas.draw_idle()
+			if self.label_col is not None:
+				self.annot = self.plot_axes.annotate("", xy=(0,0), xytext=(8,12), textcoords="offset points", \
+						bbox={"boxstyle": "round", "fc": "w"}, arrowprops={"arrowstyle": "->"})
+				self.annot.set_visible(False)
+				self.canvas_conn_id = self.plotfig_canvas.mpl_connect("motion_notify_event", hover)
+			else:
+				if self.canvas_conn_id is not None:
+					self.plotfig_canvas.mpl_disconnect(self.canvas_conn_id)
+			# Legend
+			if len(self.plot_handle_list) > 0:
+				self.plot_axes.legend(handles=self.plot_handle_list, labels=self.plot_label_list)
 
-		self.plot_axes.set_xlabel(self.tsne_labels[0])
-		self.plot_axes.set_ylabel(self.tsne_labels[1])
-		self.plotfig_canvas.draw()
-		self.plot_nav.update()
-		self.dlg.bind("<Alt-a>", self.set_alpha)
-		self.cluster_btn["state"] = tk.NORMAL
-		self.clust_save_btn["state"] = tk.DISABLED
-		self.loading_dlg.hide()
+			self.plot_axes.set_xlabel(self.tsne_labels[0])
+			self.plot_axes.set_ylabel(self.tsne_labels[1])
+			self.plotfig_canvas.draw()
+			self.plot_nav.update()
+			self.dlg.bind("<Alt-a>", self.set_alpha)
+			self.cluster_btn["state"] = tk.NORMAL
+			self.clust_save_btn["state"] = tk.DISABLED
+			self.loading_dlg.hide()
 
 	def kclusters(self):
 		# Compute and display k-means clusters
 		dlg = OneIntDialog(self.dlg, "k-Means Clusters", "Enter the number of clusters to identify", min_value=2, max_value=min(30, len(self.dataset[0])-1), initial=2)
 		num_clusters = dlg.show()
 		self.loading_dlg.display("Clustering t-SNE output")
 		from sklearn.cluster import KMeans
@@ -8317,15 +8694,15 @@
 				dl.append(self.data_labels[self.groupby_col-1])
 			show_columnar_table(self.dlg, "t-SNE Results", "Coordinates for the two t-SNE dimensions:", dt, dl, "t-SNE coordinates")
 
 	def set_alpha(self, *args):
 		dlg = OneFloatDialog(self.dlg, "Transparency", "Enter the transparency (alpha) value", min_value=0.0, max_value=1.0, initial=self.alpha)
 		new_alpha = dlg.show()
 		if new_alpha is not None:
-			self.alpha = new_alpha
+			self.alpha = min(1.0, max(new_alpha, 0.0))
 			self.q_recalc()
 
 	def show(self):
 		self.dlg.wait_window(self.dlg)
 	def do_close(self, *args):
 		self.parent.remove_tsne(self)
 		try:
@@ -8346,14 +8723,17 @@
 		self.plot_title = None
 		self.dlg = tk.Toplevel()
 		self.dlg.title("UMAP Analysis")
 		self.loading_dlg = LoadingDialog(self.dlg)
 		self.alpha = 0.45
 		self.umap_coords = None
 		self.umap_labels = None
+		# Hover annotation for scatter plots
+		self.annot = None
+		self.canvas_conn_id = None
 		# Data
 		self.dataset = None
 		self.data_labels = None
 		self.numeric_columns = [c[0] for c in self.column_specs if c[1] in ("int", "float")]
 		self.numeric_columns.sort()
 		self.categ_columns = [c[0] for c in self.column_specs if c[1] == "string"]
 		self.categ_columns.sort()
@@ -8377,14 +8757,24 @@
 		self.sel_only_ck.grid(row=0, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
 
 		self.autoupdate_var = tk.StringVar(ctrl_frame, "1")
 		self.autoupdate_ck = ttk.Checkbutton(ctrl_frame, text="Auto-update", command=self.set_autoupdate, variable=self.autoupdate_var,
 				onvalue="1", offvalue="0")
 		self.autoupdate_ck.grid(row=0, column=1, sticky=tk.W, padx=(3,3), pady=(3,3))
 
+		self.compvars_var = tk.StringVar(ctrl_frame, "0")
+		self.compvars_ck = ttk.Checkbutton(ctrl_frame, text="Complete variables only", command=self.q_recalc, variable=self.compvars_var,
+				onvalue="1", offvalue="0")
+		self.compvars_ck.grid(row=1, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
+
+		self.compcases_var = tk.StringVar(ctrl_frame, "0")
+		self.compcases_ck = ttk.Checkbutton(ctrl_frame, text="Complete cases only", command=self.q_recalc, variable=self.compcases_var,
+				onvalue="1", offvalue="0")
+		self.compcases_ck.grid(row=1, column=1, sticky=tk.W, padx=(3,3), pady=(3,3))
+
 		# Frame for input selection and output plot
 		self.content_frame = tk.Frame(self.dlg)
 		self.content_frame.grid(row=2, column=0, sticky=tk.NSEW)
 		self.dlg.rowconfigure(2, weight=1)
 		self.dlg.columnconfigure(0, weight=1)
 		self.content_frame.rowconfigure(0, weight=1)
 		self.content_frame.columnconfigure(0, weight=1)
@@ -8399,15 +8789,15 @@
 		self.inp_frame.columnconfigure(0, weight=1)
 		io_panes.add(self.inp_frame, weight=1)
 
 		self.output_frame = tk.Frame(io_panes, borderwidth=3, relief=tk.RIDGE)
 		self.output_frame.grid(row=0, column=1, sticky=tk.NSEW)
 		self.output_frame.rowconfigure(0, weight=1)
 		self.output_frame.columnconfigure(0, weight=1)
-		io_panes.add(self.output_frame, weight=1)
+		io_panes.add(self.output_frame, weight=4)
 
 		# Variable selection
 		# Add multi-select list of variables to the leftmost pane
 		var_frame = tk.Frame(self.inp_frame)
 		var_frame.grid(row=0, column=0, sticky=tk.NSEW)
 		var_frame.rowconfigure(0, weight=1)
 		var_frame.columnconfigure(0, weight=1)
@@ -8418,19 +8808,20 @@
 
 		# UMAP parameter selection
 		inpopt_frame = tk.Frame(self.inp_frame)
 		inpopt_frame.grid(row=1, column=0, sticky=tk.NSEW)
 		inpopt_frame.columnconfigure(1, weight=1)
 		self.neighbors_var = tk.IntVar(inpopt_frame, min(15, math.floor(self.parent.table_row_count/4)))
 		ttk.Label(inpopt_frame, text="Neighbors:").grid(row=0, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
-		neighbor_sel = ttk.Spinbox(inpopt_frame, textvariable=self.neighbors_var, from_=2, to=math.floor(self.parent.table_row_count/4), width=5)
+		neighbor_sel = ttk.Spinbox(inpopt_frame, textvariable=self.neighbors_var, from_=2, to=math.floor(self.parent.table_row_count/4), width=5,
+				command=self.q_recalc)
 		neighbor_sel.grid(row=0, column=1, sticky=tk.W, padx=(3,3), pady=(3,3))
 		ttk.Label(inpopt_frame, text="Minimum distance:").grid(row=1, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
 		self.mindist_var = tk.DoubleVar(inpopt_frame, 0.1)
-		mindist_sel = ttk.Spinbox(inpopt_frame, textvariable=self.mindist_var, from_=0.0, to=0.99, increment=0.01, width=4)
+		mindist_sel = ttk.Spinbox(inpopt_frame, textvariable=self.mindist_var, from_=0.0, to=0.99, increment=0.01, width=4, command=self.q_recalc)
 		mindist_sel.grid(row=1, column=1, sticky=tk.W, padx=(3,3), pady=(3,3))
 		# n_components is fixed at 2, with no user input allowed.
 		ttk.Label(inpopt_frame, text="Distance metric:").grid(row=2, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
 		self.metric_var = tk.StringVar(inpopt_frame, 'euclidean')
 		metric_sel = ttk.Combobox(inpopt_frame, state="readonly", textvariable=self.metric_var, width=15,
 				values=['braycurtis', 'canberra', 'chebyshev', 'cosine', 'correlation', 'euclidean', 'manhattan', 'minkowski'])
 		metric_sel.grid(row=2, column=1, sticky=tk.W, padx=(3,3), pady=(3,3))
@@ -8543,30 +8934,62 @@
 		# are to be assigned to a column.
 		if self.sel_only_var.get() == "1":
 			dataset = self.parent.get_sel_data(column_list)
 			self.data_rowids = self.parent.get_sel_rowids()
 		else:
 			dataset = self.parent.get_all_data(column_list)
 			self.data_rowids = self.parent.get_all_rowids()
-		if dataset is None or len(dataset[0]) < 6:
+		if dataset is not None:
+			# UMAP can operate on sparse arrays, so removal of missing data is optional
+			if self.compvars_var.get() == "1":
+				# Remove columns with missing data.  This may remove all columns.
+				badcols = []
+				for col in range(self.n_dataset_columns):
+					if not all(dataset[col]):
+						badcols.append(col)
+				if len(badcols) > 0:
+					badcols.reverse()
+					for bc in badcols:
+						del dataset[bc]
+						del column_list[bc]
+						if self.label_col is not None:
+							self.label_col -= 1
+					if self.groupby_col is not None:
+						self.groupby_col = len(column_list)
+					self.n_dataset_columns = self.n_dataset_columns - len(badcols)
+			if self.compcases_var.get() == "1" and self.n_dataset_columns > 0:
+				# Remove rows with missing data.  This may remove all rows.
+				column_indexes = range(self.n_dataset_columns)
+				clean_data = [[] for _ in dataset]
+				clean_rowids = []
+				for i in range(len(dataset[0])):
+					ok = True
+					for col in column_indexes:
+						if dataset[col][i] is None or dataset[col][i] == '':
+							ok = False
+					if ok:
+						for col in range(len(dataset)):
+							clean_data[col].append(dataset[col][i])
+						clean_rowids.append(self.data_rowids[i])
+				self.data_rowids = clean_rowids
+				dataset = clean_data
+			if dataset is not None and len(dataset) > 0 and self.n_dataset_columns > 0:
+				# Convert to floats for numeric data only
+				for i in range(self.n_dataset_columns):
+					if column_list[i] in self.numeric_columns:
+						dataset[i] = [conv_float(v) for v in dataset[i]]
+		if dataset is None or self.n_dataset_columns < 3 or len(dataset[0]) < 6:
 			self.dataset = None
 			self.data_labels = None
 			self.data_btn["state"] = tk.DISABLED
 			self.calc_btn["state"] = tk.DISABLED
 			self.loading_dlg.hide()
-			warning("The dataset must have at least 6 rows for UMAP analysis", {'parent':self.dlg})
+			warning("The dataset must have at least 3 variables and 6 cases for UMAP analysis", {'parent':self.dlg})
 		else:
-			# UMAP can operate on sparse arrays, so there's no need to remove missing data
-			clean_data = dataset
-			# Convert to floats for numeric data only
-			for i in range(len(clean_data)):
-				if column_list[i] in self.numeric_columns:
-					clean_data[i] = [conv_float(v) for v in clean_data[i]]
-			#
-			self.dataset = sort_columns(clean_data)
+			self.dataset = sort_columns(dataset)
 			self.data_labels = column_list
 			self.data_btn["state"] = tk.NORMAL
 			self.calc_btn["state"] = tk.NORMAL
 			self.dtable_btn["state"] = tk.DISABLED
 
 	def clear_output(self):
 		self.dlg.bind("<Alt-a>")
@@ -8580,19 +9003,20 @@
 
 	def recalculate(self):
 		self.loading_dlg.display("Calculating UMAP")
 		import umap
 		from sklearn.preprocessing import StandardScaler
 		self.clear_output()
 		self.get_data()
-		if self.dataset is not None:
+		if self.dataset is not None and len(self.dataset[0]) > 5:
 			# Check to see if this is a sparse matrix
 			is_sparse = False
 			for col in range(self.n_dataset_columns):
-				if any([x is None or x == 0.0 for x in self.dataset[col]]):
+				#if any([x is None or x == 0.0 for x in self.dataset[col]]):
+				if any([x is None for x in self.dataset[col]]):
 					is_sparse = True
 					break
 			ds = copy.copy(self.dataset[0:self.n_dataset_columns])
 			if is_sparse:
 				# Replace all None with 0
 				for col in range(len(ds)):
 					ds[col] = [0.0 if x is None else x for x in ds[col]]
@@ -8773,15 +9197,15 @@
 				dl.append(self.data_labels[self.groupby_col-1])
 			show_columnar_table(self.dlg, "UMAP Results", "Coordinates for the two UMAP dimensions:", dt, dl, "UMAP coordinates")
 
 	def set_alpha(self, *args):
 		dlg = OneFloatDialog(self.dlg, "Transparency", "Enter the transparency (alpha) value", min_value=0.0, max_value=1.0, initial=self.alpha)
 		new_alpha = dlg.show()
 		if new_alpha is not None:
-			self.alpha = new_alpha
+			self.alpha = min(1.0, max(new_alpha, 0.0))
 			self.q_recalc()
 
 	def show(self):
 		self.dlg.wait_window(self.dlg)
 	def do_close(self, *args):
 		self.parent.remove_umap(self)
 		try:
@@ -10755,15 +11179,15 @@
 		ttk.Label(keyframe, width=10, text="Alt-C").grid(row=4, column=0, sticky=tk.N+tk.W)
 		ttk.Label(keyframe, width=50, justify=tk.LEFT, wraplength=350, text="Toggles display of the count of data rows at each location on the map.").grid(row=4, column=1)
 		ttk.Label(keyframe, width=10, text="Alt-F").grid(row=5, column=0, sticky=tk.N+tk.W)
 		ttk.Label(keyframe, width=50, justify=tk.LEFT, wraplength=350, text="Flip (invert) the Y axis on min-max plots, bar plots, bubble plots, scatter plots, and Y-range plots.").grid(row=5, column=1)
 		ttk.Label(keyframe, width=10, text="Alt-G").grid(row=6, column=0, sticky=tk.N+tk.W)
 		ttk.Label(keyframe, width=50, justify=tk.LEFT, wraplength=350, text="From the main application (map) window, open the plot dialog.  On a Normal Q-Q plot, toggle the coloring of points to correspond to groups defined by Jenks Natural Breaks.").grid(row=6, column=1)
 		ttk.Label(keyframe, width=10, text="Alt-L").grid(row=7, column=0, sticky=tk.N+tk.W)
-		ttk.Label(keyframe, width=50, justify=tk.LEFT, wraplength=350, text="Toggle the display of a LOESS smoothing line on line plots and scatter plots.").grid(row=7, column=1)
+		ttk.Label(keyframe, width=50, justify=tk.LEFT, wraplength=350, text="Toggle the display of a LOESS smoothing line on line plots and scatter plots.  Show or hide correlation coefficients in a correlation matrix.").grid(row=7, column=1)
 		ttk.Label(keyframe, width=10, text="Alt-P").grid(row=8, column=0, sticky=tk.N+tk.W)
 		ttk.Label(keyframe, width=50, justify=tk.LEFT, wraplength=350, text="Open the Plot Data dialog from the map view.").grid(row=8, column=1)
 		ttk.Label(keyframe, width=10, text="Alt-Q").grid(row=9, column=0, sticky=tk.N+tk.W)
 		ttk.Label(keyframe, width=50, justify=tk.LEFT, wraplength=350, text="Open the Query Data dialog from the map view.").grid(row=9, column=1)
 		ttk.Label(keyframe, width=10, text="Alt-R").grid(row=10, column=0, sticky=tk.N+tk.W)
 		ttk.Label(keyframe, width=50, justify=tk.LEFT, wraplength=350, text="For line plots and scatter plots: toggle the display of an ordinary least-squares linear regression line. For box plots, bar plots, min-max plots, stripcharts and violin plots: rotate the X and Y axes.").grid(row=10, column=1)
 		ttk.Label(keyframe, width=10, text="Alt-S").grid(row=11, column=0, sticky=tk.N+tk.W)
```

### Comparing `mapdata-3.6.4/mapdata/symbols/24x24/ball24.xbm` & `mapdata-3.7.0/mapdata/symbols/24x24/ball24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.6.4/mapdata/symbols/24x24/block24.xbm` & `mapdata-3.7.0/mapdata/symbols/24x24/block24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.6.4/mapdata/symbols/24x24/circle24.xbm` & `mapdata-3.7.0/mapdata/symbols/24x24/circle24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.6.4/mapdata/symbols/24x24/square24.xbm` & `mapdata-3.7.0/mapdata/symbols/24x24/square24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.6.4/mapdata/symbols/28x28/ball28.xbm` & `mapdata-3.7.0/mapdata/symbols/28x28/ball28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.6.4/mapdata/symbols/28x28/block28.xbm` & `mapdata-3.7.0/mapdata/symbols/28x28/block28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.6.4/mapdata/symbols/28x28/circle28.xbm` & `mapdata-3.7.0/mapdata/symbols/28x28/circle28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.6.4/mapdata/symbols/28x28/square28.xbm` & `mapdata-3.7.0/mapdata/symbols/28x28/square28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.6.4/mapdata.egg-info/PKG-INFO` & `mapdata-3.7.0/mapdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 3.6.4
+Version: 3.7.0
 Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: cortice@tutanota.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,Spreadsheet,Database,PNG,JPG,Postscript
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mapdata-3.6.4/mapdata.egg-info/SOURCES.txt` & `mapdata-3.7.0/mapdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapdata-3.6.4/setup.py` & `mapdata-3.7.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with io.open('README.md', encoding='utf-8') as f:
 	long_description = f.read()
 
 symbol_files = glob.glob("mapdata/symbols/16x16/*.xbm") + glob.glob("mapdata/symbols/20x20/*.xbm") + \
 			glob.glob("mapdata/symbols/24x24/*.xbm") + glob.glob("mapdata/symbols/28x28/*.xbm")
 
 setuptools.setup(name='mapdata',
-	version='3.6.4',
+	version='3.7.0',
 	description="An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database",
 	author='Dreas Nielsen',
 	author_email='cortice@tutanota.com',
     url='https://osdn.net/project/mapdata/',
     packages=['mapdata'],
 	scripts=['mapdata/mapdata.py'],
 	data_files=[('symbols', symbol_files), ('config', ['mapdata/configfile/mapdata.conf'])],
```

