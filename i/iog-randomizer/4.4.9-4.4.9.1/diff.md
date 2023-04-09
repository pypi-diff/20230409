# Comparing `tmp/iog-randomizer-4.4.9.tar.gz` & `tmp/iog-randomizer-4.4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iog-randomizer-4.4.9.tar", last modified: Tue Nov  1 19:08:22 2022, max compression
+gzip compressed data, was "iog-randomizer-4.4.9.1.tar", last modified: Sun Apr  9 04:47:14 2023, max compression
```

## Comparing `iog-randomizer-4.4.9.tar` & `iog-randomizer-4.4.9.1.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxrwxrwx   0        0        0        0 2022-11-01 19:08:22.288465 iog-randomizer-4.4.9/
--rw-rw-rw-   0        0        0     1233 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/LICENSE
--rw-rw-rw-   0        0        0      186 2022-11-01 19:08:22.288465 iog-randomizer-4.4.9/PKG-INFO
--rw-rw-rw-   0        0        0    16459 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/README.md
-drwxrwxrwx   0        0        0        0 2022-11-01 19:08:22.104973 iog-randomizer-4.4.9/iog_randomizer.egg-info/
--rw-rw-rw-   0        0        0      186 2022-11-01 19:08:22.000000 iog-randomizer-4.4.9/iog_randomizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6261 2022-11-01 19:08:22.000000 iog-randomizer-4.4.9/iog_randomizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-01 19:08:22.000000 iog-randomizer-4.4.9/iog_randomizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2022-11-01 19:08:22.000000 iog-randomizer-4.4.9/iog_randomizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-11-01 19:08:22.000000 iog-randomizer-4.4.9/iog_randomizer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-11-01 19:08:22.117620 iog-randomizer-4.4.9/randomizer/
--rw-rw-rw-   0        0        0       25 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-01 19:08:22.228558 iog-randomizer-4.4.9/randomizer/bin/
--rw-rw-rw-   0        0        0       84 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/00f49a_roominit.bin
--rw-rw-rw-   0        0        0     2048 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/00f500_redjewel.bin
--rw-rw-rw-   0        0        0      448 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9/randomizer/bin/00fdf0_pi.bin
--rw-rw-rw-   0        0        0       40 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/01a7c2_babel.bin
--rw-rw-rw-   0        0        0      256 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/01aade_roomrewards.bin
--rw-rw-rw-   0        0        0      440 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/01abf0_enemies_z3.bin
--rw-rw-rw-   0        0        0      440 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/01abf0_enemiesadvanced.bin
--rw-rw-rw-   0        0        0      440 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9/randomizer/bin/01abf0_enemiesbeginner.bin
--rw-rw-rw-   0        0        0      440 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9/randomizer/bin/01abf0_enemiesexpert.bin
--rw-rw-rw-   0        0        0      440 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9/randomizer/bin/01abf0_enemiesintermediate.bin
--rw-rw-rw-   0        0        0      440 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/01abf0_enemiesohko.bin
--rw-rw-rw-   0        0        0      224 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/01afa6_chests.bin
--rw-rw-rw-   0        0        0     2863 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/01dabf_startmenu.bin
--rw-rw-rw-   0        0        0     1210 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/01e132_itemdesc.bin
--rw-rw-rw-   0        0        0      478 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/01fd24_acquisition.bin
--rw-rw-rw-   0        0        0       98 2021-03-25 16:40:25.000000 iog-randomizer-4.4.9/randomizer/bin/02f0c0_firebird.bin
--rw-rw-rw-   0        0        0     1784 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/02f130_enemystats.bin
--rw-rw-rw-   0        0        0     1784 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/02f130_enemystats_z3.bin
--rw-rw-rw-   0        0        0      109 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/03881d_item05.bin
--rw-rw-rw-   0        0        0      157 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/038bf5_item09.bin
--rw-rw-rw-   0        0        0      220 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/038f17_item0d.bin
--rw-rw-rw-   0        0        0       53 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/03950c_item16.bin
--rw-rw-rw-   0        0        0       36 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/03983d_item19.bin
--rw-rw-rw-   0        0        0      268 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/039d09_item25.bin
--rw-rw-rw-   0        0        0       81 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/039f5d_item28.bin
--rw-rw-rw-   0        0        0      686 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/03b401_mapchoices.bin
--rw-rw-rw-   0        0        0      368 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/03b955_mapdest.bin
--rw-rw-rw-   0        0        0      135 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/03f779_statupgrades.bin
--rw-rw-rw-   0        0        0       79 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/03fd70_rjm.bin
--rw-rw-rw-   0        0        0      134 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9/randomizer/bin/03fdc0_startmenu.bin
--rw-rw-rw-   0        0        0       74 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/03ff90_copd4.bin
--rw-rw-rw-   0        0        0       70 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/048a94_teacher.bin
--rw-rw-rw-   0        0        0      399 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/04b9a5_seaside.bin
--rw-rw-rw-   0        0        0       78 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/04c4fb_edward.bin
--rw-rw-rw-   0        0        0       57 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/04c6af_edward2.bin
--rw-rw-rw-   0        0        0       95 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/04d1a0_castleguard.bin
--rw-rw-rw-   0        0        0      256 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/04e2a3_itory.bin
--rw-rw-rw-   0        0        0      238 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/04e5ff_lilly.bin
--rw-rw-rw-   0        0        0      220 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/04fb50_tutorial.bin
--rw-rw-rw-   0        0        0     2048 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/058100_redjewel.bin
--rw-rw-rw-   0        0        0      175 2020-02-26 04:14:01.000000 iog-randomizer-4.4.9/randomizer/bin/0584a9_goldship.bin
--rw-rw-rw-   0        0        0      122 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/05cf85_freejia.bin
--rw-rw-rw-   0        0        0      184 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/05d7e2_trappedlaborer.bin
--rw-rw-rw-   0        0        0      479 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/05d89a_neilscottage.bin
--rw-rw-rw-   0        0        0      248 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/05e647_nazca.bin
--rw-rw-rw-   0        0        0      338 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/05f356_skygarden.bin
--rw-rw-rw-   0        0        0       42 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/069739_mudoor.bin
--rw-rw-rw-   0        0        0      462 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/0699dc_mu.bin
--rw-rw-rw-   0        0        0       46 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/06ba36_angelsign.bin
--rw-rw-rw-   0        0        0     1867 2021-09-13 18:24:28.000000 iog-randomizer-4.4.9/randomizer/bin/06dd30_collectioncheck.bin
--rw-rw-rw-   0        0        0       88 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/06e500_vampchange.bin
--rw-rw-rw-   0        0        0       37 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/078569_watermia1.bin
--rw-rw-rw-   0        0        0      173 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/0786c1_watermia2.bin
--rw-rw-rw-   0        0        0      145 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/079237_russianglass.bin
--rw-rw-rw-   0        0        0      192 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/07b59e_necklace.bin
--rw-rw-rw-   0        0        0       80 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/07c432_euro1.bin
--rw-rw-rw-   0        0        0      572 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/07c4d0_euro2.bin
--rw-rw-rw-   0        0        0       86 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/07e517_euroitem.bin
--rw-rw-rw-   0        0        0      352 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/088fc4_natives.bin
--rw-rw-rw-   0        0        0      113 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/089a31_ankorwat.bin
--rw-rw-rw-   0        0        0      115 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/089abf_ankorwat.bin
--rw-rw-rw-   0        0        0      163 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/08b010_snakegame.bin
--rw-rw-rw-   0        0        0     1136 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/08cec9_jeweler.bin
--rw-rw-rw-   0        0        0      811 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/08db07_darkspace.bin
--rw-rw-rw-   0        0        0       80 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/08fd30_forcechange.bin
--rw-rw-rw-   0        0        0       87 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9/randomizer/bin/08fd80_jeweler2.bin
--rw-rw-rw-   0        0        0       87 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/08fd80_jeweler2_rjm.bin
--rw-rw-rw-   0        0        0      375 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/09ca02_incaship.bin
--rw-rw-rw-   0        0        0      253 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/09d0f5_moontribe.bin
--rw-rw-rw-   0        0        0      302 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/09d11e_moontribe.bin
--rw-rw-rw-   0        0        0      130 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/09d30f_moontribe.bin
--rw-rw-rw-   0        0        0       88 2020-02-26 04:14:02.000000 iog-randomizer-4.4.9/randomizer/bin/0aff99_viperchange.bin
--rw-rw-rw-   0        0        0      318 2022-11-01 18:06:43.000000 iog-randomizer-4.4.9/randomizer/bin/0bfd00_switches.bin
--rw-rw-rw-   0        0        0      434 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9/randomizer/bin/0bfe40_infdeath.bin
--rw-rw-rw-   0        0        0      211 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/0ce099_babel.bin
--rw-rw-rw-   0        0        0    12286 2020-02-26 04:14:02.000000 iog-randomizer-4.4.9/randomizer/bin/0d8000_mapdata.bin
--rw-rw-rw-   0        0        0      112 2021-09-13 18:24:28.000000 iog-randomizer-4.4.9/randomizer/bin/0f8fa4_fluteless.bin
--rw-rw-rw-   0        0        0       68 2021-04-20 04:45:25.000000 iog-randomizer-4.4.9/randomizer/bin/108ea3_multijewel.bin
--rw-rw-rw-   0        0        0     1531 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/193d25_ishtarpuzzle.bin
--rw-rw-rw-   0        0        0     1257 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/1a5a37_angelmap.bin
--rw-rw-rw-   0        0        0      481 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/1d42a2_incatile.bin
--rw-rw-rw-   0        0        0      486 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/1e28a5_mupassage.bin
--rw-rw-rw-   0        0        0        0 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/__init__.py
--rw-rw-rw-   0        0        0     1024 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/incamapblank.bin
--rw-rw-rw-   0        0        0     4096 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/ishtarmapblank.bin
--rw-rw-rw-   0        0        0       57 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/bin/item_get_blank.bin
-drwxrwxrwx   0        0        0        0 2022-11-01 19:08:22.061168 iog-randomizer-4.4.9/randomizer/bin/plugins/
-drwxrwxrwx   0        0        0        0 2022-11-01 19:08:22.272446 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/
--rw-rw-rw-   0        0        0        4 2020-02-26 04:14:02.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/00800f_BrkVector.bin
--rw-rw-rw-   0        0        0      472 2020-02-26 04:14:02.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/008476_FasterInterrupts.bin
--rw-rw-rw-   0        0        0       34 2022-11-01 17:12:52.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/008ffd_FasterCop23.bin
--rw-rw-rw-   0        0        0       15 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/00b125_PageAlignedActorFinder.bin
--rw-rw-rw-   0        0        0      174 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/00bce1_FasterCometShimmerThinkers.bin
--rw-rw-rw-   0        0        0       46 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/00f3d7_FasterOrbiters.bin
--rw-rw-rw-   0        0        0      229 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/00fd00_LibsAndMisc.bin
--rw-rw-rw-   0        0        0       12 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/0281da_FasterMultiplication.bin
--rw-rw-rw-   0        0        0       12 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/0281ee_FasterDivision.bin
--rw-rw-rw-   0        0        0        2 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/02a5e8_HereBeDragons_RemoveNops.bin
--rw-rw-rw-   0        0        0        1 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/03c84b_FasterRenderingFragment.bin
--rw-rw-rw-   0        0        0      193 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/03c854_FasterRendering.bin
--rw-rw-rw-   0        0        0      125 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/03ca5f_FasterAnimating.bin
--rw-rw-rw-   0        0        0       27 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/03cde4_HereBeDragons_PageAlignActorIds.bin
--rw-rw-rw-   0        0        0       15 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/03f745_PageAlignActorIdsHelper.bin
--rw-rw-rw-   0        0        0     1362 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/07e9fc_ApocalypseGaiaAssets2.bin
--rw-rw-rw-   0        0        0        2 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/08c313_PageAlignPyramidSmasher8.bin
--rw-rw-rw-   0        0        0        2 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/08c3b2_PageAlignPyramidSmasher7.bin
--rw-rw-rw-   0        0        0        2 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/08c49c_PageAlignPyramidSmasher3.bin
--rw-rw-rw-   0        0        0        2 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/08c556_PageAlignPyramidSmasher5.bin
--rw-rw-rw-   0        0        0        2 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/08c567_PageAlignPyramidSmasher6.bin
--rw-rw-rw-   0        0        0        2 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/08c5da_PageAlignPyramidSmasher1.bin
--rw-rw-rw-   0        0        0        2 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/08c5ef_PageAlignPyramidSmasher2.bin
--rw-rw-rw-   0        0        0        2 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/08c61c_PageAlignPyramidSmasher4.bin
--rw-rw-rw-   0        0        0     4114 2021-04-20 04:45:25.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/09aa6e_ApocalypseGaiaCode.bin
--rw-rw-rw-   0        0        0     1783 2021-04-20 04:45:25.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/09f790_ApocalypseGaiaAssets1.bin
--rw-rw-rw-   0        0        0        7 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/0aa36e_FasterMakePlayerImmune.bin
--rw-rw-rw-   0        0        0        4 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/0acbf2_FixVanillaGardenWormBug.bin
--rw-rw-rw-   0        0        0      530 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/0afd87_PushAndUpdateAGAssets.bin
--rw-rw-rw-   0        0        0        9 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/0ceac7_CometThinkerTableFragment.bin
--rw-rw-rw-   0        0        0      470 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/0ceb74_CometThinkers.bin
--rw-rw-rw-   0        0        0     1837 2021-04-20 04:45:25.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/0ceeaa_CometAndDarkGaiaCode.bin
--rw-rw-rw-   0        0        0        1 2020-02-26 04:14:05.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/AG/1f2ce7_SetCometBg2HeightTo2.bin
-drwxrwxrwx   0        0        0        0 2022-11-01 19:08:22.061168 iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/
-drwxrwxrwx   0        0        0        0 2022-11-01 19:08:22.275432 iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/bagu/
--rw-rw-rw-   0        0        0    16384 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/bagu/1a8000.bin
--rw-rw-rw-   0        0        0     5120 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/bagu/1b8000.bin
-drwxrwxrwx   0        0        0        0 2022-11-01 19:08:22.276429 iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/freet/
--rw-rw-rw-   0        0        0     2356 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/freet/1a820a.bin
-drwxrwxrwx   0        0        0        0 2022-11-01 19:08:22.281428 iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/invisible/
--rw-rw-rw-   0        0        0    32768 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/invisible/1a8000.bin
--rw-rw-rw-   0        0        0    32768 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/invisible/1b8000.bin
--rw-rw-rw-   0        0        0    16384 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/invisible/1c8000.bin
-drwxrwxrwx   0        0        0        0 2022-11-01 19:08:22.282413 iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/solar/
--rw-rw-rw-   0        0        0    69280 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/solar/1a8000.bin
-drwxrwxrwx   0        0        0        0 2022-11-01 19:08:22.283416 iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/sye/
--rw-rw-rw-   0        0        0    69280 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/sye/1a8000.bin
--rw-rw-rw-   0        0        0   331576 2022-11-01 17:12:52.000000 iog-randomizer-4.4.9/randomizer/classes.py
--rw-rw-rw-   0        0        0    68771 2021-04-20 04:45:25.000000 iog-randomizer-4.4.9/randomizer/constants.py
--rw-rw-rw-   0        0        0      191 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/errors.py
--rw-rw-rw-   0        0        0   200620 2022-11-01 19:08:13.000000 iog-randomizer-4.4.9/randomizer/iogr_rom.py
-drwxrwxrwx   0        0        0        0 2022-11-01 19:08:22.286402 iog-randomizer-4.4.9/randomizer/models/
--rw-rw-rw-   0        0        0        0 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/models/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-01 19:08:22.288465 iog-randomizer-4.4.9/randomizer/models/enums/
--rw-rw-rw-   0        0        0        0 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/models/enums/__init__.py
--rw-rw-rw-   0        0        0      113 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/models/enums/difficulty.py
--rw-rw-rw-   0        0        0      129 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/models/enums/enemizer.py
--rw-rw-rw-   0        0        0      107 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/models/enums/entrance_shuffle.py
--rw-rw-rw-   0        0        0      128 2020-02-26 04:14:06.000000 iog-randomizer-4.4.9/randomizer/models/enums/goal.py
--rw-rw-rw-   0        0        0      121 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9/randomizer/models/enums/level.py
--rw-rw-rw-   0        0        0      101 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/models/enums/logic.py
--rw-rw-rw-   0        0        0      174 2021-09-13 18:24:28.000000 iog-randomizer-4.4.9/randomizer/models/enums/sprites.py
--rw-rw-rw-   0        0        0      128 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/models/enums/start_location.py
--rw-rw-rw-   0        0        0      118 2021-09-13 18:24:28.000000 iog-randomizer-4.4.9/randomizer/models/enums/statue_req.py
--rw-rw-rw-   0        0        0     2097 2021-10-04 13:49:25.000000 iog-randomizer-4.4.9/randomizer/models/randomizer_data.py
--rw-rw-rw-   0        0        0      818 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/patch.py
--rw-rw-rw-   0        0        0     4190 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/quintet_comp.py
--rw-rw-rw-   0        0        0    18409 2019-11-10 22:39:22.000000 iog-randomizer-4.4.9/randomizer/quintet_text.py
-drwxrwxrwx   0        0        0        0 2022-11-01 19:08:22.288465 iog-randomizer-4.4.9/randomizer/tests/
--rw-rw-rw-   0        0        0        0 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/tests/__init__.py
--rw-rw-rw-   0        0        0      407 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9/randomizer/tests/test_generate_filename.py
--rw-rw-rw-   0        0        0       42 2022-11-01 19:08:22.288465 iog-randomizer-4.4.9/setup.cfg
--rw-rw-rw-   0        0        0      518 2022-11-01 19:08:12.000000 iog-randomizer-4.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.359680 iog-randomizer-4.4.9.1/
+-rw-rw-rw-   0        0        0     1233 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/LICENSE
+-rw-rw-rw-   0        0        0      188 2023-04-09 04:47:14.359680 iog-randomizer-4.4.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0    16459 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 04:47:13.547349 iog-randomizer-4.4.9.1/iog_randomizer.egg-info/
+-rw-rw-rw-   0        0        0      188 2023-04-09 04:47:13.000000 iog-randomizer-4.4.9.1/iog_randomizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6261 2023-04-09 04:47:13.000000 iog-randomizer-4.4.9.1/iog_randomizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 04:47:13.000000 iog-randomizer-4.4.9.1/iog_randomizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-09 04:47:13.000000 iog-randomizer-4.4.9.1/iog_randomizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-09 04:47:13.000000 iog-randomizer-4.4.9.1/iog_randomizer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 04:47:13.609862 iog-randomizer-4.4.9.1/randomizer/
+-rw-rw-rw-   0        0        0       25 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.109746 iog-randomizer-4.4.9.1/randomizer/bin/
+-rw-rw-rw-   0        0        0       84 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/00f49a_roominit.bin
+-rw-rw-rw-   0        0        0     2048 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/00f500_redjewel.bin
+-rw-rw-rw-   0        0        0      448 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9.1/randomizer/bin/00fdf0_pi.bin
+-rw-rw-rw-   0        0        0       40 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/01a7c2_babel.bin
+-rw-rw-rw-   0        0        0      256 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/01aade_roomrewards.bin
+-rw-rw-rw-   0        0        0      440 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/01abf0_enemies_z3.bin
+-rw-rw-rw-   0        0        0      440 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/01abf0_enemiesadvanced.bin
+-rw-rw-rw-   0        0        0      440 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9.1/randomizer/bin/01abf0_enemiesbeginner.bin
+-rw-rw-rw-   0        0        0      440 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9.1/randomizer/bin/01abf0_enemiesexpert.bin
+-rw-rw-rw-   0        0        0      440 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9.1/randomizer/bin/01abf0_enemiesintermediate.bin
+-rw-rw-rw-   0        0        0      440 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/01abf0_enemiesohko.bin
+-rw-rw-rw-   0        0        0      224 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/01afa6_chests.bin
+-rw-rw-rw-   0        0        0     2863 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/01dabf_startmenu.bin
+-rw-rw-rw-   0        0        0     1210 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/01e132_itemdesc.bin
+-rw-rw-rw-   0        0        0      478 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/01fd24_acquisition.bin
+-rw-rw-rw-   0        0        0       98 2021-03-25 16:40:25.000000 iog-randomizer-4.4.9.1/randomizer/bin/02f0c0_firebird.bin
+-rw-rw-rw-   0        0        0     1784 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/02f130_enemystats.bin
+-rw-rw-rw-   0        0        0     1784 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/02f130_enemystats_z3.bin
+-rw-rw-rw-   0        0        0      109 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/03881d_item05.bin
+-rw-rw-rw-   0        0        0      157 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/038bf5_item09.bin
+-rw-rw-rw-   0        0        0      220 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/038f17_item0d.bin
+-rw-rw-rw-   0        0        0       53 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/03950c_item16.bin
+-rw-rw-rw-   0        0        0       36 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/03983d_item19.bin
+-rw-rw-rw-   0        0        0      268 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/039d09_item25.bin
+-rw-rw-rw-   0        0        0       81 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/039f5d_item28.bin
+-rw-rw-rw-   0        0        0      686 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/03b401_mapchoices.bin
+-rw-rw-rw-   0        0        0      368 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/03b955_mapdest.bin
+-rw-rw-rw-   0        0        0      135 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/03f779_statupgrades.bin
+-rw-rw-rw-   0        0        0       79 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/03fd70_rjm.bin
+-rw-rw-rw-   0        0        0      134 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9.1/randomizer/bin/03fdc0_startmenu.bin
+-rw-rw-rw-   0        0        0       74 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/03ff90_copd4.bin
+-rw-rw-rw-   0        0        0       70 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/048a94_teacher.bin
+-rw-rw-rw-   0        0        0      399 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/04b9a5_seaside.bin
+-rw-rw-rw-   0        0        0       78 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/04c4fb_edward.bin
+-rw-rw-rw-   0        0        0       57 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/04c6af_edward2.bin
+-rw-rw-rw-   0        0        0       95 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/04d1a0_castleguard.bin
+-rw-rw-rw-   0        0        0      256 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/04e2a3_itory.bin
+-rw-rw-rw-   0        0        0      238 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/04e5ff_lilly.bin
+-rw-rw-rw-   0        0        0      220 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/04fb50_tutorial.bin
+-rw-rw-rw-   0        0        0     2048 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/058100_redjewel.bin
+-rw-rw-rw-   0        0        0      175 2020-02-26 04:14:01.000000 iog-randomizer-4.4.9.1/randomizer/bin/0584a9_goldship.bin
+-rw-rw-rw-   0        0        0      122 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/05cf85_freejia.bin
+-rw-rw-rw-   0        0        0      184 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/05d7e2_trappedlaborer.bin
+-rw-rw-rw-   0        0        0      479 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/05d89a_neilscottage.bin
+-rw-rw-rw-   0        0        0      248 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/05e647_nazca.bin
+-rw-rw-rw-   0        0        0      338 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/05f356_skygarden.bin
+-rw-rw-rw-   0        0        0       42 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/069739_mudoor.bin
+-rw-rw-rw-   0        0        0      462 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/0699dc_mu.bin
+-rw-rw-rw-   0        0        0       46 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/06ba36_angelsign.bin
+-rw-rw-rw-   0        0        0     1867 2022-11-06 21:34:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/06dd30_collectioncheck.bin
+-rw-rw-rw-   0        0        0       88 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/06e500_vampchange.bin
+-rw-rw-rw-   0        0        0       37 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/078569_watermia1.bin
+-rw-rw-rw-   0        0        0      173 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/0786c1_watermia2.bin
+-rw-rw-rw-   0        0        0      145 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/079237_russianglass.bin
+-rw-rw-rw-   0        0        0      192 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/07b59e_necklace.bin
+-rw-rw-rw-   0        0        0       80 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/07c432_euro1.bin
+-rw-rw-rw-   0        0        0      572 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/07c4d0_euro2.bin
+-rw-rw-rw-   0        0        0       86 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/07e517_euroitem.bin
+-rw-rw-rw-   0        0        0      352 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/088fc4_natives.bin
+-rw-rw-rw-   0        0        0      113 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/089a31_ankorwat.bin
+-rw-rw-rw-   0        0        0      115 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/089abf_ankorwat.bin
+-rw-rw-rw-   0        0        0      163 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/08b010_snakegame.bin
+-rw-rw-rw-   0        0        0     1136 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/08cec9_jeweler.bin
+-rw-rw-rw-   0        0        0      811 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/08db07_darkspace.bin
+-rw-rw-rw-   0        0        0       80 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/08fd30_forcechange.bin
+-rw-rw-rw-   0        0        0       87 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/08fd80_jeweler2.bin
+-rw-rw-rw-   0        0        0       87 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/08fd80_jeweler2_rjm.bin
+-rw-rw-rw-   0        0        0      375 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/09ca02_incaship.bin
+-rw-rw-rw-   0        0        0      253 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/09d0f5_moontribe.bin
+-rw-rw-rw-   0        0        0      302 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/09d11e_moontribe.bin
+-rw-rw-rw-   0        0        0      130 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/09d30f_moontribe.bin
+-rw-rw-rw-   0        0        0       88 2020-02-26 04:14:02.000000 iog-randomizer-4.4.9.1/randomizer/bin/0aff99_viperchange.bin
+-rw-rw-rw-   0        0        0      317 2023-04-09 03:38:21.000000 iog-randomizer-4.4.9.1/randomizer/bin/0bfd00_switches.bin
+-rw-rw-rw-   0        0        0      434 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9.1/randomizer/bin/0bfe40_infdeath.bin
+-rw-rw-rw-   0        0        0      211 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/0ce099_babel.bin
+-rw-rw-rw-   0        0        0    12286 2020-02-26 04:14:02.000000 iog-randomizer-4.4.9.1/randomizer/bin/0d8000_mapdata.bin
+-rw-rw-rw-   0        0        0      112 2021-09-13 18:24:28.000000 iog-randomizer-4.4.9.1/randomizer/bin/0f8fa4_fluteless.bin
+-rw-rw-rw-   0        0        0       68 2021-04-20 04:45:25.000000 iog-randomizer-4.4.9.1/randomizer/bin/108ea3_multijewel.bin
+-rw-rw-rw-   0        0        0     1531 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/193d25_ishtarpuzzle.bin
+-rw-rw-rw-   0        0        0     1257 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/1a5a37_angelmap.bin
+-rw-rw-rw-   0        0        0      481 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/1d42a2_incatile.bin
+-rw-rw-rw-   0        0        0      486 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/1e28a5_mupassage.bin
+-rw-rw-rw-   0        0        0        0 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/__init__.py
+-rw-rw-rw-   0        0        0     1024 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/incamapblank.bin
+-rw-rw-rw-   0        0        0     4096 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/ishtarmapblank.bin
+-rw-rw-rw-   0        0        0       57 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/item_get_blank.bin
+drwxrwxrwx   0        0        0        0 2023-04-09 04:47:13.500513 iog-randomizer-4.4.9.1/randomizer/bin/plugins/
+drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.234717 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/
+-rw-rw-rw-   0        0        0        4 2020-02-26 04:14:02.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/00800f_BrkVector.bin
+-rw-rw-rw-   0        0        0      472 2020-02-26 04:14:02.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/008476_FasterInterrupts.bin
+-rw-rw-rw-   0        0        0       34 2023-02-07 15:44:11.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/008ffd_FasterCop23.bin
+-rw-rw-rw-   0        0        0       15 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/00b125_PageAlignedActorFinder.bin
+-rw-rw-rw-   0        0        0      174 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/00bce1_FasterCometShimmerThinkers.bin
+-rw-rw-rw-   0        0        0       46 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/00f3d7_FasterOrbiters.bin
+-rw-rw-rw-   0        0        0      229 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/00fd00_LibsAndMisc.bin
+-rw-rw-rw-   0        0        0       12 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/0281da_FasterMultiplication.bin
+-rw-rw-rw-   0        0        0       12 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/0281ee_FasterDivision.bin
+-rw-rw-rw-   0        0        0        2 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/02a5e8_HereBeDragons_RemoveNops.bin
+-rw-rw-rw-   0        0        0        1 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/03c84b_FasterRenderingFragment.bin
+-rw-rw-rw-   0        0        0      193 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/03c854_FasterRendering.bin
+-rw-rw-rw-   0        0        0      125 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/03ca5f_FasterAnimating.bin
+-rw-rw-rw-   0        0        0       27 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/03cde4_HereBeDragons_PageAlignActorIds.bin
+-rw-rw-rw-   0        0        0       15 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/03f745_PageAlignActorIdsHelper.bin
+-rw-rw-rw-   0        0        0     1362 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/07e9fc_ApocalypseGaiaAssets2.bin
+-rw-rw-rw-   0        0        0        2 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/08c313_PageAlignPyramidSmasher8.bin
+-rw-rw-rw-   0        0        0        2 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/08c3b2_PageAlignPyramidSmasher7.bin
+-rw-rw-rw-   0        0        0        2 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/08c49c_PageAlignPyramidSmasher3.bin
+-rw-rw-rw-   0        0        0        2 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/08c556_PageAlignPyramidSmasher5.bin
+-rw-rw-rw-   0        0        0        2 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/08c567_PageAlignPyramidSmasher6.bin
+-rw-rw-rw-   0        0        0        2 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/08c5da_PageAlignPyramidSmasher1.bin
+-rw-rw-rw-   0        0        0        2 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/08c5ef_PageAlignPyramidSmasher2.bin
+-rw-rw-rw-   0        0        0        2 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/08c61c_PageAlignPyramidSmasher4.bin
+-rw-rw-rw-   0        0        0     4114 2021-04-20 04:45:25.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/09aa6e_ApocalypseGaiaCode.bin
+-rw-rw-rw-   0        0        0     1783 2021-04-20 04:45:25.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/09f790_ApocalypseGaiaAssets1.bin
+-rw-rw-rw-   0        0        0        7 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/0aa36e_FasterMakePlayerImmune.bin
+-rw-rw-rw-   0        0        0        4 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/0acbf2_FixVanillaGardenWormBug.bin
+-rw-rw-rw-   0        0        0      530 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/0afd87_PushAndUpdateAGAssets.bin
+-rw-rw-rw-   0        0        0        9 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/0ceac7_CometThinkerTableFragment.bin
+-rw-rw-rw-   0        0        0      470 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/0ceb74_CometThinkers.bin
+-rw-rw-rw-   0        0        0     1837 2021-04-20 04:45:25.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/0ceeaa_CometAndDarkGaiaCode.bin
+-rw-rw-rw-   0        0        0        1 2020-02-26 04:14:05.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/1f2ce7_SetCometBg2HeightTo2.bin
+drwxrwxrwx   0        0        0        0 2023-04-09 04:47:13.516109 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/
+drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.250339 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/bagu/
+-rw-rw-rw-   0        0        0    16384 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/bagu/1a8000.bin
+-rw-rw-rw-   0        0        0     5120 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/bagu/1b8000.bin
+drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.265959 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/freet/
+-rw-rw-rw-   0        0        0     2356 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/freet/1a820a.bin
+drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.281581 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/invisible/
+-rw-rw-rw-   0        0        0    32768 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/invisible/1a8000.bin
+-rw-rw-rw-   0        0        0    32768 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/invisible/1b8000.bin
+-rw-rw-rw-   0        0        0    16384 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/invisible/1c8000.bin
+drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.281581 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/solar/
+-rw-rw-rw-   0        0        0    69280 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/solar/1a8000.bin
+drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.297202 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/sye/
+-rw-rw-rw-   0        0        0    69280 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/sye/1a8000.bin
+-rw-rw-rw-   0        0        0   331576 2023-04-09 03:38:21.000000 iog-randomizer-4.4.9.1/randomizer/classes.py
+-rw-rw-rw-   0        0        0    68771 2021-04-20 04:45:25.000000 iog-randomizer-4.4.9.1/randomizer/constants.py
+-rw-rw-rw-   0        0        0      191 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/errors.py
+-rw-rw-rw-   0        0        0   200866 2023-04-09 04:45:25.000000 iog-randomizer-4.4.9.1/randomizer/iogr_rom.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.297202 iog-randomizer-4.4.9.1/randomizer/models/
+-rw-rw-rw-   0        0        0        0 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.359680 iog-randomizer-4.4.9.1/randomizer/models/enums/
+-rw-rw-rw-   0        0        0        0 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/__init__.py
+-rw-rw-rw-   0        0        0      113 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/difficulty.py
+-rw-rw-rw-   0        0        0      129 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/enemizer.py
+-rw-rw-rw-   0        0        0      107 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/entrance_shuffle.py
+-rw-rw-rw-   0        0        0      128 2020-02-26 04:14:06.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/goal.py
+-rw-rw-rw-   0        0        0      121 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/level.py
+-rw-rw-rw-   0        0        0      101 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/logic.py
+-rw-rw-rw-   0        0        0      174 2021-09-13 18:24:28.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/sprites.py
+-rw-rw-rw-   0        0        0      128 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/start_location.py
+-rw-rw-rw-   0        0        0      118 2021-09-13 18:24:28.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/statue_req.py
+-rw-rw-rw-   0        0        0     2097 2023-04-09 03:38:21.000000 iog-randomizer-4.4.9.1/randomizer/models/randomizer_data.py
+-rw-rw-rw-   0        0        0      818 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/patch.py
+-rw-rw-rw-   0        0        0     4190 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/quintet_comp.py
+-rw-rw-rw-   0        0        0    18409 2019-11-10 22:39:22.000000 iog-randomizer-4.4.9.1/randomizer/quintet_text.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.359680 iog-randomizer-4.4.9.1/randomizer/tests/
+-rw-rw-rw-   0        0        0        0 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/tests/__init__.py
+-rw-rw-rw-   0        0        0      407 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/tests/test_generate_filename.py
+-rw-rw-rw-   0        0        0       42 2023-04-09 04:47:14.359680 iog-randomizer-4.4.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      520 2023-04-09 04:45:36.000000 iog-randomizer-4.4.9.1/setup.py
```

### Comparing `iog-randomizer-4.4.9/LICENSE` & `iog-randomizer-4.4.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/README.md` & `iog-randomizer-4.4.9.1/README.md`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/iog_randomizer.egg-info/SOURCES.txt` & `iog-randomizer-4.4.9.1/iog_randomizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/00f500_redjewel.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/00f500_redjewel.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/01dabf_startmenu.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/01dabf_startmenu.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/01e132_itemdesc.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/01e132_itemdesc.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/02f130_enemystats.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/02f130_enemystats.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/02f130_enemystats_z3.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/02f130_enemystats_z3.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/03b401_mapchoices.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/03b401_mapchoices.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/058100_redjewel.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/058100_redjewel.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/06dd30_collectioncheck.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/06dd30_collectioncheck.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/07c4d0_euro2.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/07c4d0_euro2.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/08cec9_jeweler.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/08cec9_jeweler.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/08db07_darkspace.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/08db07_darkspace.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/0d8000_mapdata.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/0d8000_mapdata.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/193d25_ishtarpuzzle.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/193d25_ishtarpuzzle.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/1a5a37_angelmap.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/1a5a37_angelmap.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/ishtarmapblank.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/ishtarmapblank.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/plugins/AG/07e9fc_ApocalypseGaiaAssets2.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/07e9fc_ApocalypseGaiaAssets2.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/plugins/AG/09aa6e_ApocalypseGaiaCode.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/09aa6e_ApocalypseGaiaCode.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/plugins/AG/09f790_ApocalypseGaiaAssets1.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/09f790_ApocalypseGaiaAssets1.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/plugins/AG/0afd87_PushAndUpdateAGAssets.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/0afd87_PushAndUpdateAGAssets.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/plugins/AG/0ceeaa_CometAndDarkGaiaCode.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/0ceeaa_CometAndDarkGaiaCode.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/bagu/1a8000.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/bagu/1a8000.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/bagu/1b8000.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/bagu/1b8000.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/freet/1a820a.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/freet/1a820a.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/invisible/1a8000.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/invisible/1a8000.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/invisible/1b8000.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/invisible/1b8000.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/invisible/1c8000.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/invisible/1c8000.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/solar/1a8000.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/solar/1a8000.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/bin/plugins/sprites/sye/1a8000.bin` & `iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/sye/1a8000.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/classes.py` & `iog-randomizer-4.4.9.1/randomizer/classes.py`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/constants.py` & `iog-randomizer-4.4.9.1/randomizer/constants.py`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/iogr_rom.py` & `iog-randomizer-4.4.9.1/randomizer/iogr_rom.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .models.enums.goal import Goal
 from .models.enums.statue_req import StatueReq
 from .models.enums.logic import Logic
 from .models.enums.entrance_shuffle import EntranceShuffle
 from .models.enums.enemizer import Enemizer
 from .models.enums.start_location import StartLocation
 
-VERSION = "4.4.9"
+VERSION = "4.4.9.1"
 
 MAX_RANDO_RETRIES = 9
 PRINT_LOG = False
 
 KARA_EDWARDS = 1
 KARA_MINE = 2
 KARA_ANGEL = 3
@@ -850,19 +850,14 @@
 
         # Write room reward initialization routine
         f_roominit = open(BIN_PATH + "00f49a_roominit.bin", "rb")
         patch.seek(int("f49a", 16) + rom_offset)
         patch.write(f_roominit.read())
         f_roominit.close
 
-        # Set "open mode" flag in RAM (for autotracker)
-        if settings.open_mode:
-            patch.seek(int("bfd4e", 16) + rom_offset)
-            patch.write(b"\xff\x02")
-
         ##########################################################################
         #                         Modify South Cape events
         ##########################################################################
         # Teacher sets switch #$38 and spoils Mystic Statues required
         f_teacher = open(BIN_PATH + "048a94_teacher.bin", "rb")
         patch.seek(int("48a94", 16) + rom_offset)
         patch.write(f_teacher.read())
@@ -1176,14 +1171,18 @@
         patch.write(b"\xf3\xc5\x80")
 
         # Update NPC dialogue to acknowledge change
         patch.seek(int("5c331", 16) + rom_offset)
         patch.write(b"\x42\xa2\x80\xa0\x2b\xac\x48\xac\xd6\xae\xa4\x87\x84\xac\xd7\x58\xcb\xa5")
         patch.write(b"\x8d\x8b\x8e\x82\x8a\x84\x83\xac\x80\x86\x80\x88\x8d\x2a\x2a\x2a\xc0")
 
+        # Update NPC dialogue to Neomatamune's quote (congrats tourney winner 2023)
+        patch.seek(int("5bdbf", 16) + rom_offset)
+        patch.write(qt_encode("French don't say Sacre Bleu!") + b"\xc0")
+
         # Add inventory full option to Creepy Guy event
         patch.seek(int("5b6df", 16) + rom_offset)
         patch.write(INV_FULL)
 
         # Alter laborer text
         patch.seek(int("5bfdb", 16) + rom_offset)
         patch.write(b"\xde\xbf")
@@ -2908,14 +2907,18 @@
             patch.write(b"\x18")
 
             if kara_location == KARA_EDWARDS:  # Underground tunnel exit, map 19 (0x13)
                 # Set spoiler for Kara's location in Lance's Letter
                 patch.seek(int("39521", 16) + rom_offset)
                 patch.write(b"\x44\x83\xa7\x80\xa2\x83\x0e\xa3\xac\x60\xa2\x88\xa3\x8e\x8d")
 
+                # Set Kara's location in RAM switches (for autotracker)
+                patch.seek(int("bfd13", 16) + rom_offset)
+                patch.write(b"\x01")
+
                 # Set map check ID for Magic Dust item event
                 patch.seek(int("393a9", 16) + rom_offset)
                 patch.write(b"\x13\x00\xD0\x08\x02\x45\x0b\x0b\x0d\x0d")
 
                 # Set Kara painting event in appropriate map
                 patch.seek(int("c8ac5", 16) + rom_offset)
                 patch.write(b"\x0b\x0b\x00\x4e\xd1\x86\xff\xca")  # this is correct
@@ -2925,14 +2928,18 @@
                 patch.write(b"\x02\xb6\x30")
 
             elif kara_location == KARA_MINE:
                 # Set spoiler for Kara's location in Lance's Letter
                 patch.seek(int("39521", 16) + rom_offset)
                 patch.write(b"\x43\x88\x80\x8c\x8e\x8d\x83\xac\x4c\x88\x8d\x84")
 
+                # Set Kara's location in RAM switches (for autotracker)
+                patch.seek(int("bfd13", 16) + rom_offset)
+                patch.write(b"\x02")
+
                 # Set map check ID for Magic Dust item event
                 patch.seek(int("393a9", 16) + rom_offset)
                 patch.write(b"\x47\x00\xD0\x08\x02\x45\x0b\x24\x0d\x26")
 
                 # Change "Sam" to "Samlet"
                 patch.seek(int("5fee0", 16) + rom_offset)
                 patch.write(b"\x1a\x00\x10\x02\xc0\x9e\xd2\x02\x0b\x02\xc1\x6b")
@@ -2968,14 +2975,18 @@
 
             elif kara_location == KARA_KRESS:
 
                 # Set spoiler for Kara's location in Lance's Letter
                 patch.seek(int("39521", 16) + rom_offset)
                 patch.write(b"\x4c\xa4\x2a\xac\x4a\xa2\x84\xa3\xa3")
 
+                # Set Kara's location in RAM switches (for autotracker)
+                patch.seek(int("bfd13", 16) + rom_offset)
+                patch.write(b"\x04")
+
                 # Set map check ID for Magic Dust item event
                 patch.seek(int("393a9", 16) + rom_offset)
                 patch.write(b"\xa9\x00\xD0\x08\x02\x45\x12\x06\x14\x08")
 
                 # Set Kara painting event in appropriate map
                 # Map #169, written into unused Map #104 (Seaside Tunnel)
                 patch.seek(int("c8152", 16) + rom_offset)
@@ -2989,14 +3000,18 @@
                 patch.write(b"\x02\xb6\x30")
 
             elif kara_location == KARA_ANKORWAT:
                 # Set spoiler for Kara's location in Lance's Letter
                 patch.seek(int("39521", 16) + rom_offset)
                 patch.write(b"\x40\x8d\x8a\x8e\xa2\xac\x67\x80\xa4")
 
+                # Set Kara's location in RAM switches (for autotracker)
+                patch.seek(int("bfd13", 16) + rom_offset)
+                patch.write(b"\x05")
+
                 # Set map check ID for Magic Dust item event
                 patch.seek(int("393a9", 16) + rom_offset)
                 patch.write(b"\xbf\x00\xD0\x08\x02\x45\x1a\x10\x1c\x12")
 
                 # Set Kara painting event in appropriate map (Map #191)
                 # Map #191, written into unused Map #104 (Seaside Tunnel)
                 patch.seek(int("c817e", 16) + rom_offset)
@@ -3005,25 +3020,14 @@
                 patch.write(b"\x05\x0a\x02\x8c\xc3\x82\x00\x00\x00\x00\xed\xea\x80\x00\x0f")
                 patch.write(b"\x0b\x00\xa3\x9a\x88\x00\x1a\x10\x00\x4e\xd1\x86\x00\xff\xca")
 
                 # Adjust sprite
                 patch.seek(int("6d15b", 16) + rom_offset)
                 patch.write(b"\x02\xb6\x30")
 
-        # Set Kara's location and logic mode in RAM switches (for autotracker)
-        if settings.logic.value == Logic.COMPLETABLE.value:
-            logic_int = 0x10 + kara_location
-        elif settings.logic.value == Logic.BEATABLE.value:
-            logic_int = 0x20 + kara_location
-        else:
-            logic_int = 0x40 + kara_location
-
-        patch.seek(int("bfd13", 16) + rom_offset)
-        patch.write(logic_int.to_bytes(1,byteorder="little"))
-
         ##########################################################################
         #                          Have fun with death text
         ##########################################################################
         death_list = []
         death_list.append(
             b"\x2d\x48\xa4\xac\xd6\xa3\xa3\x8e\xac\x87\x80\xa0\xa0\x84\x8d\xa3\xac\xd6\xd7\xcb\xd6\xfe\x85\xa2\x88\x84\x8d\x83\xac\xd7\x73\x88\xa3\xac\xd7\x89\xcb\x4c\x4e\x63\x64\x4b\x69\xac\x83\x84\x80\x83\x2a\x2e\xcb\xac\xac\x6d\x4c\x88\xa2\x80\x82\x8b\x84\xac\x4c\x80\xa8\xc0")
         death_list.append(
```

### Comparing `iog-randomizer-4.4.9/randomizer/models/randomizer_data.py` & `iog-randomizer-4.4.9.1/randomizer/models/randomizer_data.py`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/patch.py` & `iog-randomizer-4.4.9.1/randomizer/patch.py`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/quintet_comp.py` & `iog-randomizer-4.4.9.1/randomizer/quintet_comp.py`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/randomizer/quintet_text.py` & `iog-randomizer-4.4.9.1/randomizer/quintet_text.py`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9/setup.py` & `iog-randomizer-4.4.9.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='iog-randomizer',
-    version='4.4.9',
+    version='4.4.9.1',
     description='The Illusion of Gaia Randomizer',
     author='dontbagume,bryon_w,raeven0',
     packages=setuptools.find_packages(),
     package_data={'': [
         'bin/*.bin',
         'bin/plugins/**/*.bin',
         'bin/plugins/**/**/*.bin'
```

