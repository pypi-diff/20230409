# Comparing `tmp/naruno-0.53.0.tar.gz` & `tmp/naruno-0.54.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno-0.53.0.tar", last modified: Tue Apr  4 12:11:56 2023, max compression
+gzip compressed data, was "naruno-0.54.0.tar", last modified: Sat Apr  8 23:33:43 2023, max compression
```

## Comparing `naruno-0.53.0.tar` & `naruno-0.54.0.tar`

### file list

```diff
@@ -1,300 +1,301 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.222700 naruno-0.53.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-04 12:11:44.000000 naruno-0.53.0/LICENCE-naruno-gui_lib__.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-04 12:11:44.000000 naruno-0.53.0/LICENCE-naruno-lib-mix__.md
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-04 12:11:44.000000 naruno-0.53.0/LICENCE-naruno-wallet-elipticcurve__.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-04 12:11:44.000000 naruno-0.53.0/LICENSE-others__.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-04 12:11:44.000000 naruno-0.53.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-04-04 12:11:56.222700 naruno-0.53.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-04-04 12:11:44.000000 naruno-0.53.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.182700 naruno-0.53.0/naruno/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.182700 naruno-0.53.0/naruno/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/accounts/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.182700 naruno-0.53.0/naruno/accounts/commanders/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/accounts/commanders/delete_commander.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/accounts/commanders/get_comnder.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/accounts/commanders/save_commander.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/accounts/get_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/accounts/get_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/accounts/get_sequence_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/accounts/save_accounts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.182700 naruno-0.53.0/naruno/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.182700 naruno-0.53.0/naruno/api/buildozer/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/api/buildozer/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    24352 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.182700 naruno-0.53.0/naruno/apps/
--rw-r--r--   0 runner    (1001) docker     (123)    26904 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/apps/remote_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.170700 naruno-0.53.0/naruno/blockchain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.186700 naruno-0.53.0/naruno/blockchain/block/
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/blockchain/block/block_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/blockchain/block/blocks_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/blockchain/block/change_transaction_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/blockchain/block/create_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/blockchain/block/get_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/blockchain/block/get_block_from_blockchain_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/blockchain/block/get_minumum_transfer_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.186700 naruno-0.53.0/naruno/blockchain/block/hash/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/blockchain/block/hash/accounts_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/blockchain/block/hash/blocks_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/blockchain/block/hash/calculate_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/blockchain/block/hash/tx_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/blockchain/block/max_data_size.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/blockchain/block/max_tx_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/blockchain/block/save_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/blockchain/block/save_block_to_blockchain_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/blockchain/block/shares.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.186700 naruno-0.53.0/naruno/blockchain/candidate_block/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/blockchain/candidate_block/candidate_block_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.186700 naruno-0.53.0/naruno/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.186700 naruno-0.53.0/naruno/consensus/
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/consensus_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.186700 naruno-0.53.0/naruno/consensus/finished/
--rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/finished/finished_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.186700 naruno-0.53.0/naruno/consensus/finished/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/finished/transactions/transactions_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.186700 naruno-0.53.0/naruno/consensus/finished/true_time/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/finished/true_time/true_time_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.186700 naruno-0.53.0/naruno/consensus/ongoing/
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/ongoing/ongoing_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.174700 naruno-0.53.0/naruno/consensus/rounds/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.186700 naruno-0.53.0/naruno/consensus/rounds/round_1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.186700 naruno-0.53.0/naruno/consensus/rounds/round_1/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.186700 naruno-0.53.0/naruno/consensus/rounds/round_1/checks/candidate_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/rounds/round_1/checks/checks_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.174700 naruno-0.53.0/naruno/consensus/rounds/round_1/checks/time/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.186700 naruno-0.53.0/naruno/consensus/rounds/round_1/checks/time/time_difference/
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/consensus/rounds/round_1/process/
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/rounds/round_1/process/process_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/consensus/rounds/round_1/process/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/consensus/rounds/round_1/process/transactions/checks/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/consensus/rounds/round_1/process/transactions/find_newly/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/consensus/rounds/round_1/process/transactions/find_validated/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/rounds/round_1/round_1_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/consensus/rounds/round_2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/consensus/rounds/round_2/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/rounds/round_2/checks/checks_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.174700 naruno-0.53.0/naruno/consensus/rounds/round_2/checks/time/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/consensus/rounds/round_2/checks/time/time_difference/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/consensus/rounds/round_2/process/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/rounds/round_2/process/process_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/consensus/rounds/round_2/process/rescue/
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/consensus/rounds/round_2/process/validate/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/rounds/round_2/process/validate/validate_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/rounds/round_2/round_2_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/consensus/sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/sync/send_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/sync/send_block_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/consensus/sync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/db/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/db/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/blocks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/db/commanders/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/commanders/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/db/connected_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/connected_nodes/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/db/connected_nodes_test_0/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/connected_nodes_test_0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/db/connected_nodes_test_1/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/connected_nodes_test_1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.190700 naruno-0.53.0/naruno/db/connected_nodes_test_2/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/connected_nodes_test_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/db/extracted_proofs/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/extracted_proofs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/db/my_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/my_transactions/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/db/pending_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/pending_transactions/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/db/pending_transactions_test_0/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/pending_transactions_test_0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/db/pending_transactions_test_1/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/pending_transactions_test_1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/db/pending_transactions_test_2/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/pending_transactions_test_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/db/proof/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/proof/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/db/qrs/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/qrs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/db/remote_app_cache/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/remote_app_cache/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/db/signs/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/signs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/db/test_consensus_trigger_finished/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/test_consensus_trigger_finished/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/db/test_finished_main/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/test_finished_main/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/db/test_finished_main_2/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/test_finished_main_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/db/test_finished_main_3/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/test_finished_main_3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/db/test_finished_main_false_time/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/test_finished_main_false_time/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/db/test_finished_main_no_reset/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/test_finished_main_no_reset/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/db/test_proof_extracted/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/db/test_proof_extracted/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.194700 naruno-0.53.0/naruno/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui/popup.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui/the_naruno_gui_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.178700 naruno-0.53.0/naruno/gui_lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.202700 naruno-0.53.0/naruno/gui_lib/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/fonts/POPPINS_LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)   151396 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/fonts/Poppins-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   171604 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/fonts/Poppins-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   153944 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/fonts/Poppins-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   176588 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/fonts/Poppins-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   152764 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/fonts/Poppins-ExtraBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   173916 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/fonts/Poppins-ExtraBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161456 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/fonts/Poppins-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   186168 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/fonts/Poppins-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   182012 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/fonts/Poppins-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   159892 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/fonts/Poppins-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   184460 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/fonts/Poppins-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   156520 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/fonts/Poppins-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   180444 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/fonts/Poppins-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   158240 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/fonts/Poppins-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   155232 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/fonts/Poppins-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   178584 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/fonts/Poppins-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161652 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/fonts/Poppins-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   187044 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/fonts/Poppins-ThinItalic.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.206700 naruno-0.53.0/naruno/gui_lib/images/
--rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/images/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/images/logo_sm_orb_fw.png
--rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/images/logo_w_bc.png
--rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/images/logo_win.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.178700 naruno-0.53.0/naruno/gui_lib/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.206700 naruno-0.53.0/naruno/gui_lib/libs/baseclass/
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/libs/baseclass/node_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/libs/baseclass/operations_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/libs/baseclass/root_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/libs/baseclass/settings_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/libs/baseclass/tabnavigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/libs/baseclass/wallet_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/libs/baseclass/welcome_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.206700 naruno-0.53.0/naruno/gui_lib/libs/kv/
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/libs/kv/node_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/libs/kv/operations_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/libs/kv/root_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/libs/kv/settings_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/libs/kv/tabnavigation.kv
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/libs/kv/wallet_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/gui_lib/libs/kv/welcome_screen.kv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.210700 naruno-0.53.0/naruno/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.210700 naruno-0.53.0/naruno/lib/backup/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/backup/naruno_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/backup/naruno_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/clean_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/config_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.210700 naruno-0.53.0/naruno/lib/mix/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/mix/merkle_root.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/mix/mixlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.210700 naruno-0.53.0/naruno/lib/performance_analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/performance_analyzers/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/performance_analyzers/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/performance_analyzers/blockshash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/performance_analyzers/blockshash_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/performance_analyzers/heartbeat_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/performance_analyzers/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/perpetualtimer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/safety.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/settings_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/lib/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.210700 naruno-0.53.0/naruno/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/logs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.214700 naruno-0.53.0/naruno/node/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.214700 naruno-0.53.0/naruno/node/client/
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/node/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/node/get_candidate_blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.214700 naruno-0.53.0/naruno/node/server/
--rw-r--r--   0 runner    (1001) docker     (123)    28423 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/node/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/node/unl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.214700 naruno-0.53.0/naruno/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.214700 naruno-0.53.0/naruno/transactions/check/
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/check/check_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.214700 naruno-0.53.0/naruno/transactions/check/datas/
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/check/datas/check_datas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.214700 naruno-0.53.0/naruno/transactions/check/len/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/check/len/check_len.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.214700 naruno-0.53.0/naruno/transactions/check/sign/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/check/sign/check_sign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.214700 naruno-0.53.0/naruno/transactions/check/type/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/check/type/check_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/get_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.214700 naruno-0.53.0/naruno/transactions/my_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/my_transactions/check_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/my_transactions/get_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/my_transactions/get_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/my_transactions/save_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/my_transactions/save_to_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/my_transactions/sended_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/my_transactions/validate_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.214700 naruno-0.53.0/naruno/transactions/pending/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/pending/delete_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/pending/get_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/pending/save_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/pending_to_validating.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/print_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/process_the_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/send.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/transactions/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.218700 naruno-0.53.0/naruno/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/delete_current_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.218700 naruno-0.53.0/naruno/wallet/ellipticcurve/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/ellipticcurve/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/ellipticcurve/ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/ellipticcurve/math.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/ellipticcurve/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/ellipticcurve/privateKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/ellipticcurve/publicKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/ellipticcurve/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.218700 naruno-0.53.0/naruno/wallet/ellipticcurve/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/ellipticcurve/utils/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/ellipticcurve/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/ellipticcurve/utils/der.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/ellipticcurve/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/ellipticcurve/utils/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/ellipticcurve/utils/oid.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/ellipticcurve/utils/pem.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/get_saved_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/print_wallets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/save_wallet_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/wallet_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/wallet_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/wallet_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-04 12:11:44.000000 naruno-0.53.0/naruno/wallet/wallet_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:11:56.182700 naruno-0.53.0/naruno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-04-04 12:11:55.000000 naruno-0.53.0/naruno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-04-04 12:11:56.000000 naruno-0.53.0/naruno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 12:11:55.000000 naruno-0.53.0/naruno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-04 12:11:55.000000 naruno-0.53.0/naruno.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-04 12:11:55.000000 naruno-0.53.0/naruno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 12:11:56.222700 naruno-0.53.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-04 12:11:44.000000 naruno-0.53.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.734332 naruno-0.54.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-08 23:33:31.000000 naruno-0.54.0/LICENCE-naruno-gui_lib__.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-08 23:33:31.000000 naruno-0.54.0/LICENCE-naruno-lib-mix__.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-08 23:33:31.000000 naruno-0.54.0/LICENCE-naruno-wallet-elipticcurve__.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-08 23:33:31.000000 naruno-0.54.0/LICENSE-others__.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-08 23:33:31.000000 naruno-0.54.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-04-08 23:33:43.734332 naruno-0.54.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-04-08 23:33:31.000000 naruno-0.54.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.710332 naruno-0.54.0/naruno/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.710332 naruno-0.54.0/naruno/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/accounts/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.710332 naruno-0.54.0/naruno/accounts/commanders/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/accounts/commanders/delete_commander.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/accounts/commanders/get_comnder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/accounts/commanders/save_commander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/accounts/get_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/accounts/get_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/accounts/get_sequence_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/accounts/save_accounts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.710332 naruno-0.54.0/naruno/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.710332 naruno-0.54.0/naruno/api/buildozer/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/api/buildozer/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24981 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/api/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.710332 naruno-0.54.0/naruno/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)    29526 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/apps/remote_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.706332 naruno-0.54.0/naruno/blockchain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/blockchain/block/
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/blockchain/block/block_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/blockchain/block/blocks_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/blockchain/block/change_transaction_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/blockchain/block/create_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/blockchain/block/get_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/blockchain/block/get_block_from_blockchain_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/blockchain/block/get_minumum_transfer_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/blockchain/block/hash/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/blockchain/block/hash/accounts_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/blockchain/block/hash/blocks_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/blockchain/block/hash/calculate_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/blockchain/block/hash/tx_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/blockchain/block/just_one_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/blockchain/block/max_data_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/blockchain/block/max_tx_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/blockchain/block/save_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/blockchain/block/save_block_to_blockchain_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/blockchain/block/shares.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/blockchain/candidate_block/
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/blockchain/candidate_block/candidate_block_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/consensus_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/finished/
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/finished/finished_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/finished/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/finished/transactions/transactions_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/finished/true_time/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/finished/true_time/true_time_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/ongoing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/ongoing/ongoing_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.706332 naruno-0.54.0/naruno/consensus/rounds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/rounds/round_1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/rounds/round_1/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/rounds/round_1/checks/candidate_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/rounds/round_1/checks/checks_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.706332 naruno-0.54.0/naruno/consensus/rounds/round_1/checks/time/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/rounds/round_1/checks/time/time_difference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/rounds/round_1/process/
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/rounds/round_1/process/process_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/rounds/round_1/process/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/rounds/round_1/process/transactions/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/rounds/round_1/process/transactions/find_newly/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/rounds/round_1/process/transactions/find_validated/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/rounds/round_1/round_1_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/rounds/round_2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/rounds/round_2/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/rounds/round_2/checks/checks_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.706332 naruno-0.54.0/naruno/consensus/rounds/round_2/checks/time/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/rounds/round_2/checks/time/time_difference/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/rounds/round_2/process/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/rounds/round_2/process/process_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/rounds/round_2/process/rescue/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/rounds/round_2/process/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/rounds/round_2/process/validate/validate_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/rounds/round_2/round_2_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/consensus/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/sync/send_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/sync/send_block_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/consensus/sync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.714332 naruno-0.54.0/naruno/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/blocks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/commanders/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/commanders/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/connected_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/connected_nodes/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/connected_nodes_test_0/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/connected_nodes_test_0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/connected_nodes_test_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/connected_nodes_test_1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/connected_nodes_test_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/connected_nodes_test_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/extracted_proofs/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/extracted_proofs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/my_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/my_transactions/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/pending_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/pending_transactions/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/pending_transactions_test_0/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/pending_transactions_test_0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/pending_transactions_test_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/pending_transactions_test_1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/pending_transactions_test_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/pending_transactions_test_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/proof/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/proof/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/qrs/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/qrs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/remote_app_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/remote_app_cache/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/signs/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/signs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/test_consensus_trigger_finished/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/test_consensus_trigger_finished/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/test_finished_main/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/test_finished_main/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/test_finished_main_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/test_finished_main_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/test_finished_main_3/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/test_finished_main_3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/test_finished_main_false_time/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/test_finished_main_false_time/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/test_finished_main_no_reset/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/test_finished_main_no_reset/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/db/test_proof_extracted/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/db/test_proof_extracted/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.718332 naruno-0.54.0/naruno/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui/popup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui/the_naruno_gui_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.706332 naruno-0.54.0/naruno/gui_lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.722332 naruno-0.54.0/naruno/gui_lib/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/fonts/POPPINS_LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)   151396 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/fonts/Poppins-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   171604 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/fonts/Poppins-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   153944 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/fonts/Poppins-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   176588 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/fonts/Poppins-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   152764 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/fonts/Poppins-ExtraBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   173916 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/fonts/Poppins-ExtraBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161456 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/fonts/Poppins-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   186168 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/fonts/Poppins-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   182012 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/fonts/Poppins-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   159892 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/fonts/Poppins-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   184460 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/fonts/Poppins-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156520 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/fonts/Poppins-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   180444 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/fonts/Poppins-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   158240 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/fonts/Poppins-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155232 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/fonts/Poppins-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   178584 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/fonts/Poppins-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161652 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/fonts/Poppins-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   187044 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/fonts/Poppins-ThinItalic.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.726332 naruno-0.54.0/naruno/gui_lib/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/images/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/images/logo_sm_orb_fw.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/images/logo_w_bc.png
+-rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/images/logo_win.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.706332 naruno-0.54.0/naruno/gui_lib/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.726332 naruno-0.54.0/naruno/gui_lib/libs/baseclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/libs/baseclass/node_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/libs/baseclass/operations_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/libs/baseclass/root_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/libs/baseclass/settings_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/libs/baseclass/tabnavigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/libs/baseclass/wallet_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/libs/baseclass/welcome_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.726332 naruno-0.54.0/naruno/gui_lib/libs/kv/
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/libs/kv/node_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/libs/kv/operations_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/libs/kv/root_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/libs/kv/settings_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/libs/kv/tabnavigation.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/libs/kv/wallet_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/gui_lib/libs/kv/welcome_screen.kv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.730332 naruno-0.54.0/naruno/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.730332 naruno-0.54.0/naruno/lib/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/backup/naruno_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/backup/naruno_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/clean_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/config_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.730332 naruno-0.54.0/naruno/lib/mix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/mix/merkle_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/mix/mixlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.730332 naruno-0.54.0/naruno/lib/performance_analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/performance_analyzers/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/performance_analyzers/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/performance_analyzers/blockshash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/performance_analyzers/blockshash_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/performance_analyzers/heartbeat_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/performance_analyzers/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/perpetualtimer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/safety.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/settings_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/lib/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.730332 naruno-0.54.0/naruno/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/logs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.730332 naruno-0.54.0/naruno/node/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.730332 naruno-0.54.0/naruno/node/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/node/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/node/get_candidate_blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.730332 naruno-0.54.0/naruno/node/server/
+-rw-r--r--   0 runner    (1001) docker     (123)    28423 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/node/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/node/unl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.730332 naruno-0.54.0/naruno/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.730332 naruno-0.54.0/naruno/transactions/check/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/check/check_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.730332 naruno-0.54.0/naruno/transactions/check/datas/
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/check/datas/check_datas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.730332 naruno-0.54.0/naruno/transactions/check/len/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/check/len/check_len.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.730332 naruno-0.54.0/naruno/transactions/check/sign/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/check/sign/check_sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.730332 naruno-0.54.0/naruno/transactions/check/type/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/check/type/check_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/get_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.730332 naruno-0.54.0/naruno/transactions/my_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/my_transactions/check_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/my_transactions/get_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/my_transactions/get_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/my_transactions/save_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/my_transactions/save_to_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/my_transactions/sended_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/my_transactions/validate_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.734332 naruno-0.54.0/naruno/transactions/pending/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/pending/delete_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/pending/get_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/pending/save_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/pending_to_validating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/print_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/process_the_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/transactions/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.734332 naruno-0.54.0/naruno/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/delete_current_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.734332 naruno-0.54.0/naruno/wallet/ellipticcurve/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/ellipticcurve/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/ellipticcurve/ecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/ellipticcurve/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/ellipticcurve/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/ellipticcurve/privateKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/ellipticcurve/publicKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/ellipticcurve/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.734332 naruno-0.54.0/naruno/wallet/ellipticcurve/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/ellipticcurve/utils/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/ellipticcurve/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/ellipticcurve/utils/der.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/ellipticcurve/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/ellipticcurve/utils/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/ellipticcurve/utils/oid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/ellipticcurve/utils/pem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/get_saved_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/print_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/save_wallet_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/wallet_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/wallet_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/wallet_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-08 23:33:31.000000 naruno-0.54.0/naruno/wallet/wallet_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:43.710332 naruno-0.54.0/naruno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-04-08 23:33:43.000000 naruno-0.54.0/naruno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-04-08 23:33:43.000000 naruno-0.54.0/naruno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 23:33:43.000000 naruno-0.54.0/naruno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-08 23:33:43.000000 naruno-0.54.0/naruno.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-08 23:33:43.000000 naruno-0.54.0/naruno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 23:33:43.734332 naruno-0.54.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-08 23:33:31.000000 naruno-0.54.0/setup.py
```

### Comparing `naruno-0.53.0/LICENCE-naruno-gui_lib__.md` & `naruno-0.54.0/LICENCE-naruno-gui_lib__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/LICENCE-naruno-lib-mix__.md` & `naruno-0.54.0/LICENCE-naruno-lib-mix__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/LICENCE-naruno-wallet-elipticcurve__.md` & `naruno-0.54.0/LICENCE-naruno-wallet-elipticcurve__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/LICENSE-others__.md` & `naruno-0.54.0/LICENSE-others__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/PKG-INFO` & `naruno-0.54.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naruno
-Version: 0.53.0
+Version: 0.54.0
 Summary: Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.
 Home-page: https://github.com/Naruno/Naruno
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MPL-2.0
 Description: <p align="center">
           <a href="https://github.com/Naruno/Naruno">
@@ -60,15 +60,15 @@
           </p>
         
           <p align="center">
             <a href="https://github.com/Naruno/Naruno/actions/workflows/codeql-analysis.yml">
           <img src="https://github.com/Naruno/Naruno/actions/workflows/codeql-analysis.yml/badge.svg" alt="CodeQL">
           </a>
           .
-          <a href="https://codebeat.co/projects/github-com-naruno-naruno-master"><img alt="codebeat badge" src="https://codebeat.co/badges/de3a4741-5829-4fbd-9eaf-6ca26689586e" /></a>
+          <a href="https://codebeat.co/projects/github-com-naruno-naruno-master"><img alt="codebeat badge" src="https://codebeat.co/badges/1365faa1-70b1-41d9-80df-4ee49f798e1a" /></a>
           .
           <a href="https://www.codacy.com/gh/Naruno/Naruno/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Naruno/Naruno&amp;utm_campaign=Badge_Grade"><img  alt="codacy badge" src="https://app.codacy.com/project/badge/Grade/b6a1e33964ac4759bc36a02763ca9bcb"/></a>
           </p>
         
           <p align="center">
           <a href="https://codescene.io/projects/36313"><img src="https://codescene.io/projects/36313/status-badges/code-health" alt="Code Health"></a>
           .
@@ -116,22 +116,20 @@
         - Already Automated Workflows
         - 100% Code Coverage with unit, functional and stability tests
         - Already distribute CLI, API and GUI in Android, Windows, MacOS and Linux
         
         - Mobile Master Node Support
         - Two Web3 Integration way as Embedded App (Naruno App Engine) and Remote App (Naruno API)
         
-        - And more... 
+        - And more...
         
         \*Some features will be adjusted in stable release.
         
         The software is written in **PEP8** format and **only** needs dependent libraries for GUI panel. Naruno software, designed with a focus on the **community on the Github platform**, In addition, **Stability**, **Functional** and **Unit** tests of all systems are ready and automated. It also has various structures for **automatic setup of test environments**. It is fully compatible with **Git code management system** and **Agile mindset**.
         
-        
-        
         # Documents
         
         Our documents are available in the [docs](https://github.com/Naruno/Naruno/tree/master/docs) folder and [this](https://docs.naruno.org/) website.
         
         # Contribute
         
         Naruno is a completely community driven project, you can contribute in any way if you follow the [guidelines](https://github.com/Naruno/Naruno/blob/master/CONTRIBUTING.md) and [terms](https://github.com/Naruno/Naruno/blob/master/CODE_OF_CONDUCT.md).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: naruno Version: 0.53.0 Summary: Naruno is a
+Metadata-Version: 2.1 Name: naruno Version: 0.54.0 Summary: Naruno is a
 lightning-fast, secure, and scalable blockchain that is able to create
 transaction proofs and verification via raw data and timestamp. We remove the
 archive nodes and lazy web3 integrations. With Naruno everyone can get the
 proof (5-10MB) of their transactions via their nodes and after everyone can use
 in another node for verification the raw data and timestamp. Also you can
 integrate your web3 applications with 4 code lines (just python for now) via
 our remote app system. Home-page: https://github.com/Naruno/Naruno Author:
```

### Comparing `naruno-0.53.0/README.md` & `naruno-0.54.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
   </p>
 
   <p align="center">
     <a href="https://github.com/Naruno/Naruno/actions/workflows/codeql-analysis.yml">
   <img src="https://github.com/Naruno/Naruno/actions/workflows/codeql-analysis.yml/badge.svg" alt="CodeQL">
   </a>
   .
-  <a href="https://codebeat.co/projects/github-com-naruno-naruno-master"><img alt="codebeat badge" src="https://codebeat.co/badges/de3a4741-5829-4fbd-9eaf-6ca26689586e" /></a>
+  <a href="https://codebeat.co/projects/github-com-naruno-naruno-master"><img alt="codebeat badge" src="https://codebeat.co/badges/1365faa1-70b1-41d9-80df-4ee49f798e1a" /></a>
   .
   <a href="https://www.codacy.com/gh/Naruno/Naruno/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Naruno/Naruno&amp;utm_campaign=Badge_Grade"><img  alt="codacy badge" src="https://app.codacy.com/project/badge/Grade/b6a1e33964ac4759bc36a02763ca9bcb"/></a>
   </p>
 
   <p align="center">
   <a href="https://codescene.io/projects/36313"><img src="https://codescene.io/projects/36313/status-badges/code-health" alt="Code Health"></a>
   .
@@ -108,22 +108,20 @@
 - Already Automated Workflows
 - 100% Code Coverage with unit, functional and stability tests
 - Already distribute CLI, API and GUI in Android, Windows, MacOS and Linux
 
 - Mobile Master Node Support
 - Two Web3 Integration way as Embedded App (Naruno App Engine) and Remote App (Naruno API)
 
-- And more... 
+- And more...
 
 \*Some features will be adjusted in stable release.
 
 The software is written in **PEP8** format and **only** needs dependent libraries for GUI panel. Naruno software, designed with a focus on the **community on the Github platform**, In addition, **Stability**, **Functional** and **Unit** tests of all systems are ready and automated. It also has various structures for **automatic setup of test environments**. It is fully compatible with **Git code management system** and **Agile mindset**.
 
-
-
 # Documents
 
 Our documents are available in the [docs](https://github.com/Naruno/Naruno/tree/master/docs) folder and [this](https://docs.naruno.org/) website.
 
 # Contribute
 
 Naruno is a completely community driven project, you can contribute in any way if you follow the [guidelines](https://github.com/Naruno/Naruno/blob/master/CONTRIBUTING.md) and [terms](https://github.com/Naruno/Naruno/blob/master/CODE_OF_CONDUCT.md).
```

### Comparing `naruno-0.53.0/naruno/accounts/account.py` & `naruno-0.54.0/naruno/accounts/account.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/accounts/commanders/delete_commander.py` & `naruno-0.54.0/naruno/accounts/commanders/delete_commander.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/accounts/commanders/get_comnder.py` & `naruno-0.54.0/naruno/accounts/commanders/get_comnder.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/accounts/commanders/save_commander.py` & `naruno-0.54.0/naruno/accounts/commanders/save_commander.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/accounts/get_accounts.py` & `naruno-0.54.0/naruno/accounts/get_accounts.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/accounts/get_balance.py` & `naruno-0.54.0/naruno/accounts/get_balance.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from urllib.request import urlopen
 
 from naruno.accounts.get_accounts import GetAccounts
 from naruno.blockchain.block.get_block import GetBlock
 from naruno.blockchain.block.get_minumum_transfer_amount import \
     GetMinimumTransferAmount
 from naruno.lib.settings_system import the_settings
+from naruno.transactions.pending.get_pending import GetPending
 from naruno.wallet.wallet_import import Address
 
 
 def GetBalance(user,
                account_list=None,
                dont_convert=False,
                block=None,
@@ -44,8 +45,15 @@
 
         the_account_list = GetAccounts(
         ) if account_list is None else account_list
         the_account_list.execute(
             f"SELECT * FROM account_list WHERE address = '{address}'")
         for row in the_account_list.fetchall():
             balance += row[2]
+            break
+        if not block.just_one_tx:
+            for tx in block.validating_list + GetPending():
+                if Address(tx.fromUser) == user:
+                    balance -= float(tx.amount) + float(tx.transaction_fee)
+                elif tx.toUser == user:
+                    balance += float(tx.amount)
     return balance
```

### Comparing `naruno-0.53.0/naruno/accounts/save_accounts.py` & `naruno-0.54.0/naruno/accounts/save_accounts.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/api/buildozer/main.py` & `naruno-0.54.0/naruno/api/buildozer/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/api/main.py` & `naruno-0.54.0/naruno/api/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 
 from flask_cors import CORS
 
 from naruno.accounts.get_balance import GetBalance
 from naruno.accounts.get_sequence_number import GetSequanceNumber
 from naruno.blockchain.block.create_block import CreateBlock
 from naruno.blockchain.block.get_block import GetBlock
-from naruno.blockchain.block.save_block import SaveBlock
+from naruno.blockchain.block.just_one_tx import GetJustOneTX
 from naruno.blockchain.block.max_data_size import GetMaxDataSize
 from naruno.blockchain.block.max_tx_number import GetMaxTXNumber
+from naruno.blockchain.block.save_block import SaveBlock
 from naruno.consensus.consensus_main import consensus_trigger
 from naruno.lib.export import export_the_transactions
 from naruno.lib.log import get_logger
 from naruno.lib.perpetualtimer import perpetualTimer
 from naruno.lib.safety import safety_check
 from naruno.lib.settings_system import (d_mode_settings, t_mode_settings,
                                         the_settings)
@@ -150,28 +151,31 @@
     address = str(
         request.form["to_user"]) if "to_user" in request.form else None
     amount = float(
         request.form["amount"]) if "amount" in request.form else None
     data = str(request.form["data"]) if "data" in request.form else ""
     password = str(
         request.form["password"]) if "password" in request.form else None
+    sequence_number = str(
+        request.form["sequence_number"]) if "sequence_number" in request.form else None        
     block = None
     with contextlib.suppress(Exception):
         block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
                  if custom_block is None else custom_block)
     send_tx = send(
         password,
         address,
         amount=amount,
         data=data,
         block=block,
         custom_current_time=custom_current_time,
         custom_sequence_number=custom_sequence_number,
         custom_balance=custom_balance,
         custom_account_list=custom_account_list,
+        custom_set_sequence_number=sequence_number,
     )
     if send_tx != False:
         SavetoMyTransaction(send_tx, sended=True)
         if not the_settings()["baklava"]:
             server.send_transaction(
                 send_tx,
                 custom_current_time=custom_current_time,
@@ -597,14 +601,25 @@
     # Check publisher mode
     the_block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
                  if custom_block is None else custom_block)
 
     return jsonify(GetMaxTXNumber(block=the_block))
 
 
+@app.route("/blockjustonetx/get/", methods=["GET"])
+def blockjustonetx_get_page():
+    logger.info(
+        f"{request.remote_addr} {request.method} {request.url} {request.form}")
+    # Check publisher mode
+    the_block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
+                 if custom_block is None else custom_block)
+
+    return jsonify(GetJustOneTX(block=the_block))
+
+
 @app.route("/blockmaxdatasize/get/", methods=["GET"])
 def blockmaxdatasize_get_page():
     logger.info(
         f"{request.remote_addr} {request.method} {request.url} {request.form}")
     # Check publisher mode
 
     the_block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
```

### Comparing `naruno-0.53.0/naruno/apps/remote_app.py` & `naruno-0.54.0/naruno/apps/remote_app.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     SendedTransaction
 from naruno.transactions.my_transactions.validate_transaction import \
     ValidateTransaction
 from naruno.transactions.transaction import Transaction
 from naruno.wallet.wallet_import import Address
 from naruno.wallet.wallet_import import wallet_import
 
+from naruno.lib.perpetualtimer import perpetualTimer
+
 logger = get_logger("REMOTE_APP")
 
 
 class splitted_data:
 
     def __init__(self, split):
         self.split = split
@@ -62,14 +64,15 @@
         password="123",
         sended=False,
         sended_not_validated=False,
         cache_true=True,
         wait_amount=None,
         checking=True,
         commander=None,
+        total_check=None,
     ):
         """
         :param host: The host of the node
         :param port: The port of the node
         :param password: The password of the wallet
         """
         self.app_name = app_name
@@ -92,19 +95,23 @@
 
         self.sended_not_validated = sended_not_validated
 
         self.cache_true = cache_true
 
         self.last_sended = 0
 
+        a_block = Block("Onur")
+
         if wait_amount is None:
-            self.wait_amount = Block("Onur").block_time * 2
+            self.wait_amount = a_block.block_time * 2
         else:
             self.wait_amount = wait_amount
 
+
+
         self.get_cache()
 
         backup_host = copy.copy(self.host)
         backup_port = copy.copy(self.port)
         if the_settings()["baklava"]:
             self.host = "test_net.1.naruno.org"
             self.port = 8000
@@ -116,14 +123,43 @@
             ).text)
         self.max_data_size = int(
             self.prepare_request(
                 "/blockmaxdatasize/get/",
                 type="get",
             ).text)
 
+
+
+
+
+        
+
+        if total_check is not None:
+            self.total_check = total_check
+        else:
+            self.total_check = self.prepare_request(
+                "/blockjustonetx/get/",
+                type="get",
+            ).text
+
+            if "true" in self.total_check:
+                self.total_check = False
+            else:
+                self.total_check = True            
+
+        self.original_wait_amoount = copy.copy(self.wait_amount)
+
+        self.check_thread = None
+        if self.total_check:
+            self.check_thread = perpetualTimer(self.original_wait_amoount, self.checker)
+            self.sequence_number = int(self.prepare_request(f"/sequence/get/?address={wallet_import(-1,3)}", type="get").text.replace("\n", "")) + 1
+            self.wait_amount = 0
+
+
+
         self.host = backup_host
         self.port = backup_port
 
         self.sended_txs = []
 
         self.checking = checking
 
@@ -147,14 +183,18 @@
 
         self.api_thread = threading.Thread(target=self.api.run)
         self.api_thread.start()
         sys.argv = backup
 
     def close(self):
         DeleteCommander(self.commander) if not self.commander is None else None
+        if self.check_thread is not None:
+            while len(self.sended_txs) > 0:
+                time.sleep(10)
+            self.check_thread.cancel()
         if self.api is not None:
             self.api.close()
 
     def disable_cache(self):
         self.cache_true = False
         self.cache = []
 
@@ -302,15 +342,15 @@
                     f"split-{2+splitted_data.index(each_data)}-{split_random}{each_data}",
                     to_user=to_user,
                     force=force,
                     retrysecond=retrysecond,
                 )
 
             self.checking = backup_checking
-            self.checker()
+            self.checker() if self.check_thread is None else None
 
             self.send(
                 action=action,
                 app_data=f"split-1-{split_random}",
                 to_user=to_user,
                 force=force,
                 retrysecond=retrysecond,
@@ -320,17 +360,26 @@
         data = json.dumps(data)
 
         request_body = {
             "password": self.password,
             "to_user": to_user,
             "data": data,
         }
-
-        self.sended_txs.append(
-            [action, app_data, to_user, amount, force, retrysecond, data])
+        
+        if self.wait_amount == 0 and self.total_check:
+            
+            request_body["sequence_number"] = copy.copy(self.sequence_number)
+            
+        alread_in_sended = False
+        for tx in self.sended_txs:
+            if tx[0] == action and tx[1] == app_data and tx[2] == to_user and tx[3] == amount and tx[4] == force and tx[5] == retrysecond and tx[6] == data:
+                alread_in_sended = True
+        if not alread_in_sended:
+            self.sended_txs.append(
+                [action, app_data, to_user, amount, force, retrysecond, data])
 
         if amount is not None:
             request_body["amount"] = amount
 
         response = self.prepare_request("/send/",
                                         type="post",
                                         data=request_body)
@@ -341,32 +390,40 @@
                 logger.info("Trying to send again")
                 return self.send_forcer(action, app_data, to_user, retrysecond)
             return False
         else:
             logger.info(
                 f"Message sent: app_name:{self.app_name} action:{action} data: {data} to: {to_user}"
             )
+            if self.wait_amount == 0 and self.total_check:
+                self.sequence_number += 1
             self.last_sended = time.time()
-            if self.checking:
+            if self.checking and self.check_thread is None:
                 self.checker()
             return True
 
     def checker(self):
         time.sleep(self.wait_amount)
-        backup_sended_not_validated = copy.copy(self.sended_not_validated)
-        backup_sended = copy.copy(self.sended)
-        self.sended_not_validated = False
-        self.sended = True
 
-        new_txs = self.get(get_all=True, disable_caches=True)
 
-        for sended_tx in self.sended_txs[:]:
+        new_txs = self.get(get_all=True, disable_caches=True, from_thread=True, disable_sended_not_validated=True, force_sended=True)
+
+        for sended_tx in self.sended_txs[:self.max_tx_number//2]:
             in_get = False
             with contextlib.suppress(ValueError):
                 self.sended_txs.remove(sended_tx)
+                backup_host = copy.copy(self.host)
+                backup_port = copy.copy(self.port)
+                if the_settings()["baklava"]:
+                    self.host = "test_net.1.naruno.org"
+                    self.port = 8000
+             
+                self.sequence_number = int(self.prepare_request(f"/sequence/get/?address={wallet_import(-1,3)}", type="get").text.replace("\n", "")) + 1
+                self.host = backup_host
+                self.port = backup_port                   
             for vaidated_tx in new_txs:
                 if (vaidated_tx["toUser"] == sended_tx[2]
                         and vaidated_tx["data"]["action"] == json.loads(
                             sended_tx[6])["action"]
                         and vaidated_tx["data"]["app_data"] == json.loads(
                             sended_tx[6])["app_data"]):
                     in_get = True
@@ -377,48 +434,44 @@
                     sended_tx[1],
                     sended_tx[2],
                     sended_tx[3],
                     sended_tx[4],
                     sended_tx[5],
                 )
 
-        self.sended_not_validated = backup_sended_not_validated
-        self.sended = backup_sended
 
-    def get_(self, get_all, disable_caches):
+    def get_(self, get_all, disable_caches, disable_sended_not_validated, force_sended):
         self.get_cache() if not disable_caches else None
         response = self.prepare_request("/transactions/received", type="get")
         transactions = response.json()
 
         transactions_sended = {}
         transactions_sended_not_validated = {}
 
-        if self.sended:
+        if self.sended or force_sended:
             response = self.prepare_request("/transactions/sended/validated",
                                             type="get")
             transactions_sended = response.json()
 
-        if self.sended_not_validated:
+        if self.sended_not_validated and not disable_sended_not_validated:
             response = self.prepare_request(
                 "/transactions/sended/not_validated", type="get")
             transactions_sended_not_validated = response.json()
 
         new_dict = {}
         commanders = GetCommander()
         for transaction in transactions:
-            
             if (transactions[transaction]["transaction"]["signature"]
                     in self.cache) and not get_all:
-
                 continue
             else:
                 if (transactions[transaction]["transaction"]["toUser"]
                         == wallet_import(-1, 3)
-                        or Address(transactions[transaction]["transaction"]["fromUser"])
-                        in commanders):
+                        or Address(transactions[transaction]["transaction"]
+                                   ["fromUser"]) in commanders):
                     new_dict[transaction] = transactions[transaction]
                     the_tx = Transaction.load_json(
                         transactions[transaction]["transaction"])
                     if not transactions[transaction]["transaction"][
                             "data"] == "NP":
                         with contextlib.suppress(json.decoder.JSONDecodeError):
                             transactions[transaction]["transaction"][
@@ -442,15 +495,15 @@
                             ["signature"]) if not disable_caches else None
                 elif transactions[transaction]["transaction"][
                         "fromUser"] == wallet_import(-1, 0):
                     transactions_sended[transaction] = transactions[
                         transaction]
 
         for transaction in transactions_sended:
-            if self.sended:
+            if self.sended or force_sended:
                 if (transactions_sended[transaction]["transaction"]
                     ["signature"] in self.cache) and not get_all:
                     continue
                 else:
                     if transactions_sended[transaction]["transaction"][
                             "fromUser"] == wallet_import(-1, 0):
                         new_dict[transaction] = transactions_sended[
@@ -484,24 +537,24 @@
                             ValidateTransaction(
                                 the_tx) if not get_all else None
                             self.cache.append(
                                 transactions_sended[transaction]["transaction"]
                                 ["signature"]) if not disable_caches else None
         split_not_validated = []
         for transaction in transactions_sended_not_validated:
-            if self.sended_not_validated:
+            if self.sended_not_validated and disable_sended_not_validated:
                 if (transactions_sended_not_validated[transaction]
                     ["transaction"]["signature"]
                         in self.cache) and not get_all:
                     continue
                 else:
                     if transactions_sended_not_validated[transaction][
                             "transaction"]["fromUser"] == wallet_import(-1, 0):
                         the_tx = Transaction.load_json(
-                            transactions_sended[transaction]["transaction"])
+                            transactions_sended_not_validated[transaction]["transaction"])
 
                         new_dict[
                             transaction] = transactions_sended_not_validated[
                                 transaction]
                         if (not transactions_sended_not_validated[transaction]
                             ["transaction"]["data"] == "NP"):
                             with contextlib.suppress(
@@ -646,49 +699,55 @@
             if transaction["fromUser"] == wallet_import(-1, 3):
                 the_tx = Transaction.load_json(transaction)
                 if the_settings()["baklava"] and not transaction["data"][
                         "app_data"].startswith("split-"):
                     SendedTransaction(the_tx) if not get_all else None
                 result.append(transaction)
 
-            elif transaction["toUser"] == wallet_import(-1, 3) or transaction["fromUser"] in commanders:
+            elif (transaction["toUser"] == wallet_import(-1, 3)
+                  or transaction["fromUser"] in commanders):
                 result.append(transaction)
 
         for transaction in result[:]:
             if transaction["data"]["app_data"].startswith("split-"):
                 result.remove(transaction) if not get_all else None
 
         if not len(result) == 0:
             logger.info("New datas received")
 
         return result
 
-    def get(self, get_all=False, disable_caches=False):
+    def get(self, get_all=False, disable_caches=False, from_thread=False, disable_sended_not_validated=False, force_sended=False):
         self.host = copy.copy(self.first_host)
         self.port = copy.copy(self.first_port)
         backup_host = copy.copy(self.host)
         backup_port = copy.copy(self.port)
+
+        if (self.sended or force_sended) and self.check_thread is not None and not from_thread:
+            while len(self.sended_txs) > 0:
+                time.sleep(10)
+
         if the_settings()["baklava"]:
             self.host = "test_net.1.naruno.org"
             self.port = 8000
 
         first = []
         with contextlib.suppress(Exception):
-            first = self.get_(get_all=get_all, disable_caches=disable_caches)
+            first = self.get_(get_all=get_all, disable_caches=disable_caches, disable_sended_not_validated=disable_sended_not_validated, force_sended=force_sended)
         self.host = backup_host
         self.port = backup_port
 
-        second = self.get_(get_all=get_all, disable_caches=disable_caches)
+        second = self.get_(get_all=get_all, disable_caches=disable_caches, disable_sended_not_validated=disable_sended_not_validated, force_sended=force_sended)
 
         the_list = first + second
 
         with contextlib.suppress(TypeError):
             if "print" in inspect.stack()[1].code_context[0]:
                 total = ""
                 for data in the_list:
                     fromUser = data["fromUser"]
                     toUser = data["toUser"]
                     action = data["data"]["action"].replace(self.app_name, "")
                     data = data["data"]["app_data"]
                     total += f"\n-----\nFrom: {fromUser}, To: {toUser} \nApp Name: {self.app_name}, Action: {action} \nData: {data}\n-----"
                 return total
-        return the_list
+        return the_list
```

### Comparing `naruno-0.53.0/naruno/blockchain/block/block_main.py` & `naruno-0.54.0/naruno/blockchain/block/block_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,16 @@
 
         self.validated = False
         self.validated_time = None
 
         self.dowload_true_block = ""
         self.sync = False
 
+        self.just_one_tx = True
+
         self.shares = []
         self.fee_address = creator
 
     def reset_the_block(self, custom_nodes=None):
         """
         When the block is verified and if block have a transaction
         and if block have at least half of the max_tx_number transaction,it saves the block
```

### Comparing `naruno-0.53.0/naruno/blockchain/block/blocks_hash.py` & `naruno-0.54.0/naruno/blockchain/block/blocks_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/blockchain/block/change_transaction_fee.py` & `naruno-0.54.0/naruno/blockchain/block/change_transaction_fee.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/blockchain/block/create_block.py` & `naruno-0.54.0/naruno/blockchain/block/create_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/blockchain/block/get_block.py` & `naruno-0.54.0/naruno/blockchain/block/get_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/blockchain/block/get_block_from_blockchain_db.py` & `naruno-0.54.0/naruno/blockchain/block/get_block_from_blockchain_db.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/blockchain/block/get_minumum_transfer_amount.py` & `naruno-0.54.0/naruno/blockchain/block/get_minumum_transfer_amount.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/blockchain/block/hash/accounts_hash.py` & `naruno-0.54.0/naruno/blockchain/block/hash/accounts_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/blockchain/block/hash/blocks_hash.py` & `naruno-0.54.0/naruno/blockchain/block/hash/blocks_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/blockchain/block/hash/calculate_hash.py` & `naruno-0.54.0/naruno/blockchain/block/hash/calculate_hash.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from naruno.blockchain.block.hash.accounts_hash import AccountsHash
 from naruno.blockchain.block.hash.blocks_hash import BlocksHash
 from naruno.blockchain.block.hash.tx_hash import TransactionsHash
-from naruno.consensus.rounds.round_1.process.transactions.checks.duplicated import Remove_Duplicates
-from naruno.lib.mix.merkle_root import MerkleTree
+from naruno.consensus.rounds.round_1.process.transactions.checks.duplicated import \
+    Remove_Duplicates
 from naruno.lib.log import get_logger
+from naruno.lib.mix.merkle_root import MerkleTree
 
 logger = get_logger("BLOCKCHAIN")
 
+
 def CalculateHash(block, part_of_blocks_hash, the_blocks_hash, the_accounts):
     """
     Calculates and returns the hash of the block.
     """
     logger.info(f"Calculating the hash of the block#{block.sequence_number}")
 
-
     block = Remove_Duplicates(block)
     block.validating_list = sorted(block.validating_list,
-                                    key=lambda x: x.fromUser)
+                                   key=lambda x: x.fromUser)
 
     # Transaction Hash
     validating_list = [tx.dump_json() for tx in block.validating_list]
     logger.debug(f"block.validating_list: {validating_list}")
     tx_hash = TransactionsHash(block)
     logger.debug(f"tx_hash: {tx_hash}")
 
@@ -58,15 +59,16 @@
         str(block.transaction_delay_time),
         str(block.max_data_size),
         str(block.part_amount),
         str(block.max_tx_number),
         str(block.minumum_transfer_amount),
         str(block.round_1_time),
         str(block.round_2_time),
-        #str(block.validated_time),
+        # str(block.validated_time),
+        str(block.just_one_tx),
         str(block.shares),
         str(block.fee_address),
     ]
 
     logger.debug(f"main_list: {main_list}")
 
     the_hash = MerkleTree(main_list).getRootHash()
```

### Comparing `naruno-0.53.0/naruno/blockchain/block/hash/tx_hash.py` & `naruno-0.54.0/naruno/blockchain/block/hash/tx_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/blockchain/block/max_data_size.py` & `naruno-0.54.0/naruno/blockchain/block/max_data_size.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/blockchain/block/max_tx_number.py` & `naruno-0.54.0/naruno/blockchain/block/max_tx_number.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/blockchain/block/save_block.py` & `naruno-0.54.0/naruno/blockchain/block/save_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/blockchain/block/save_block_to_blockchain_db.py` & `naruno-0.54.0/naruno/blockchain/block/save_block_to_blockchain_db.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/blockchain/block/shares.py` & `naruno-0.54.0/naruno/blockchain/block/shares.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/blockchain/candidate_block/candidate_block_main.py` & `naruno-0.54.0/naruno/blockchain/candidate_block/candidate_block_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/cli/main.py` & `naruno-0.54.0/naruno/cli/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/config.py` & `naruno-0.54.0/naruno/config.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/consensus_main.py` & `naruno-0.54.0/naruno/consensus/consensus_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/finished/finished_main.py` & `naruno-0.54.0/naruno/consensus/finished/finished_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/finished/transactions/transactions_main.py` & `naruno-0.54.0/naruno/consensus/finished/transactions/transactions_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/finished/true_time/true_time_main.py` & `naruno-0.54.0/naruno/consensus/finished/true_time/true_time_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/ongoing/ongoing_main.py` & `naruno-0.54.0/naruno/consensus/ongoing/ongoing_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py` & `naruno-0.54.0/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/rounds/round_1/checks/checks_main.py` & `naruno-0.54.0/naruno/consensus/rounds/round_1/checks/checks_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py` & `naruno-0.54.0/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/rounds/round_1/process/process_main.py` & `naruno-0.54.0/naruno/consensus/rounds/round_1/process/process_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py` & `naruno-0.54.0/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py` & `naruno-0.54.0/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py` & `naruno-0.54.0/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py` & `naruno-0.54.0/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/rounds/round_1/round_1_main.py` & `naruno-0.54.0/naruno/consensus/rounds/round_1/round_1_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py` & `naruno-0.54.0/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/rounds/round_2/checks/checks_main.py` & `naruno-0.54.0/naruno/consensus/rounds/round_2/checks/checks_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py` & `naruno-0.54.0/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py` & `naruno-0.54.0/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/rounds/round_2/process/process_main.py` & `naruno-0.54.0/naruno/consensus/rounds/round_2/process/process_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py` & `naruno-0.54.0/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/rounds/round_2/process/validate/validate_main.py` & `naruno-0.54.0/naruno/consensus/rounds/round_2/process/validate/validate_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/rounds/round_2/round_2_main.py` & `naruno-0.54.0/naruno/consensus/rounds/round_2/round_2_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/sync/send_block.py` & `naruno-0.54.0/naruno/consensus/sync/send_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/sync/send_block_hash.py` & `naruno-0.54.0/naruno/consensus/sync/send_block_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/consensus/sync/sync.py` & `naruno-0.54.0/naruno/consensus/sync/sync.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui/main.py` & `naruno-0.54.0/naruno/gui/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui/popup.py` & `naruno-0.54.0/naruno/gui/popup.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/fonts/POPPINS_LICENCE` & `naruno-0.54.0/naruno/gui_lib/fonts/POPPINS_LICENCE`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/fonts/Poppins-Black.ttf` & `naruno-0.54.0/naruno/gui_lib/fonts/Poppins-Black.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/fonts/Poppins-BlackItalic.ttf` & `naruno-0.54.0/naruno/gui_lib/fonts/Poppins-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/fonts/Poppins-Bold.ttf` & `naruno-0.54.0/naruno/gui_lib/fonts/Poppins-Bold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/fonts/Poppins-BoldItalic.ttf` & `naruno-0.54.0/naruno/gui_lib/fonts/Poppins-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/fonts/Poppins-ExtraBold.ttf` & `naruno-0.54.0/naruno/gui_lib/fonts/Poppins-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/fonts/Poppins-ExtraBoldItalic.ttf` & `naruno-0.54.0/naruno/gui_lib/fonts/Poppins-ExtraBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/fonts/Poppins-ExtraLight.ttf` & `naruno-0.54.0/naruno/gui_lib/fonts/Poppins-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/fonts/Poppins-ExtraLightItalic.ttf` & `naruno-0.54.0/naruno/gui_lib/fonts/Poppins-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/fonts/Poppins-Italic.ttf` & `naruno-0.54.0/naruno/gui_lib/fonts/Poppins-Italic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/fonts/Poppins-Light.ttf` & `naruno-0.54.0/naruno/gui_lib/fonts/Poppins-Light.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/fonts/Poppins-LightItalic.ttf` & `naruno-0.54.0/naruno/gui_lib/fonts/Poppins-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/fonts/Poppins-Medium.ttf` & `naruno-0.54.0/naruno/gui_lib/fonts/Poppins-Medium.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/fonts/Poppins-MediumItalic.ttf` & `naruno-0.54.0/naruno/gui_lib/fonts/Poppins-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/fonts/Poppins-Regular.ttf` & `naruno-0.54.0/naruno/gui_lib/fonts/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/fonts/Poppins-SemiBold.ttf` & `naruno-0.54.0/naruno/gui_lib/fonts/Poppins-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/fonts/Poppins-SemiBoldItalic.ttf` & `naruno-0.54.0/naruno/gui_lib/fonts/Poppins-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/fonts/Poppins-Thin.ttf` & `naruno-0.54.0/naruno/gui_lib/fonts/Poppins-Thin.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/fonts/Poppins-ThinItalic.ttf` & `naruno-0.54.0/naruno/gui_lib/fonts/Poppins-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/images/logo.ico` & `naruno-0.54.0/naruno/gui_lib/images/logo.ico`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/images/logo.png` & `naruno-0.54.0/naruno/gui_lib/images/logo.png`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/images/logo_sm_orb_fw.png` & `naruno-0.54.0/naruno/gui_lib/images/logo_sm_orb_fw.png`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/images/logo_w_bc.png` & `naruno-0.54.0/naruno/gui_lib/images/logo_w_bc.png`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/images/logo_win.ico` & `naruno-0.54.0/naruno/gui_lib/images/logo_win.ico`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/libs/baseclass/node_screen.py` & `naruno-0.54.0/naruno/gui_lib/libs/baseclass/node_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/libs/baseclass/operations_screen.py` & `naruno-0.54.0/naruno/gui_lib/libs/baseclass/operations_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/libs/baseclass/root_screen.py` & `naruno-0.54.0/naruno/gui_lib/libs/baseclass/root_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/libs/baseclass/settings_screen.py` & `naruno-0.54.0/naruno/gui_lib/libs/baseclass/settings_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/libs/baseclass/tabnavigation.py` & `naruno-0.54.0/naruno/gui_lib/libs/baseclass/tabnavigation.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/libs/baseclass/wallet_screen.py` & `naruno-0.54.0/naruno/gui_lib/libs/baseclass/wallet_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/libs/baseclass/welcome_screen.py` & `naruno-0.54.0/naruno/gui_lib/libs/baseclass/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/libs/kv/node_screen.kv` & `naruno-0.54.0/naruno/gui_lib/libs/kv/node_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/libs/kv/operations_screen.kv` & `naruno-0.54.0/naruno/gui_lib/libs/kv/operations_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/libs/kv/root_screen.kv` & `naruno-0.54.0/naruno/gui_lib/libs/kv/root_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/libs/kv/settings_screen.kv` & `naruno-0.54.0/naruno/gui_lib/libs/kv/settings_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/libs/kv/tabnavigation.kv` & `naruno-0.54.0/naruno/gui_lib/libs/kv/tabnavigation.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/libs/kv/wallet_screen.kv` & `naruno-0.54.0/naruno/gui_lib/libs/kv/wallet_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/gui_lib/libs/kv/welcome_screen.kv` & `naruno-0.54.0/naruno/gui_lib/libs/kv/welcome_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/backup/naruno_export.py` & `naruno-0.54.0/naruno/lib/backup/naruno_export.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/backup/naruno_import.py` & `naruno-0.54.0/naruno/lib/backup/naruno_import.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/clean_up.py` & `naruno-0.54.0/naruno/lib/clean_up.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/config_system.py` & `naruno-0.54.0/naruno/lib/config_system.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/encryption.py` & `naruno-0.54.0/naruno/lib/encryption.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/export.py` & `naruno-0.54.0/naruno/lib/export.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/log.py` & `naruno-0.54.0/naruno/lib/log.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/mix/merkle_root.py` & `naruno-0.54.0/naruno/lib/mix/merkle_root.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/mix/mixlib.py` & `naruno-0.54.0/naruno/lib/mix/mixlib.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/notification.py` & `naruno-0.54.0/naruno/lib/notification.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/performance_analyzers/accounts.py` & `naruno-0.54.0/naruno/lib/performance_analyzers/accounts.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/performance_analyzers/block.py` & `naruno-0.54.0/naruno/lib/performance_analyzers/block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/performance_analyzers/blockshash.py` & `naruno-0.54.0/naruno/lib/performance_analyzers/blockshash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/performance_analyzers/blockshash_part.py` & `naruno-0.54.0/naruno/lib/performance_analyzers/blockshash_part.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/performance_analyzers/heartbeat_db.py` & `naruno-0.54.0/naruno/lib/performance_analyzers/heartbeat_db.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/performance_analyzers/transactions.py` & `naruno-0.54.0/naruno/lib/performance_analyzers/transactions.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/perpetualtimer.py` & `naruno-0.54.0/naruno/lib/perpetualtimer.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,8 +28,12 @@
 
         if self.interval != 0:
             self.start()
 
     def run(self):
         while not self.finished.wait(self.interval):
             with contextlib.suppress(json.decoder.JSONDecodeError):
-                self.function(*self.args, **self.kwargs)
+                self.function(*self.args, **self.kwargs)
+
+    def cancel(self):
+        self.finished.set()
+        self.join()
```

### Comparing `naruno-0.53.0/naruno/lib/qr.py` & `naruno-0.54.0/naruno/lib/qr.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/safety.py` & `naruno-0.54.0/naruno/lib/safety.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/settings_system.py` & `naruno-0.54.0/naruno/lib/settings_system.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/sign.py` & `naruno-0.54.0/naruno/lib/sign.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/status.py` & `naruno-0.54.0/naruno/lib/status.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/lib/verify.py` & `naruno-0.54.0/naruno/lib/verify.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/node/client/client.py` & `naruno-0.54.0/naruno/node/client/client.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/node/get_candidate_blocks.py` & `naruno-0.54.0/naruno/node/get_candidate_blocks.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/node/server/server.py` & `naruno-0.54.0/naruno/node/server/server.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/node/unl.py` & `naruno-0.54.0/naruno/node/unl.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/transactions/check/check_transaction.py` & `naruno-0.54.0/naruno/transactions/check/check_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/transactions/check/datas/check_datas.py` & `naruno-0.54.0/naruno/transactions/check/datas/check_datas.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,85 +18,85 @@
     block,
     transaction,
     custom_current_time=None,
     custom_balance=None,
     custom_sequence_number=None,
     custom_PENDING_TRANSACTIONS_PATH=None,
     custom_account_list=None,
-    disable_already_in=False
+    disable_already_in=False,
 ):
     """
     Check if the transaction datas are valid
     """
 
-
     if not disable_already_in:
         pending_transactions = GetPending(
-            custom_PENDING_TRANSACTIONS_PATH=custom_PENDING_TRANSACTIONS_PATH)        
+            custom_PENDING_TRANSACTIONS_PATH=custom_PENDING_TRANSACTIONS_PATH)
         for already_tx in pending_transactions + block.validating_list:
             if already_tx.signature == transaction.signature:
                 logger.error("Transaction is already in the pending list")
                 return False
 
         for tx in pending_transactions + block.validating_list:
-            if (tx.fromUser == transaction.fromUser):
-                    if tx.signature != transaction.signature:
-                        if transaction.transaction_time < tx.transaction_time:
+            if (tx.fromUser == transaction.fromUser) and block.just_one_tx:
+                if tx.signature != transaction.signature:
+                    if transaction.transaction_time < tx.transaction_time:
+                        pass
+                    elif transaction.transaction_time == tx.transaction_time:
+                        if transaction.sequence_number < tx.sequence_number:
                             pass
-                        elif transaction.transaction_time == tx.transaction_time:
-                            if transaction.sequence_number < tx.sequence_number:
-                                pass
-                            else:
-                                logger.info("Multiple transaction in one account")
-                                return False
                         else:
                             logger.info("Multiple transaction in one account")
                             return False
-
-    balance = (GetBalance(
-        transaction.fromUser,
-        block=block,
-    ) if custom_balance is None else custom_balance)
-    if balance >= (float(transaction.amount) +
-                   float(transaction.transaction_fee)):
-        pass
-    else:
-        logger.error("Balance is not valid")
-        return False
-
-    if transaction.amount >= block.minumum_transfer_amount:
-        pass
-    else:
-        if (GetBalance(
-                transaction.toUser,
-                account_list=custom_account_list,
-                dont_convert=True,
-                block=block,
-        ) >= 0):
+                    else:
+                        logger.info("Multiple transaction in one account")
+                        return False
+    if not disable_already_in:
+        balance = (GetBalance(
+            transaction.fromUser,
+            block=block,
+        ) if custom_balance is None else custom_balance)
+        if balance >= (float(transaction.amount) +
+                    float(transaction.transaction_fee)):
             pass
         else:
-            logger.error("Minimum transfer amount is not reached")
+            logger.error("Balance is not valid")
             return False
 
+        if transaction.amount >= block.minumum_transfer_amount:
+            pass
+        else:
+            if (GetBalance(
+                    transaction.toUser,
+                    account_list=custom_account_list,
+                    dont_convert=True,
+                    block=block,
+            ) >= 0):
+                pass
+            else:
+                logger.error("Minimum transfer amount is not reached")
+                return False
+
     if transaction.transaction_fee >= block.transaction_fee:
         pass
     else:
         logger.error(
             f"Transaction fee is not reached {transaction.transaction_fee}-{block.transaction_fee}"
         )
         return False
 
-    get_sequence_number = (GetSequanceNumber(transaction.fromUser)
-                           if custom_sequence_number is None else
-                           custom_sequence_number)
-    if transaction.sequence_number == (get_sequence_number + 1):
-        pass
-    else:
-        logger.error("Sequance number is not valid")
-        return False
+    if not disable_already_in:
+        get_sequence_number = (GetSequanceNumber(transaction.fromUser, block=block)
+                            if custom_sequence_number is None else
+                            custom_sequence_number)
+        if transaction.sequence_number == (get_sequence_number + 1):
+            pass
+        else:
+            logger.error("Sequance number is not valid")
+            return False
 
     current_time = (int(time.time())
                     if custom_current_time is None else custom_current_time)
     if (current_time -
             transaction.transaction_time) <= block.transaction_delay_time:
         pass
     else:
```

### Comparing `naruno-0.53.0/naruno/transactions/check/len/check_len.py` & `naruno-0.54.0/naruno/transactions/check/len/check_len.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/transactions/check/sign/check_sign.py` & `naruno-0.54.0/naruno/transactions/check/sign/check_sign.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/transactions/check/type/check_type.py` & `naruno-0.54.0/naruno/transactions/check/type/check_type.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/transactions/cleaner.py` & `naruno-0.54.0/naruno/transactions/cleaner.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
         clean_list = []
         for transaction in list_of_transactions:
             ok = False
             just = True
             for transaction_ in list_of_transactions:
                 if not transaction.__dict__ == transaction_.__dict__:
-                    if transaction.fromUser == transaction_.fromUser:
+                    if transaction.fromUser == transaction_.fromUser and block.just_one_tx:
                         just = False
                         if transaction.sequence_number < transaction_.sequence_number:
                             ok = True
                         
                         elif (transaction.sequence_number ==
                               transaction_.sequence_number):
                             if (transaction.transaction_time <
```

### Comparing `naruno-0.53.0/naruno/transactions/get_transaction.py` & `naruno-0.54.0/naruno/transactions/get_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/transactions/my_transactions/check_proof.py` & `naruno-0.54.0/naruno/transactions/my_transactions/check_proof.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/transactions/my_transactions/get_my_transaction.py` & `naruno-0.54.0/naruno/transactions/my_transactions/get_my_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/transactions/my_transactions/get_proof.py` & `naruno-0.54.0/naruno/transactions/my_transactions/get_proof.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/transactions/my_transactions/save_my_transaction.py` & `naruno-0.54.0/naruno/transactions/my_transactions/save_my_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/transactions/my_transactions/save_to_my_transaction.py` & `naruno-0.54.0/naruno/transactions/my_transactions/save_to_my_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/transactions/my_transactions/sended_transaction.py` & `naruno-0.54.0/naruno/transactions/my_transactions/sended_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/transactions/my_transactions/validate_transaction.py` & `naruno-0.54.0/naruno/transactions/my_transactions/validate_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/transactions/pending/delete_pending.py` & `naruno-0.54.0/naruno/transactions/pending/delete_pending.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/transactions/pending/get_pending.py` & `naruno-0.54.0/naruno/transactions/pending/get_pending.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/transactions/pending/save_pending.py` & `naruno-0.54.0/naruno/transactions/pending/save_pending.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/transactions/pending_to_validating.py` & `naruno-0.54.0/naruno/transactions/pending_to_validating.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/transactions/print_transactions.py` & `naruno-0.54.0/naruno/transactions/print_transactions.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/transactions/process_the_transaction.py` & `naruno-0.54.0/naruno/transactions/process_the_transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                 elif action[1] == "sequence_number":
                     account.sequence_number += action[2]
                 edited_accounts.append(account)
 
     # Syncs new sorted list to block.validating_list
 
     block.validating_list = sorted(temp_validating_list,
-                                   key=lambda x: x.fromUser)
+                                   key=lambda x: x.signature)
 
     new_added_accounts_list = sorted(new_added_accounts_list,
                                      key=lambda x: x.Address)
 
     conn = sqlite3.connect(the_TEMP_ACCOUNTS_PATH)
     c = conn.cursor()
     for changed_account in edited_accounts:
```

### Comparing `naruno-0.53.0/naruno/transactions/send.py` & `naruno-0.54.0/naruno/transactions/send.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     amount=None,
     data="",
     block=None,
     custom_current_time=None,
     custom_sequence_number=None,
     custom_balance=None,
     custom_account_list=None,
+    custom_set_sequence_number=None,
 ):
     """
     The main function for sending the transaction.
 
     Inputs:
         password: The password of the wallet.
         to_user: The address of the recipient.
@@ -75,14 +76,17 @@
 
 
             transaction_fee = float(urlopen("http://test_net.1.naruno.org:8000/blocktransactionfee/get/").read().decode("utf-8"))
             max_tx_number = int(urlopen("http://test_net.1.naruno.org:8000/blockmaxtxnumber/get/").read().decode("utf-8"))
             max_data_size = int(urlopen("http://test_net.1.naruno.org:8000/blockmaxdatasize/get/").read().decode("utf-8"))
             minumum_transfer_amount = int(urlopen("http://test_net.1.naruno.org:8000/blockminumumtransferamount/get/").read().decode("utf-8"))
 
+        if custom_set_sequence_number is not None:
+            sequence_number = custom_set_sequence_number
+
         the_minumum_amount = 0
         if (the_balance >= 0):
             pass
         else:
             the_minumum_amount = minumum_transfer_amount
         amount = amount if amount is not None else the_minumum_amount
```

### Comparing `naruno-0.53.0/naruno/transactions/transaction.py` & `naruno-0.54.0/naruno/transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/wallet/delete_current_wallet.py` & `naruno-0.54.0/naruno/wallet/delete_current_wallet.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/wallet/ellipticcurve/curve.py` & `naruno-0.54.0/naruno/wallet/ellipticcurve/curve.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/wallet/ellipticcurve/ecdsa.py` & `naruno-0.54.0/naruno/wallet/ellipticcurve/ecdsa.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/wallet/ellipticcurve/math.py` & `naruno-0.54.0/naruno/wallet/ellipticcurve/math.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/wallet/ellipticcurve/privateKey.py` & `naruno-0.54.0/naruno/wallet/ellipticcurve/privateKey.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/wallet/ellipticcurve/publicKey.py` & `naruno-0.54.0/naruno/wallet/ellipticcurve/publicKey.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/wallet/ellipticcurve/signature.py` & `naruno-0.54.0/naruno/wallet/ellipticcurve/signature.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/wallet/ellipticcurve/utils/binary.py` & `naruno-0.54.0/naruno/wallet/ellipticcurve/utils/binary.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/wallet/ellipticcurve/utils/compatibility.py` & `naruno-0.54.0/naruno/wallet/ellipticcurve/utils/compatibility.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/wallet/ellipticcurve/utils/der.py` & `naruno-0.54.0/naruno/wallet/ellipticcurve/utils/der.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/wallet/ellipticcurve/utils/oid.py` & `naruno-0.54.0/naruno/wallet/ellipticcurve/utils/oid.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/wallet/get_saved_wallet.py` & `naruno-0.54.0/naruno/wallet/get_saved_wallet.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/wallet/print_wallets.py` & `naruno-0.54.0/naruno/wallet/print_wallets.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/wallet/save_wallet_list.py` & `naruno-0.54.0/naruno/wallet/save_wallet_list.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/wallet/wallet_create.py` & `naruno-0.54.0/naruno/wallet/wallet_create.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/wallet/wallet_delete.py` & `naruno-0.54.0/naruno/wallet/wallet_delete.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/wallet/wallet_import.py` & `naruno-0.54.0/naruno/wallet/wallet_import.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno/wallet/wallet_selector.py` & `naruno-0.54.0/naruno/wallet/wallet_selector.py`

 * *Files identical despite different names*

### Comparing `naruno-0.53.0/naruno.egg-info/PKG-INFO` & `naruno-0.54.0/naruno.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naruno
-Version: 0.53.0
+Version: 0.54.0
 Summary: Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.
 Home-page: https://github.com/Naruno/Naruno
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MPL-2.0
 Description: <p align="center">
           <a href="https://github.com/Naruno/Naruno">
@@ -60,15 +60,15 @@
           </p>
         
           <p align="center">
             <a href="https://github.com/Naruno/Naruno/actions/workflows/codeql-analysis.yml">
           <img src="https://github.com/Naruno/Naruno/actions/workflows/codeql-analysis.yml/badge.svg" alt="CodeQL">
           </a>
           .
-          <a href="https://codebeat.co/projects/github-com-naruno-naruno-master"><img alt="codebeat badge" src="https://codebeat.co/badges/de3a4741-5829-4fbd-9eaf-6ca26689586e" /></a>
+          <a href="https://codebeat.co/projects/github-com-naruno-naruno-master"><img alt="codebeat badge" src="https://codebeat.co/badges/1365faa1-70b1-41d9-80df-4ee49f798e1a" /></a>
           .
           <a href="https://www.codacy.com/gh/Naruno/Naruno/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Naruno/Naruno&amp;utm_campaign=Badge_Grade"><img  alt="codacy badge" src="https://app.codacy.com/project/badge/Grade/b6a1e33964ac4759bc36a02763ca9bcb"/></a>
           </p>
         
           <p align="center">
           <a href="https://codescene.io/projects/36313"><img src="https://codescene.io/projects/36313/status-badges/code-health" alt="Code Health"></a>
           .
@@ -116,22 +116,20 @@
         - Already Automated Workflows
         - 100% Code Coverage with unit, functional and stability tests
         - Already distribute CLI, API and GUI in Android, Windows, MacOS and Linux
         
         - Mobile Master Node Support
         - Two Web3 Integration way as Embedded App (Naruno App Engine) and Remote App (Naruno API)
         
-        - And more... 
+        - And more...
         
         \*Some features will be adjusted in stable release.
         
         The software is written in **PEP8** format and **only** needs dependent libraries for GUI panel. Naruno software, designed with a focus on the **community on the Github platform**, In addition, **Stability**, **Functional** and **Unit** tests of all systems are ready and automated. It also has various structures for **automatic setup of test environments**. It is fully compatible with **Git code management system** and **Agile mindset**.
         
-        
-        
         # Documents
         
         Our documents are available in the [docs](https://github.com/Naruno/Naruno/tree/master/docs) folder and [this](https://docs.naruno.org/) website.
         
         # Contribute
         
         Naruno is a completely community driven project, you can contribute in any way if you follow the [guidelines](https://github.com/Naruno/Naruno/blob/master/CONTRIBUTING.md) and [terms](https://github.com/Naruno/Naruno/blob/master/CODE_OF_CONDUCT.md).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: naruno Version: 0.53.0 Summary: Naruno is a
+Metadata-Version: 2.1 Name: naruno Version: 0.54.0 Summary: Naruno is a
 lightning-fast, secure, and scalable blockchain that is able to create
 transaction proofs and verification via raw data and timestamp. We remove the
 archive nodes and lazy web3 integrations. With Naruno everyone can get the
 proof (5-10MB) of their transactions via their nodes and after everyone can use
 in another node for verification the raw data and timestamp. Also you can
 integrate your web3 applications with 4 code lines (just python for now) via
 our remote app system. Home-page: https://github.com/Naruno/Naruno Author:
```

### Comparing `naruno-0.53.0/naruno.egg-info/SOURCES.txt` & `naruno-0.54.0/naruno.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 naruno/blockchain/block/block_main.py
 naruno/blockchain/block/blocks_hash.py
 naruno/blockchain/block/change_transaction_fee.py
 naruno/blockchain/block/create_block.py
 naruno/blockchain/block/get_block.py
 naruno/blockchain/block/get_block_from_blockchain_db.py
 naruno/blockchain/block/get_minumum_transfer_amount.py
+naruno/blockchain/block/just_one_tx.py
 naruno/blockchain/block/max_data_size.py
 naruno/blockchain/block/max_tx_number.py
 naruno/blockchain/block/save_block.py
 naruno/blockchain/block/save_block_to_blockchain_db.py
 naruno/blockchain/block/shares.py
 naruno/blockchain/block/hash/accounts_hash.py
 naruno/blockchain/block/hash/blocks_hash.py
```

### Comparing `naruno-0.53.0/setup.py` & `naruno-0.54.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup
 
 setup(
     author="Naruno Developers",
     author_email="onur.atakan.ulusoy@naruno.org",
     packages=["naruno"],
     name="naruno",
-    version="0.53.0",
+    version="0.54.0",
     url="https://github.com/Naruno/Naruno",
     description=
     "Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.",
     keywords=[
         "python",
         "cryptography",
         "blockchain",
```

