# Comparing `tmp/lifesci-0.3.1.tar.gz` & `tmp/lifesci-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifesci-0.3.1.tar", last modified: Thu Feb 10 21:23:50 2022, max compression
+gzip compressed data, was "lifesci-0.3.2.tar", last modified: Sun Apr  9 12:48:49 2023, max compression
```

## Comparing `lifesci-0.3.1.tar` & `lifesci-0.3.2.tar`

### file list

```diff
@@ -1,73 +1,88 @@
-drwxr-xr-x   0 bmmalone  (1000) bmmalone  (1000)        0 2022-02-10 21:23:50.311986 lifesci-0.3.1/
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     1071 2022-02-06 15:52:16.000000 lifesci-0.3.1/LICENSE
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     1095 2022-02-10 21:23:50.311986 lifesci-0.3.1/PKG-INFO
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)      565 2022-02-10 21:11:41.000000 lifesci-0.3.1/README.md
-drwxr-xr-x   0 bmmalone  (1000) bmmalone  (1000)        0 2022-02-10 21:23:50.301986 lifesci-0.3.1/lifesci/
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)       76 2022-02-10 21:11:25.000000 lifesci-0.3.1/lifesci/__init__.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     7675 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/amino_acid_utils.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)    12544 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bam_utils.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)   103824 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bed_utils.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)    11998 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio.py
-drwxr-xr-x   0 bmmalone  (1000) bmmalone  (1000)        0 2022-02-10 21:23:50.311986 lifesci-0.3.1/lifesci/bio_programs/
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)        0 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/__init__.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     6141 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/bam_to_wiggle.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     2512 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/bed12_to_gtf.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     2374 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/bedx_to_bedy.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     2476 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/calculate_bed_overlap.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     3222 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/convert_ccds_to_bed.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     1721 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/count_aligned_reads.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     1330 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/count_reads.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     3178 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/create_mygene_report.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     1027 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/dna_to_aa.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     8924 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/download_srr_files.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     1622 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/extract_bed_sequences.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     1392 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/extract_cds_coordinates.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     1993 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/fasta_to_fastq.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     3828 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/fastq_pe_dedupe.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     1412 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/filter_bam_by_ids.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     1684 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/fix_all_bed_files.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)      836 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/get_all_utrs.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     4212 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/get_read_length_distribution.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     6400 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/gtf_to_bed12.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     2668 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/join_long_chromosomes.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     6604 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/merge_isoforms.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     4039 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/parse_meme_names.py
-drwxr-xr-x   0 bmmalone  (1000) bmmalone  (1000)        0 2022-02-10 21:23:50.311986 lifesci-0.3.1/lifesci/bio_programs/plotting/
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)        0 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/plotting/__init__.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     2531 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/plotting/create_aligned_read_count_bar_chart.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     4037 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/plotting/plot_read_length_distribution.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     2098 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/remove_duplicate_bed_entries.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     2237 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/remove_duplicate_sequences.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     1174 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/remove_multimapping_reads.py
--rwxr-xr-x   0 bmmalone  (1000) bmmalone  (1000)     1967 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/reorder_fasta.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     2909 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/run_bowtie.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     2477 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/split_bed12_blocks.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     3775 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/split_long_chromosomes.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     6094 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/bio_programs/subtract_bed.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)    18497 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/fastx_utils.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     9004 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/gene_ontology_utils.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     9638 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/gffread_utils.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)    12072 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/gtf_utils.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     4973 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/igv.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)    10195 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/meme_utils.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     6049 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/metacyc_utils.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     5144 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/mhcnames_utils.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)    11255 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/mygene_utils.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     2660 2022-02-10 21:10:16.000000 lifesci-0.3.1/lifesci/peptide_dataset.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)    10336 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/pyensembl_utils.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     9229 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/sequence_similarity_utils.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     5997 2022-02-06 15:52:16.000000 lifesci-0.3.1/lifesci/star_utils.py
-drwxr-xr-x   0 bmmalone  (1000) bmmalone  (1000)        0 2022-02-10 21:23:50.301986 lifesci-0.3.1/lifesci.egg-info/
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     1095 2022-02-10 21:23:50.000000 lifesci-0.3.1/lifesci.egg-info/PKG-INFO
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     2221 2022-02-10 21:23:50.000000 lifesci-0.3.1/lifesci.egg-info/SOURCES.txt
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)        1 2022-02-10 21:23:50.000000 lifesci-0.3.1/lifesci.egg-info/dependency_links.txt
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     2161 2022-02-10 21:23:50.000000 lifesci-0.3.1/lifesci.egg-info/entry_points.txt
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)        1 2022-02-06 17:00:33.000000 lifesci-0.3.1/lifesci.egg-info/not-zip-safe
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)      360 2022-02-10 21:23:50.000000 lifesci-0.3.1/lifesci.egg-info/requires.txt
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)       14 2022-02-10 21:23:50.000000 lifesci-0.3.1/lifesci.egg-info/top_level.txt
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)      218 2022-02-10 21:23:50.311986 lifesci-0.3.1/setup.cfg
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     3967 2022-02-10 21:11:09.000000 lifesci-0.3.1/setup.py
-drwxr-xr-x   0 bmmalone  (1000) bmmalone  (1000)        0 2022-02-10 21:23:50.311986 lifesci-0.3.1/tests/
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)    20447 2022-02-06 15:52:16.000000 lifesci-0.3.1/tests/TestBedUtils.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)     3555 2022-02-06 15:52:16.000000 lifesci-0.3.1/tests/TestGtfUtils.py
--rw-r--r--   0 bmmalone  (1000) bmmalone  (1000)        0 2022-02-06 15:52:16.000000 lifesci-0.3.1/tests/__init__.py
+drwxr-xr-x   0 brandon   (1000) brandon   (1000)        0 2023-04-09 12:48:49.462580 lifesci-0.3.2/
+-rw-r--r--   0 brandon   (1000) brandon   (1000)      198 2023-04-09 12:29:09.000000 lifesci-0.3.2/.gitignore
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     2106 2023-01-16 15:26:01.000000 lifesci-0.3.2/CHANGELOG.md
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     1071 2023-01-16 15:26:01.000000 lifesci-0.3.2/LICENSE
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     1014 2023-04-09 12:48:49.462580 lifesci-0.3.2/PKG-INFO
+-rw-r--r--   0 brandon   (1000) brandon   (1000)      565 2023-01-16 15:26:01.000000 lifesci-0.3.2/README.md
+drwxr-xr-x   0 brandon   (1000) brandon   (1000)        0 2023-04-09 12:48:49.442580 lifesci-0.3.2/docs/
+-rw-r--r--   0 brandon   (1000) brandon   (1000)      757 2023-01-16 15:26:01.000000 lifesci-0.3.2/docs/Makefile
+-rw-r--r--   0 brandon   (1000) brandon   (1000)  3311384 2023-01-16 15:26:01.000000 lifesci-0.3.2/docs/pybed-utils-notes.pdf
+-rw-r--r--   0 brandon   (1000) brandon   (1000)       48 2023-01-16 15:26:01.000000 lifesci-0.3.2/docs/requirements.txt
+drwxr-xr-x   0 brandon   (1000) brandon   (1000)        0 2023-04-09 12:48:49.442580 lifesci-0.3.2/docs/source/
+-rw-r--r--   0 brandon   (1000) brandon   (1000)       84 2023-01-16 15:26:01.000000 lifesci-0.3.2/docs/source/api.rst
+-rw-r--r--   0 brandon   (1000) brandon   (1000)    12387 2023-01-16 15:26:01.000000 lifesci-0.3.2/docs/source/cli.rst
+-rw-r--r--   0 brandon   (1000) brandon   (1000)    10896 2023-01-16 15:26:01.000000 lifesci-0.3.2/docs/source/conf.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)      283 2023-01-16 15:26:01.000000 lifesci-0.3.2/docs/source/index.rst
+-rw-r--r--   0 brandon   (1000) brandon   (1000)      190 2023-01-16 15:26:01.000000 lifesci-0.3.2/docs/source/intro.rst
+drwxr-xr-x   0 brandon   (1000) brandon   (1000)        0 2023-04-09 12:48:49.452580 lifesci-0.3.2/lifesci/
+-rw-r--r--   0 brandon   (1000) brandon   (1000)      306 2023-04-09 12:29:09.000000 lifesci-0.3.2/lifesci/__init__.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)      160 2023-04-09 12:48:49.000000 lifesci-0.3.2/lifesci/_version.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     7675 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/amino_acid_utils.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)    12544 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bam_utils.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)   103824 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bed_utils.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)    11998 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio.py
+drwxr-xr-x   0 brandon   (1000) brandon   (1000)        0 2023-04-09 12:48:49.462580 lifesci-0.3.2/lifesci/bio_programs/
+-rw-r--r--   0 brandon   (1000) brandon   (1000)        0 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/__init__.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     6141 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/bam_to_wiggle.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     2512 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/bed12_to_gtf.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     2374 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/bedx_to_bedy.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     2476 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/calculate_bed_overlap.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     3222 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/convert_ccds_to_bed.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     1721 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/count_aligned_reads.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     1330 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/count_reads.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     3178 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/create_mygene_report.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     1027 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/dna_to_aa.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     8924 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/download_srr_files.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     1622 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/extract_bed_sequences.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     1392 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/extract_cds_coordinates.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     1993 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/fasta_to_fastq.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     3828 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/fastq_pe_dedupe.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     1412 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/filter_bam_by_ids.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     1684 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/fix_all_bed_files.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)      836 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/get_all_utrs.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     4212 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/get_read_length_distribution.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     6400 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/gtf_to_bed12.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     2668 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/join_long_chromosomes.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     6604 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/merge_isoforms.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     4039 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/parse_meme_names.py
+drwxr-xr-x   0 brandon   (1000) brandon   (1000)        0 2023-04-09 12:48:49.462580 lifesci-0.3.2/lifesci/bio_programs/plotting/
+-rw-r--r--   0 brandon   (1000) brandon   (1000)        0 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/plotting/__init__.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     2531 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/plotting/create_aligned_read_count_bar_chart.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     4037 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/plotting/plot_read_length_distribution.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     2098 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/remove_duplicate_bed_entries.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     2237 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/remove_duplicate_sequences.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     1174 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/remove_multimapping_reads.py
+-rwxr-xr-x   0 brandon   (1000) brandon   (1000)     1967 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/reorder_fasta.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     2909 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/run_bowtie.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     2477 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/split_bed12_blocks.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     3775 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/split_long_chromosomes.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     6094 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/bio_programs/subtract_bed.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)    18497 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/fastx_utils.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     9004 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/gene_ontology_utils.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     9638 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/gffread_utils.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)    12072 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/gtf_utils.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     4973 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/igv.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)    10195 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/meme_utils.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     6049 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/metacyc_utils.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     5144 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/mhcnames_utils.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     3323 2023-04-07 17:18:18.000000 lifesci-0.3.2/lifesci/msa_utils.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)    11255 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/mygene_utils.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     2660 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/peptide_dataset.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)    10336 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/pyensembl_utils.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)    11783 2023-04-07 17:18:18.000000 lifesci-0.3.2/lifesci/sequence_similarity_utils.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     5997 2023-01-16 15:26:01.000000 lifesci-0.3.2/lifesci/star_utils.py
+drwxr-xr-x   0 brandon   (1000) brandon   (1000)        0 2023-04-09 12:48:49.452580 lifesci-0.3.2/lifesci.egg-info/
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     1014 2023-04-09 12:48:49.000000 lifesci-0.3.2/lifesci.egg-info/PKG-INFO
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     2469 2023-04-09 12:48:49.000000 lifesci-0.3.2/lifesci.egg-info/SOURCES.txt
+-rw-r--r--   0 brandon   (1000) brandon   (1000)        1 2023-04-09 12:48:49.000000 lifesci-0.3.2/lifesci.egg-info/dependency_links.txt
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     2160 2023-04-09 12:48:49.000000 lifesci-0.3.2/lifesci.egg-info/entry_points.txt
+-rw-r--r--   0 brandon   (1000) brandon   (1000)        1 2023-04-09 12:48:49.000000 lifesci-0.3.2/lifesci.egg-info/not-zip-safe
+-rw-r--r--   0 brandon   (1000) brandon   (1000)      406 2023-04-09 12:48:49.000000 lifesci-0.3.2/lifesci.egg-info/requires.txt
+-rw-r--r--   0 brandon   (1000) brandon   (1000)       14 2023-04-09 12:48:49.000000 lifesci-0.3.2/lifesci.egg-info/top_level.txt
+-rw-r--r--   0 brandon   (1000) brandon   (1000)      101 2023-01-16 15:26:01.000000 lifesci-0.3.2/readthedocs.yml
+-rw-r--r--   0 brandon   (1000) brandon   (1000)      218 2023-04-09 12:48:49.462580 lifesci-0.3.2/setup.cfg
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     5682 2023-04-09 12:29:09.000000 lifesci-0.3.2/setup.py
+drwxr-xr-x   0 brandon   (1000) brandon   (1000)        0 2023-04-09 12:48:49.462580 lifesci-0.3.2/tests/
+-rw-r--r--   0 brandon   (1000) brandon   (1000)    20447 2023-01-16 15:26:01.000000 lifesci-0.3.2/tests/TestBedUtils.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     3555 2023-01-16 15:26:01.000000 lifesci-0.3.2/tests/TestGtfUtils.py
+-rw-r--r--   0 brandon   (1000) brandon   (1000)        0 2023-01-16 15:26:01.000000 lifesci-0.3.2/tests/__init__.py
```

### Comparing `lifesci-0.3.1/LICENSE` & `lifesci-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/README.md` & `lifesci-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/amino_acid_utils.py` & `lifesci-0.3.2/lifesci/amino_acid_utils.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bam_utils.py` & `lifesci-0.3.2/lifesci/bam_utils.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bed_utils.py` & `lifesci-0.3.2/lifesci/bed_utils.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio.py` & `lifesci-0.3.2/lifesci/bio.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/bam_to_wiggle.py` & `lifesci-0.3.2/lifesci/bio_programs/bam_to_wiggle.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/bed12_to_gtf.py` & `lifesci-0.3.2/lifesci/bio_programs/bed12_to_gtf.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/bedx_to_bedy.py` & `lifesci-0.3.2/lifesci/bio_programs/bedx_to_bedy.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/calculate_bed_overlap.py` & `lifesci-0.3.2/lifesci/bio_programs/calculate_bed_overlap.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/convert_ccds_to_bed.py` & `lifesci-0.3.2/lifesci/bio_programs/convert_ccds_to_bed.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/count_aligned_reads.py` & `lifesci-0.3.2/lifesci/bio_programs/count_aligned_reads.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/count_reads.py` & `lifesci-0.3.2/lifesci/bio_programs/count_reads.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/create_mygene_report.py` & `lifesci-0.3.2/lifesci/bio_programs/create_mygene_report.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/dna_to_aa.py` & `lifesci-0.3.2/lifesci/bio_programs/dna_to_aa.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/download_srr_files.py` & `lifesci-0.3.2/lifesci/bio_programs/download_srr_files.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/extract_bed_sequences.py` & `lifesci-0.3.2/lifesci/bio_programs/extract_bed_sequences.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/extract_cds_coordinates.py` & `lifesci-0.3.2/lifesci/bio_programs/extract_cds_coordinates.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/fasta_to_fastq.py` & `lifesci-0.3.2/lifesci/bio_programs/fasta_to_fastq.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/fastq_pe_dedupe.py` & `lifesci-0.3.2/lifesci/bio_programs/fastq_pe_dedupe.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/filter_bam_by_ids.py` & `lifesci-0.3.2/lifesci/bio_programs/filter_bam_by_ids.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/fix_all_bed_files.py` & `lifesci-0.3.2/lifesci/bio_programs/fix_all_bed_files.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/get_all_utrs.py` & `lifesci-0.3.2/lifesci/bio_programs/get_all_utrs.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/get_read_length_distribution.py` & `lifesci-0.3.2/lifesci/bio_programs/get_read_length_distribution.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/gtf_to_bed12.py` & `lifesci-0.3.2/lifesci/bio_programs/gtf_to_bed12.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/join_long_chromosomes.py` & `lifesci-0.3.2/lifesci/bio_programs/join_long_chromosomes.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/merge_isoforms.py` & `lifesci-0.3.2/lifesci/bio_programs/merge_isoforms.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/parse_meme_names.py` & `lifesci-0.3.2/lifesci/bio_programs/parse_meme_names.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/plotting/create_aligned_read_count_bar_chart.py` & `lifesci-0.3.2/lifesci/bio_programs/plotting/create_aligned_read_count_bar_chart.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/plotting/plot_read_length_distribution.py` & `lifesci-0.3.2/lifesci/bio_programs/plotting/plot_read_length_distribution.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/remove_duplicate_bed_entries.py` & `lifesci-0.3.2/lifesci/bio_programs/remove_duplicate_bed_entries.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/remove_duplicate_sequences.py` & `lifesci-0.3.2/lifesci/bio_programs/remove_duplicate_sequences.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/remove_multimapping_reads.py` & `lifesci-0.3.2/lifesci/bio_programs/remove_multimapping_reads.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/reorder_fasta.py` & `lifesci-0.3.2/lifesci/bio_programs/reorder_fasta.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/run_bowtie.py` & `lifesci-0.3.2/lifesci/bio_programs/run_bowtie.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/split_bed12_blocks.py` & `lifesci-0.3.2/lifesci/bio_programs/split_bed12_blocks.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/split_long_chromosomes.py` & `lifesci-0.3.2/lifesci/bio_programs/split_long_chromosomes.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/bio_programs/subtract_bed.py` & `lifesci-0.3.2/lifesci/bio_programs/subtract_bed.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/fastx_utils.py` & `lifesci-0.3.2/lifesci/fastx_utils.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/gene_ontology_utils.py` & `lifesci-0.3.2/lifesci/gene_ontology_utils.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/gffread_utils.py` & `lifesci-0.3.2/lifesci/gffread_utils.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/gtf_utils.py` & `lifesci-0.3.2/lifesci/gtf_utils.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/igv.py` & `lifesci-0.3.2/lifesci/igv.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/meme_utils.py` & `lifesci-0.3.2/lifesci/meme_utils.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/metacyc_utils.py` & `lifesci-0.3.2/lifesci/metacyc_utils.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/mhcnames_utils.py` & `lifesci-0.3.2/lifesci/mhcnames_utils.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/mygene_utils.py` & `lifesci-0.3.2/lifesci/mygene_utils.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/peptide_dataset.py` & `lifesci-0.3.2/lifesci/peptide_dataset.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/pyensembl_utils.py` & `lifesci-0.3.2/lifesci/pyensembl_utils.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci/sequence_similarity_utils.py` & `lifesci-0.3.2/lifesci/sequence_similarity_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,311 +20,360 @@
 import pyllars.pandas_utils as pd_utils
 
 import lifesci.amino_acid_utils as aa_utils
 import lifesci.fastx_utils as fastx_utils
 
 import Bio
 import Bio.pairwise2
-import Bio.SubsMat.MatrixInfo
 from Bio.Blast.Applications import NcbiblastpCommandline
 
+from typing import Optional
+
+_DEFAULT_BLAST_OUT_FORMAT = '"6 qseqid qseq sseqid sseq qcovs pident mismatch evalue bitscore gapopen gaps qstart qend sstart send"'
 
-_DEFAULT_BLAST_OUT_FORMAT='"6 qseqid qseq sseqid sseq qcovs pident qlen length mismatch evalue bitscore"'
 _DEFAULT_BLAST_OUT_COLUMNS = [
-    'query_ID',
-    'query_seq',
-    'database_ID',
-    'database_seq',
-    'percent_query_coverage',
-    'percent_alignement',
-    'query_seq_len',
-    'database_seq_len',
-    'num_mismatches',
-    'e_value',
-    'bitscore'
+    "query_ID",
+    "query_seq_aligned",
+    "database_ID",
+    "database_seq_aligned",
+    "percent_query_coverage",
+    "percent_alignement",
+    "num_mismatches",
+    "e_value",
+    "bitscore",
+    "gapopen",
+    "gaps",
+    "query_seq_alignment_start",
+    "query_seq_alignment_end",
+    "database_seq_alignment_start",
+    "database_seq_alignment_end",
 ]
 
+# N.B. This currently raises a deprecation error, but using `Bio.Align.substitution_matrices`
+# is significantly slower than using Bio.SubsMat.MatrixInfo
+# import Bio.Align.substitution_matrices
+# DEFAULT_SCORING_MATRIX = Bio.Align.substitution_matrices.load("BLOSUM62")
+import Bio.SubsMat.MatrixInfo
+
 DEFAULT_SCORING_MATRIX = Bio.SubsMat.MatrixInfo.blosum62
 
 # some very large threshold so we always find some matches
 DEFAULT_E_THRESHOLD = 1e10
 
 ###
 # SNebula-related helpers
 ###
 def _calc_l_xi(l_x, l_i):
-    """ Calculate the length normalization term for SNebula """
+    """Calculate the length normalization term for SNebula"""
     num = np.abs(l_i - l_x)
     den = l_x
-    
+
     l_xi = num / den
     return l_xi
 
+
 def get_snebula_score(p_x, p_i, scoring_matrix=DEFAULT_SCORING_MATRIX):
-    """ Calculate the similarity between `p_x` and `p_i` using the SNebula
+    """Calculate the similarity between `p_x` and `p_i` using the SNebula
     formulas
 
     Parameters
     ----------
     p_{x,i} : str
         The peptide sequences
 
     scoring_matrix : dict
         A dictionary which maps two-tuples to scores. Each element in the two
         tuples are amino acids, and the value gives the score of aligning the
         first element with the second element.
-        
+
         Presumably, this is one of the options from `Bio.SubsMat.MatrixInfo`.
-        
+
     Returns
     -------
     score : float
         The snebula similarity score
     """
 
-    p_xi = Bio.pairwise2.align.globaldx(
-        p_x,
-        p_i,
-        scoring_matrix,
-        score_only=True
-    )
-    
-    p_xx = Bio.pairwise2.align.globaldx(
-        p_x,
-        p_x,
-        scoring_matrix,
-        score_only=True
-    )
-    
+    p_xi = Bio.pairwise2.align.globaldx(p_x, p_i, scoring_matrix, score_only=True)
+
+    p_xx = Bio.pairwise2.align.globaldx(p_x, p_x, scoring_matrix, score_only=True)
+
     l_xi = _calc_l_xi(len(p_x), len(p_i))
     e_term = np.exp(-1 * l_xi)
-    
+
     val = p_xi / p_xx * e_term
     return val
 
+
+def _get_snebula_score_helper(row, scoring_matrix=DEFAULT_SCORING_MATRIX):
+    mutated_epitope = row["query_seq_aligned_ungapped"]
+    reference_epitope = row["database_seq_aligned_ungapped"]
+
+    score = get_snebula_score(mutated_epitope, reference_epitope, scoring_matrix)
+
+    ret = {
+        "query_seq_aligned": row["query_seq_aligned"],
+        "database_seq_aligned": row["database_seq_aligned"],
+        "query_seq_aligned_ungapped": mutated_epitope,
+        "database_seq_aligned_ungapped": reference_epitope,
+        "database_ID": row["database_ID"],
+        "snebula_score": score,
+        "num_mismatches": row["num_mismatches"],
+    }
+
+    return ret
+
+
 ###
 # BLOSUM-related helpers
 ###
 def get_normalized_similarity(
-        mutated_epitope,
-        reference_epitope,
-        scoring_matrix=DEFAULT_SCORING_MATRIX):
-    """ Find the alignment similarity between the two epitopes
-    
+    mutated_epitope, reference_epitope, scoring_matrix=DEFAULT_SCORING_MATRIX
+):
+    """Find the alignment similarity between the two epitopes
+
     This function normalizes the score between the two epitopes using the
     similarity score from `mutated_epitope` to itself. This is, the normalized
     similarity is given as: \frac{sim(mut, ref)}{sim(mut, mut)}.
-    
+
     Please see `get_pairwise_normalized_similarity` for a version which
     normalizes by both epitope sequences.
-    
+
     Parameters
     -----------
     {mutated,reference}_epitope : str
         The respective epitope sequences. They can have different lengths.
-        
     scoring_matrix : dict
         A dictionary which maps two-tuples to scores. Each element in the two
         tuples are amino acids, and the value gives the score of aligning the
         first element with the second element.
-        
+
         Presumably, this is one of the options from `Bio.SubsMat.MatrixInfo`.
-        
+
     Returns
     -------
     score : float
         The normalized score as described above.
     """
-    
+
     score_reference_mutant = Bio.pairwise2.align.globaldx(
-        mutated_epitope,
-        reference_epitope,
-        scoring_matrix,
-        score_only=True
+        mutated_epitope, reference_epitope, scoring_matrix, score_only=True
     )
-    
+
     score_mutant_mutant = Bio.pairwise2.align.globaldx(
-        mutated_epitope,
-        mutated_epitope,
-        scoring_matrix,
-        score_only=True
+        mutated_epitope, mutated_epitope, scoring_matrix, score_only=True
     )
-    
-    return (score_reference_mutant/score_mutant_mutant)
+
+    return score_reference_mutant / score_mutant_mutant
+
 
 def get_pairwise_normalized_similarity(
-        epitope_1,
-        epitope_2,
-        scoring_matrix=DEFAULT_SCORING_MATRIX):
-    """ Find the alignment similarity between the two epitopes
-    
+    epitope_1, epitope_2, scoring_matrix=DEFAULT_SCORING_MATRIX
+):
+    """Find the alignment similarity between the two epitopes
+
     This function normalizes the score between the two epitopes using the
     "self-similarity" of both epitope sequences. This is, the normalized
     similarity is given as: \frac{2*sim(e1, e2)}{sim(e1, e1) + sim(e2, e2)}.
-    
+
     Please see `get_normalized_similarity` for a version which
     normalizes only by the self-similarity of `epitope_1`.
-    
+
     Parameters
     -----------
     epitope_{1,2} : str
         The respective epitope sequences. They can have different lengths.
-        
     scoring_matrix : dict
         A dictionary which maps two-tuples to scores. Each element in the two
         tuples are amino acids, and the value gives the score of aligning the
         first element with the second element.
-        
+
         Presumably, this is one of the options from `Bio.SubsMat.MatrixInfo`.
-        
+
     Returns
     -------
     score : float
         The normalized score as described above.
     """
-    
+
     e1_e2_score = Bio.pairwise2.align.globaldx(
-        epitope_1,
-        epitope_2,
-        scoring_matrix,
-        score_only=True
+        epitope_1, epitope_2, scoring_matrix, score_only=True
     )
-    
-    
+
     e1_e1_score = Bio.pairwise2.align.globaldx(
-        epitope_1,
-        epitope_1,
-        scoring_matrix,
-        score_only=True
+        epitope_1, epitope_1, scoring_matrix, score_only=True
     )
-    
-    
+
     e2_e2_score = Bio.pairwise2.align.globaldx(
-        epitope_2,
-        epitope_2,
-        scoring_matrix,
-        score_only=True
+        epitope_2, epitope_2, scoring_matrix, score_only=True
     )
-    
-    sim = 2*e1_e2_score / (e1_e1_score + e2_e2_score)
+
+    sim = 2 * e1_e2_score / (e1_e1_score + e2_e2_score)
     return sim
 
+
 ###
 # BLAST-related helpers
 ###
 
+
 def _get_query_db_length_matches(df, length):
-    m_query = df['query_seq_len'] == length
-    m_db = df['database_seq_len'] == length
+    m_query = df["query_seq_len"] == length
+    m_db = df["database_seq_len"] == length
     m_match = m_query & m_db
     return m_match
 
-def _get_similarity_helper(row,scoring_matrix=DEFAULT_SCORING_MATRIX):
-    mutated_epitope = row['query_seq']
-    reference_epitope = row['database_seq']
-    
+
+def _get_similarity_helper(row, scoring_matrix=DEFAULT_SCORING_MATRIX):
+    mutated_epitope = row["query_seq_aligned_ungapped"]
+    reference_epitope = row["database_seq_aligned_ungapped"]
+
     score = get_normalized_similarity(
-        mutated_epitope, reference_epitope, scoring_matrix)
-    
+        mutated_epitope, reference_epitope, scoring_matrix
+    )
+
     ret = {
-        'query_seq': mutated_epitope,
-        'database_seq': reference_epitope,
-        'database_ID': row['database_ID'],
-        'normalized_similarity': score,
-        'num_mismatches': row['num_mismatches']
+        "query_seq_aligned": row["query_seq_aligned"],
+        "database_seq_aligned": row["database_seq_aligned"],
+        "query_seq_aligned_ungapped": mutated_epitope,
+        "database_seq_aligned_ungapped": reference_epitope,
+        "database_ID": row["database_ID"],
+        "normalized_similarity": score,
+        "num_mismatches": row["num_mismatches"],
     }
-    
+
     return ret
 
+
 def get_similarity_from_blast_hits(
-        sequences,
-        blastdb_path,
-        num_threads=1,
-        identifiers=None,
-        e_value=DEFAULT_E_THRESHOLD,
-        scoring_matrix=DEFAULT_SCORING_MATRIX,
-        query_output_folder=None,
-        delete_query_output_folder=True,
-        progress_bar=True):
-    
+    sequences,
+    blastdb_path: pathlib.Path,
+    num_threads: int = 1,
+    identifiers=None,
+    e_value: float = DEFAULT_E_THRESHOLD,
+    scoring_matrix=DEFAULT_SCORING_MATRIX,
+    query_output_folder: Optional[pathlib.Path] = None,
+    delete_query_output_folder: bool = True,
+    discard_duplicate_matches: bool = True,
+    ungapped: bool = True,
+    qcov_hsp_perc: int = 100,
+    include_complete_blast_output: bool = False,
+    progress_bar: bool = True,
+    gapextend: int = 1,
+    gapopen: int = 9,
+    word_size: int = 3,
+    max_target_seqs: int = 500,
+):
+
     # for logging
-    caller = 'get_similarity_from_blast_hits'
-    
+    caller = "get_similarity_from_blast_hits"
+
     if identifiers is None:
         msg = "[{}]: creating identifiers".format(caller)
         logger.info(msg)
         identifiers = ["seq_{}".format(i) for i in range(len(sequences))]
-        
+
     if query_output_folder is None:
         query_output_folder = tempfile.mkdtemp()
-        
-    msg = ("[{}]: using temp folder: {}".format(caller, query_output_folder))
+
+    msg = "[{}]: using temp folder: {}".format(caller, query_output_folder)
     logger.info(msg)
     query_output_folder = pathlib.Path(query_output_folder)
-    
-    msg = ("[{}]: writing the sequences and identifiers to disk".format(caller))
+
+    msg = "[{}]: writing the sequences and identifiers to disk".format(caller)
     logger.info(msg)
-    query_filename = query_output_folder / 'query.fa'
-    fastx_utils.write_fasta(sequences, identifiers, query_filename)
-    
+    query_filename = query_output_folder / "query.fa"
+
+    seq_ids = list(zip(identifiers, sequences))
+    fastx_utils.write_fasta(seq_ids, query_filename, compress=False)
+
     # create our output path
-    blastp_filename = query_output_folder / 'blastp.tab'
-    
+    blastp_filename = query_output_folder / "blastp.tab"
+
     blp = NcbiblastpCommandline(
         query=str(query_filename),
         out=str(blastp_filename),
         db=blastdb_path,
         outfmt=_DEFAULT_BLAST_OUT_FORMAT,
         evalue=e_value,
-        ungapped=True,
+        ungapped=ungapped,
         comp_based_stats="F",
         num_threads=num_threads,
-        qcov_hsp_perc=100
+        qcov_hsp_perc=qcov_hsp_perc,
+        gapextend=gapextend,
+        gapopen=gapopen,
+        word_size=word_size,
+        max_target_seqs=max_target_seqs,
     )
-    
-    msg = ("calling blastp. command: '{}'".format(blp))
+
+    msg = "calling blastp. command: '{}'".format(blp)
     logger.info(msg)
 
     stdout, stderr = blp()
-    
-    msg = ("[{}]: loading blastp output".format(caller))
+
+    msg = "[{}]: loading blastp output".format(caller)
     logger.info(msg)
     df_blastp = pd.read_csv(
-        blastp_filename,
-        sep='\t',
-        header=None,
-        names=_DEFAULT_BLAST_OUT_COLUMNS
+        blastp_filename, sep="\t", header=None, names=_DEFAULT_BLAST_OUT_COLUMNS
     )
-    
-        
-    msg = ("[{}]: filtering duplicate matches".format(caller))
-    logger.info(msg)
-    
-    cols = ['query_seq', 'database_seq']
-    m_duplicates = df_blastp.duplicated(subset=cols)
+
+    m_duplicates = np.array([False] * len(df_blastp))
+    if discard_duplicate_matches:
+        msg = "[{}]: filtering duplicate matches".format(caller)
+        logger.info(msg)
+
+        cols = ["query_seq", "database_seq"]
+        m_duplicates = df_blastp.duplicated(subset=cols)
 
     msg = "[{}]: filtering sequences with non-standard aa".format(caller)
     logger.info(msg)
-    m_invalid_aa = aa_utils.get_invalid_aa_mask(df_blastp['database_seq'])
-    
+    m_invalid_aa = aa_utils.get_invalid_aa_mask(df_blastp["database_seq_aligned"])
+
     # keep only matches which pass all filters
     m_to_keep = ~m_duplicates & ~m_invalid_aa
     df_blastp = df_blastp[m_to_keep]
+    df_blastp = df_blastp.reset_index(drop=True)
 
-    msg = ("[{}]: calculating sequence similarities".format(caller))
+    msg = "[{}]: calculating sequence similarities".format(caller)
     logger.info(msg)
-    
+
+    df_blastp["query_seq_aligned_ungapped"] = df_blastp[
+        "query_seq_aligned"
+    ].str.replace("-", "")
+    df_blastp["database_seq_aligned_ungapped"] = df_blastp[
+        "database_seq_aligned"
+    ].str.replace("-", "")
+
     similarities = pd_utils.apply(
         df_blastp,
-        _get_similarity_helper,
+        # _get_similarity_helper,
+        _get_snebula_score_helper,
         scoring_matrix=scoring_matrix,
-        progress_bar=progress_bar
+        progress_bar=progress_bar,
     )
-    
-    msg = ("[{}]: building result data frame".format(caller))
+
+    msg = "[{}]: building result data frame".format(caller)
     logger.info(msg)
     df_similarities = pd.DataFrame(similarities)
-    
+
+    if include_complete_blast_output:
+        # the "concat_cols" depends on the exact score used
+        # concat_cols = ["normalized_similarity"]
+        concat_cols = ["snebula_score"]
+        df_similarities = pd.concat([df_blastp, df_similarities[concat_cols]], axis=1)
+
+        q_lens = df_similarities["query_seq_aligned"].str.len()
+        df_similarities["query_seq_gapped_aligned_len"] = q_lens
+
+        q_lens = df_similarities["query_seq_aligned_ungapped"].str.len()
+        df_similarities["query_seq_ungapped_aligned_len"] = q_lens
+
+        d_lens = df_similarities["database_seq_aligned"].str.len()
+        df_similarities["database_seq_gapped_aligned_len"] = d_lens
+
+        d_lens = df_similarities["database_seq_aligned_ungapped"].str.len()
+        df_similarities["database_seq_ungapped_aligned_len"] = d_lens
+
     if delete_query_output_folder:
         shutil.rmtree(query_output_folder)
-    
-    return df_similarities
+
+    return df_similarities
```

### Comparing `lifesci-0.3.1/lifesci/star_utils.py` & `lifesci-0.3.2/lifesci/star_utils.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/lifesci.egg-info/SOURCES.txt` & `lifesci-0.3.2/lifesci.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,37 @@
+.gitignore
+CHANGELOG.md
 LICENSE
 README.md
+readthedocs.yml
 setup.cfg
 setup.py
+docs/Makefile
+docs/pybed-utils-notes.pdf
+docs/requirements.txt
+docs/source/api.rst
+docs/source/cli.rst
+docs/source/conf.py
+docs/source/index.rst
+docs/source/intro.rst
 lifesci/__init__.py
+lifesci/_version.py
 lifesci/amino_acid_utils.py
 lifesci/bam_utils.py
 lifesci/bed_utils.py
 lifesci/bio.py
 lifesci/fastx_utils.py
 lifesci/gene_ontology_utils.py
 lifesci/gffread_utils.py
 lifesci/gtf_utils.py
 lifesci/igv.py
 lifesci/meme_utils.py
 lifesci/metacyc_utils.py
 lifesci/mhcnames_utils.py
+lifesci/msa_utils.py
 lifesci/mygene_utils.py
 lifesci/peptide_dataset.py
 lifesci/pyensembl_utils.py
 lifesci/sequence_similarity_utils.py
 lifesci/star_utils.py
 lifesci.egg-info/PKG-INFO
 lifesci.egg-info/SOURCES.txt
```

### Comparing `lifesci-0.3.1/lifesci.egg-info/entry_points.txt` & `lifesci-0.3.2/lifesci.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,7 @@
 remove-duplicate-sequences = lifesci.bio_programs.remove_duplicate_sequences:main
 remove-multimapping-reads = lifesci.bio_programs.remove_multimapping_reads:main
 reorder-fasta = lifesci.bio_programs.reorder_fasta:main
 run-bowtie = lifesci.bio_programs.run_bowtie:main
 split-bed12-blocks = lifesci.bio_programs.split_bed12_blocks:main
 split-long-chromosomes = lifesci.bio_programs.split_long_chromosomes:main
 subtract-bed = lifesci.bio_programs.subtract_bed:main
-
```

### Comparing `lifesci-0.3.1/tests/TestBedUtils.py` & `lifesci-0.3.2/tests/TestBedUtils.py`

 * *Files identical despite different names*

### Comparing `lifesci-0.3.1/tests/TestGtfUtils.py` & `lifesci-0.3.2/tests/TestGtfUtils.py`

 * *Files identical despite different names*

