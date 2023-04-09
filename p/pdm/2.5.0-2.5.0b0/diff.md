# Comparing `tmp/pdm-2.5.0.tar.gz` & `tmp/pdm-2.5.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-2.5.0.tar", last modified: Sun Apr  9 08:55:32 2023, max compression
+gzip compressed data, was "pdm-2.5.0b0.tar", last modified: Wed Mar 29 07:35:49 2023, max compression
```

## Comparing `pdm-2.5.0.tar` & `pdm-2.5.0b0.tar`

### file list

```diff
@@ -1,270 +1,270 @@
--rw-r--r--   0        0        0   115075 2023-04-09 08:55:21.983793 pdm-2.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     1075 2023-04-09 08:55:21.983793 pdm-2.5.0/LICENSE
--rw-r--r--   0        0        0     1075 2023-04-09 08:55:21.983793 pdm-2.5.0/LICENSE
--rw-r--r--   0        0        0     8229 2023-04-09 08:55:21.983793 pdm-2.5.0/README.md
--rw-r--r--   0        0        0     8229 2023-04-09 08:55:21.983793 pdm-2.5.0/README.md
--rw-r--r--   0        0        0     4423 2023-04-09 08:55:32.151942 pdm-2.5.0/pyproject.toml
--rw-r--r--   0        0        0       65 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/__main__.py
--rw-r--r--   0        0        0      316 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/__version__.py
--rw-r--r--   0        0        0     2432 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/_types.py
--rw-r--r--   0        0        0      237 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/builders/__init__.py
--rw-r--r--   0        0        0    11738 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/builders/base.py
--rw-r--r--   0        0        0     1755 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/builders/editable.py
--rw-r--r--   0        0        0      656 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/builders/sdist.py
--rw-r--r--   0        0        0     1073 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/builders/wheel.py
--rw-r--r--   0        0        0        0 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/__init__.py
--rw-r--r--   0        0        0    33643 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/actions.py
--rw-r--r--   0        0        0        0 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/__init__.py
--rw-r--r--   0        0        0     2404 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/add.py
--rw-r--r--   0        0        0     2255 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/base.py
--rw-r--r--   0        0        0     2380 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/build.py
--rw-r--r--   0        0        0     6529 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/cache.py
--rw-r--r--   0        0        0     1324 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/completion.py
--rw-r--r--   0        0        0     6102 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/config.py
--rw-r--r--   0        0        0     2948 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/export.py
--rw-r--r--   0        0        0     3034 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/fix/__init__.py
--rw-r--r--   0        0        0     2309 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/fix/fixers.py
--rw-r--r--   0        0        0     1071 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/import_cmd.py
--rw-r--r--   0        0        0     2318 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/info.py
--rw-r--r--   0        0        0     5963 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/init.py
--rw-r--r--   0        0        0     2263 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/install.py
--rw-r--r--   0        0        0    15743 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/list.py
--rw-r--r--   0        0        0     1912 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/lock.py
--rw-r--r--   0        0        0     6161 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/publish/__init__.py
--rw-r--r--   0        0        0     7904 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/publish/package.py
--rw-r--r--   0        0        0     4644 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/publish/repository.py
--rw-r--r--   0        0        0     1672 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/remove.py
--rw-r--r--   0        0        0    14018 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/run.py
--rw-r--r--   0        0        0     2436 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/search.py
--rw-r--r--   0        0        0     9364 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/self_cmd.py
--rw-r--r--   0        0        0     2891 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/show.py
--rw-r--r--   0        0        0     1447 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/sync.py
--rw-r--r--   0        0        0     2392 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/update.py
--rw-r--r--   0        0        0     1318 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/use.py
--rw-r--r--   0        0        0     1848 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/venv/__init__.py
--rw-r--r--   0        0        0     2416 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/venv/activate.py
--rw-r--r--   0        0        0     6171 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/venv/backends.py
--rw-r--r--   0        0        0     2155 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/venv/create.py
--rw-r--r--   0        0        0      809 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/venv/list.py
--rw-r--r--   0        0        0     2195 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/venv/purge.py
--rw-r--r--   0        0        0     1276 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/venv/remove.py
--rw-r--r--   0        0        0     3027 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/commands/venv/utils.py
--rw-r--r--   0        0        0        0 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/completions/__init__.py
--rw-r--r--   0        0        0     5025 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/completions/pdm.bash
--rw-r--r--   0        0        0    37111 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/completions/pdm.fish
--rw-r--r--   0        0        0    18492 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/completions/pdm.ps1
--rw-r--r--   0        0        0    24801 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/completions/pdm.zsh
--rw-r--r--   0        0        0     3553 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/filters.py
--rw-r--r--   0        0        0     1481 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/hooks.py
--rw-r--r--   0        0        0    10330 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/options.py
--rw-r--r--   0        0        0    24464 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/cli/utils.py
--rw-r--r--   0        0        0     2409 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/compat.py
--rw-r--r--   0        0        0     9321 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/core.py
--rw-r--r--   0        0        0      904 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/environments/__init__.py
--rw-r--r--   0        0        0     8889 2023-04-09 08:55:21.987793 pdm-2.5.0/src/pdm/environments/base.py
--rw-r--r--   0        0        0     3560 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/environments/local.py
--rw-r--r--   0        0        0      808 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/environments/prefix.py
--rw-r--r--   0        0        0     1614 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/environments/python.py
--rw-r--r--   0        0        0     1377 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/exceptions.py
--rw-r--r--   0        0        0     1086 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/formats/__init__.py
--rw-r--r--   0        0        0     3215 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/formats/base.py
--rw-r--r--   0        0        0     5741 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/formats/flit.py
--rw-r--r--   0        0        0     2349 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/formats/pipfile.py
--rw-r--r--   0        0        0     7289 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/formats/poetry.py
--rw-r--r--   0        0        0     7131 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/formats/requirements.py
--rw-r--r--   0        0        0     2271 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/formats/setup_py.py
--rw-r--r--   0        0        0      119 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/installers/__init__.py
--rw-r--r--   0        0        0     1853 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/installers/core.py
--rw-r--r--   0        0        0    10908 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/installers/installers.py
--rw-r--r--   0        0        0     2091 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/installers/manager.py
--rw-r--r--   0        0        0     2226 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/installers/packages.py
--rw-r--r--   0        0        0    17107 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/installers/synchronizers.py
--rw-r--r--   0        0        0    10903 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/installers/uninstallers.py
--rw-r--r--   0        0        0        0 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/__init__.py
--rw-r--r--   0        0        0     2111 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/auth.py
--rw-r--r--   0        0        0     4394 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/backends.py
--rw-r--r--   0        0        0     9886 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/caches.py
--rw-r--r--   0        0        0    24220 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/candidates.py
--rw-r--r--   0        0        0      287 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/environment.py
--rw-r--r--   0        0        0     1714 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/in_process/__init__.py
--rw-r--r--   0        0        0     2049 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/in_process/get_abi_tag.py
--rw-r--r--   0        0        0     6182 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/in_process/parse_setup.py
--rw-r--r--   0        0        0     1165 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/in_process/pep508.py
--rw-r--r--   0        0        0     1653 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/in_process/sysconfig_get_paths.py
--rw-r--r--   0        0        0     5701 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/markers.py
--rw-r--r--   0        0        0     3507 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/project_info.py
--rw-r--r--   0        0        0     2120 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/python.py
--rw-r--r--   0        0        0      318 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/python_max_versions.json
--rw-r--r--   0        0        0    20760 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/repositories.py
--rw-r--r--   0        0        0    17969 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/requirements.py
--rw-r--r--   0        0        0     2313 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/search.py
--rw-r--r--   0        0        0     1344 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/session.py
--rw-r--r--   0        0        0    14482 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/setup.py
--rw-r--r--   0        0        0    16337 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/specifiers.py
--rw-r--r--   0        0        0     5899 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/versions.py
--rw-r--r--   0        0        0     2721 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/models/working_set.py
--rw-r--r--   0        0        0        0 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/pep582/__init__.py
--rw-r--r--   0        0        0     4481 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/pep582/sitecustomize.py
--rw-r--r--   0        0        0      134 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/project/__init__.py
--rw-r--r--   0        0        0    16212 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/project/config.py
--rw-r--r--   0        0        0    26927 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/project/core.py
--rw-r--r--   0        0        0     1320 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/project/lockfile.py
--rw-r--r--   0        0        0     3046 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/project/project_file.py
--rw-r--r--   0        0        0     1009 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/project/toml_file.py
--rw-r--r--   0        0        0        0 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/py.typed
--rw-r--r--   0        0        0    19636 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/pytest.py
--rw-r--r--   0        0        0       61 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/resolver/__init__.py
--rw-r--r--   0        0        0     1954 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/resolver/core.py
--rw-r--r--   0        0        0    12796 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/resolver/providers.py
--rw-r--r--   0        0        0     1580 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/resolver/python.py
--rw-r--r--   0        0        0     3742 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/resolver/reporters.py
--rw-r--r--   0        0        0     4027 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/signals.py
--rw-r--r--   0        0        0     7966 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/termui.py
--rw-r--r--   0        0        0    13510 2023-04-09 08:55:21.991793 pdm-2.5.0/src/pdm/utils.py
--rw-r--r--   0        0        0       72 2023-04-09 08:55:21.991793 pdm-2.5.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 08:55:21.991793 pdm-2.5.0/tests/cli/__init__.py
--rw-r--r--   0        0        0     2631 2023-04-09 08:55:21.991793 pdm-2.5.0/tests/cli/conftest.py
--rw-r--r--   0        0        0    12370 2023-04-09 08:55:21.991793 pdm-2.5.0/tests/cli/test_add.py
--rw-r--r--   0        0        0     5811 2023-04-09 08:55:21.991793 pdm-2.5.0/tests/cli/test_build.py
--rw-r--r--   0        0        0     5277 2023-04-09 08:55:21.991793 pdm-2.5.0/tests/cli/test_cache.py
--rw-r--r--   0        0        0     7603 2023-04-09 08:55:21.991793 pdm-2.5.0/tests/cli/test_config.py
--rw-r--r--   0        0        0     1131 2023-04-09 08:55:21.991793 pdm-2.5.0/tests/cli/test_fix.py
--rw-r--r--   0        0        0    10432 2023-04-09 08:55:21.991793 pdm-2.5.0/tests/cli/test_hooks.py
--rw-r--r--   0        0        0     4505 2023-04-09 08:55:21.991793 pdm-2.5.0/tests/cli/test_init.py
--rw-r--r--   0        0        0    11265 2023-04-09 08:55:21.991793 pdm-2.5.0/tests/cli/test_install.py
--rw-r--r--   0        0        0    28998 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/cli/test_list.py
--rw-r--r--   0        0        0     4675 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/cli/test_lock.py
--rw-r--r--   0        0        0     7085 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/cli/test_others.py
--rw-r--r--   0        0        0     5740 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/cli/test_publish.py
--rw-r--r--   0        0        0     3872 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/cli/test_remove.py
--rw-r--r--   0        0        0    26440 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/cli/test_run.py
--rw-r--r--   0        0        0     3641 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/cli/test_self_command.py
--rw-r--r--   0        0        0     8806 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/cli/test_update.py
--rw-r--r--   0        0        0     2960 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/cli/test_use.py
--rw-r--r--   0        0        0    10565 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/cli/test_venv.py
--rw-r--r--   0        0        0     3172 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/conftest.py
--rw-r--r--   0        0        0      235 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/fixtures/Pipfile
--rw-r--r--   0        0        0        0 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0    49497 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
--rw-r--r--   0        0        0      546 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
--rw-r--r--   0        0        0   422824 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1254 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
--rw-r--r--   0        0        0     1254 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1038 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/fixtures/artifacts/demo-0.0.1.tar.gz
--rw-r--r--   0        0        0     2615 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/fixtures/artifacts/demo-0.0.1.zip
--rw-r--r--   0        0        0     4595 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
--rw-r--r--   0        0        0     5359 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0    56715 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
--rw-r--r--   0        0        0     6138 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5786 2023-04-09 08:55:21.995793 pdm-2.5.0/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
--rw-r--r--   0        0        0    17978 2023-04-09 08:55:21.999793 pdm-2.5.0/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
--rw-r--r--   0        0        0    24489 2023-04-09 08:55:21.999793 pdm-2.5.0/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0   156727 2023-04-09 08:55:21.999793 pdm-2.5.0/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
--rw-r--r--   0        0        0   305481 2023-04-09 08:55:21.999793 pdm-2.5.0/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
--rw-r--r--   0        0        0   531270 2023-04-09 08:55:22.003793 pdm-2.5.0/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
--rw-r--r--   0        0        0  1232518 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
--rw-r--r--   0        0        0    26662 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
--rw-r--r--   0        0        0    35301 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5312 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
--rw-r--r--   0        0        0      326 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/index/demo.html
--rw-r--r--   0        0        0      511 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/index/future-fstrings.html
--rw-r--r--   0        0        0      262 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/index/pep345-legacy.html
--rw-r--r--   0        0        0      262 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/index/wheel.html
--rw-r--r--   0        0        0        0 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/__init__.py
--rw-r--r--   0        0        0       42 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-#-with-hash/demo.py
--rw-r--r--   0        0        0      332 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-#-with-hash/setup.py
--rw-r--r--   0        0        0       26 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      462 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       42 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-failure-no-dep/demo.py
--rw-r--r--   0        0        0      246 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-failure-no-dep/setup.py
--rw-r--r--   0        0        0       42 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-failure/demo.py
--rw-r--r--   0        0        0      345 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-failure/setup.py
--rw-r--r--   0        0        0       12 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       36 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      442 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0     3983 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
--rw-r--r--   0        0        0      318 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
--rw-r--r--   0        0        0      157 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
--rw-r--r--   0        0        0       12 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       24 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-package/my_package/data.json
--rw-r--r--   0        0        0    29800 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      574 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0      122 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-package/requirements.ini
--rw-r--r--   0        0        0     7521 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      211 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0      728 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-package/setup.txt
--rw-r--r--   0        0        0       21 2023-04-09 08:55:22.007793 pdm-2.5.0/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       18 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/demo-parent-package/README.md
--rw-r--r--   0        0        0       22 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/demo-parent-package/package-a/foo.py
--rw-r--r--   0        0        0      120 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/demo-parent-package/package-a/setup.py
--rw-r--r--   0        0        0       22 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/demo-parent-package/package-b/bar.py
--rw-r--r--   0        0        0      197 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
--rw-r--r--   0        0        0       42 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/demo-prerelease/demo.py
--rw-r--r--   0        0        0      334 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/demo-prerelease/setup.py
--rw-r--r--   0        0        0       12 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      456 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       42 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/demo/demo.py
--rw-r--r--   0        0        0      332 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/demo/setup.py
--rw-r--r--   0        0        0       26 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/demo_extras/demo.py
--rw-r--r--   0        0        0      250 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/demo_extras/setup.py
--rw-r--r--   0        0        0        0 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/flit-demo/README.rst
--rw-r--r--   0        0        0        0 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/flit-demo/doc/index.html
--rw-r--r--   0        0        0       49 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/flit-demo/flit.py
--rw-r--r--   0        0        0      969 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/flit-demo/pyproject.toml
--rw-r--r--   0        0        0       12 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/poetry-demo/mylib.py
--rw-r--r--   0        0        0      863 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/poetry-demo/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-hatch-static/README.md
--rw-r--r--   0        0        0      386 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-hatch-static/pyproject.toml
--rw-r--r--   0        0        0       11 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-monorepo/README.md
--rw-r--r--   0        0        0        0 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-monorepo/core/core.py
--rw-r--r--   0        0        0      179 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-monorepo/core/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-monorepo/package_a/alice.py
--rw-r--r--   0        0        0      231 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-monorepo/package_b/bob.py
--rw-r--r--   0        0        0      231 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
--rw-r--r--   0        0        0      237 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-monorepo/pyproject.toml
--rw-r--r--   0        0        0      380 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-plugin-pdm/hello.py
--rw-r--r--   0        0        0      312 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
--rw-r--r--   0        0        0      380 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-plugin/hello.py
--rw-r--r--   0        0        0      168 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-plugin/setup.py
--rw-r--r--   0        0        0        0 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-removal/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-removal/bar.py
--rw-r--r--   0        0        0        0 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-removal/foo.py
--rw-r--r--   0        0        0        0 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-removal/subdir/__init__.py
--rw-r--r--   0        0        0       10 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-setuptools/AUTHORS
--rw-r--r--   0        0        0       12 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-setuptools/README.md
--rw-r--r--   0        0        0       22 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-setuptools/mymodule.py
--rw-r--r--   0        0        0      398 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-setuptools/setup.cfg
--rw-r--r--   0        0        0      308 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/projects/test-setuptools/setup.py
--rw-r--r--   0        0        0     1525 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/pypi.json
--rw-r--r--   0        0        0     1329 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/pyproject.toml
--rw-r--r--   0        0        0       20 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/requirements-include.txt
--rw-r--r--   0        0        0      502 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/fixtures/requirements.txt
--rw-r--r--   0        0        0        0 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/models/__init__.py
--rw-r--r--   0        0        0     3820 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/models/test_backends.py
--rw-r--r--   0        0        0    12991 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/models/test_candidates.py
--rw-r--r--   0        0        0     1971 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/models/test_marker.py
--rw-r--r--   0        0        0     2679 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/models/test_requirements.py
--rw-r--r--   0        0        0     2526 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/models/test_setup_parsing.py
--rw-r--r--   0        0        0     3418 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/models/test_specifiers.py
--rw-r--r--   0        0        0     2703 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/models/test_versions.py
--rw-r--r--   0        0        0        0 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/resolver/__init__.py
--rw-r--r--   0        0        0    11567 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/resolver/test_resolve.py
--rw-r--r--   0        0        0     7187 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/test_formats.py
--rw-r--r--   0        0        0     7240 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/test_installer.py
--rw-r--r--   0        0        0     1862 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/test_integration.py
--rw-r--r--   0        0        0     2859 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/test_plugin.py
--rw-r--r--   0        0        0    11182 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/test_project.py
--rw-r--r--   0        0        0     1109 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/test_signals.py
--rw-r--r--   0        0        0     4364 2023-04-09 08:55:22.011793 pdm-2.5.0/tests/test_utils.py
--rw-r--r--   0        0        0     9912 1970-01-01 00:00:00.000000 pdm-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0   113672 2023-03-29 07:35:39.122347 pdm-2.5.0b0/CHANGELOG.md
+-rw-r--r--   0        0        0     1075 2023-03-29 07:35:39.122347 pdm-2.5.0b0/LICENSE
+-rw-r--r--   0        0        0     1075 2023-03-29 07:35:39.122347 pdm-2.5.0b0/LICENSE
+-rw-r--r--   0        0        0     8229 2023-03-29 07:35:39.122347 pdm-2.5.0b0/README.md
+-rw-r--r--   0        0        0     8229 2023-03-29 07:35:39.122347 pdm-2.5.0b0/README.md
+-rw-r--r--   0        0        0     4411 2023-03-29 07:35:49.258597 pdm-2.5.0b0/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-03-29 07:35:39.126348 pdm-2.5.0b0/src/pdm/__main__.py
+-rw-r--r--   0        0        0      316 2023-03-29 07:35:39.126348 pdm-2.5.0b0/src/pdm/__version__.py
+-rw-r--r--   0        0        0     2432 2023-03-29 07:35:39.126348 pdm-2.5.0b0/src/pdm/_types.py
+-rw-r--r--   0        0        0      237 2023-03-29 07:35:39.126348 pdm-2.5.0b0/src/pdm/builders/__init__.py
+-rw-r--r--   0        0        0    11738 2023-03-29 07:35:39.126348 pdm-2.5.0b0/src/pdm/builders/base.py
+-rw-r--r--   0        0        0     1755 2023-03-29 07:35:39.126348 pdm-2.5.0b0/src/pdm/builders/editable.py
+-rw-r--r--   0        0        0      656 2023-03-29 07:35:39.126348 pdm-2.5.0b0/src/pdm/builders/sdist.py
+-rw-r--r--   0        0        0     1073 2023-03-29 07:35:39.126348 pdm-2.5.0b0/src/pdm/builders/wheel.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.126348 pdm-2.5.0b0/src/pdm/cli/__init__.py
+-rw-r--r--   0        0        0    33208 2023-03-29 07:35:39.126348 pdm-2.5.0b0/src/pdm/cli/actions.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2366 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/add.py
+-rw-r--r--   0        0        0     2263 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/base.py
+-rw-r--r--   0        0        0     2380 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/build.py
+-rw-r--r--   0        0        0     6529 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/cache.py
+-rw-r--r--   0        0        0     1324 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/completion.py
+-rw-r--r--   0        0        0     6102 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/config.py
+-rw-r--r--   0        0        0     2948 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/export.py
+-rw-r--r--   0        0        0     3034 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/fix/__init__.py
+-rw-r--r--   0        0        0     2260 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/fix/fixers.py
+-rw-r--r--   0        0        0     1071 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/import_cmd.py
+-rw-r--r--   0        0        0     2246 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/info.py
+-rw-r--r--   0        0        0     5963 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/init.py
+-rw-r--r--   0        0        0     2199 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/install.py
+-rw-r--r--   0        0        0    15661 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/list.py
+-rw-r--r--   0        0        0     1912 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/lock.py
+-rw-r--r--   0        0        0     6161 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/publish/__init__.py
+-rw-r--r--   0        0        0     7904 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/publish/package.py
+-rw-r--r--   0        0        0     4648 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/publish/repository.py
+-rw-r--r--   0        0        0     1646 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/remove.py
+-rw-r--r--   0        0        0    13969 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/run.py
+-rw-r--r--   0        0        0     2436 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/search.py
+-rw-r--r--   0        0        0     9364 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/self_cmd.py
+-rw-r--r--   0        0        0     2809 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/show.py
+-rw-r--r--   0        0        0     1409 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/sync.py
+-rw-r--r--   0        0        0     2354 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/update.py
+-rw-r--r--   0        0        0     1174 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/use.py
+-rw-r--r--   0        0        0     2250 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/venv/__init__.py
+-rw-r--r--   0        0        0     2660 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/venv/activate.py
+-rw-r--r--   0        0        0     6171 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/venv/backends.py
+-rw-r--r--   0        0        0     2155 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/venv/create.py
+-rw-r--r--   0        0        0      809 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/venv/list.py
+-rw-r--r--   0        0        0     2195 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/venv/purge.py
+-rw-r--r--   0        0        0     1586 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/venv/remove.py
+-rw-r--r--   0        0        0     2630 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/commands/venv/utils.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/completions/__init__.py
+-rw-r--r--   0        0        0     4955 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/completions/pdm.bash
+-rw-r--r--   0        0        0    35515 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/completions/pdm.fish
+-rw-r--r--   0        0        0    18056 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/completions/pdm.ps1
+-rw-r--r--   0        0        0    23709 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/completions/pdm.zsh
+-rw-r--r--   0        0        0     3502 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/filters.py
+-rw-r--r--   0        0        0     1481 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/hooks.py
+-rw-r--r--   0        0        0     9735 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/options.py
+-rw-r--r--   0        0        0    23990 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/cli/utils.py
+-rw-r--r--   0        0        0     2409 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/compat.py
+-rw-r--r--   0        0        0     9243 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/core.py
+-rw-r--r--   0        0        0      904 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/environments/__init__.py
+-rw-r--r--   0        0        0     8597 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/environments/base.py
+-rw-r--r--   0        0        0     3560 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/environments/local.py
+-rw-r--r--   0        0        0      808 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/environments/prefix.py
+-rw-r--r--   0        0        0     1614 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/environments/python.py
+-rw-r--r--   0        0        0     1377 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/exceptions.py
+-rw-r--r--   0        0        0     1086 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/formats/__init__.py
+-rw-r--r--   0        0        0     3215 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/formats/base.py
+-rw-r--r--   0        0        0     5741 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/formats/flit.py
+-rw-r--r--   0        0        0     2349 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/formats/pipfile.py
+-rw-r--r--   0        0        0     7289 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/formats/poetry.py
+-rw-r--r--   0        0        0     7131 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/formats/requirements.py
+-rw-r--r--   0        0        0     2271 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/formats/setup_py.py
+-rw-r--r--   0        0        0      119 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/installers/__init__.py
+-rw-r--r--   0        0        0     1853 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/installers/core.py
+-rw-r--r--   0        0        0    10908 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/installers/installers.py
+-rw-r--r--   0        0        0     2091 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/installers/manager.py
+-rw-r--r--   0        0        0     2226 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/installers/packages.py
+-rw-r--r--   0        0        0    17107 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/installers/synchronizers.py
+-rw-r--r--   0        0        0    10903 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/installers/uninstallers.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/models/__init__.py
+-rw-r--r--   0        0        0     2111 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/models/auth.py
+-rw-r--r--   0        0        0     4394 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/models/backends.py
+-rw-r--r--   0        0        0     9886 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/models/caches.py
+-rw-r--r--   0        0        0    24208 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/models/candidates.py
+-rw-r--r--   0        0        0      287 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/models/environment.py
+-rw-r--r--   0        0        0     1714 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/models/in_process/__init__.py
+-rw-r--r--   0        0        0     2038 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/models/in_process/get_abi_tag.py
+-rw-r--r--   0        0        0     6182 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/models/in_process/parse_setup.py
+-rw-r--r--   0        0        0     1165 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/models/in_process/pep508.py
+-rw-r--r--   0        0        0     1653 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/models/in_process/sysconfig_get_paths.py
+-rw-r--r--   0        0        0     5701 2023-03-29 07:35:39.130348 pdm-2.5.0b0/src/pdm/models/markers.py
+-rw-r--r--   0        0        0     3507 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/models/project_info.py
+-rw-r--r--   0        0        0     2120 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/models/python.py
+-rw-r--r--   0        0        0      318 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/models/python_max_versions.json
+-rw-r--r--   0        0        0    20238 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/models/repositories.py
+-rw-r--r--   0        0        0    17955 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/models/requirements.py
+-rw-r--r--   0        0        0     2313 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/models/search.py
+-rw-r--r--   0        0        0     1344 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/models/session.py
+-rw-r--r--   0        0        0    14482 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/models/setup.py
+-rw-r--r--   0        0        0    16337 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/models/specifiers.py
+-rw-r--r--   0        0        0     5899 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/models/versions.py
+-rw-r--r--   0        0        0     2721 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/models/working_set.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/pep582/__init__.py
+-rw-r--r--   0        0        0     4481 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/pep582/sitecustomize.py
+-rw-r--r--   0        0        0      134 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/project/__init__.py
+-rw-r--r--   0        0        0    16212 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/project/config.py
+-rw-r--r--   0        0        0    26676 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/project/core.py
+-rw-r--r--   0        0        0     1320 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/project/lockfile.py
+-rw-r--r--   0        0        0     3046 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/project/project_file.py
+-rw-r--r--   0        0        0     1009 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/project/toml_file.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/py.typed
+-rw-r--r--   0        0        0    19636 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/pytest.py
+-rw-r--r--   0        0        0       61 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/resolver/__init__.py
+-rw-r--r--   0        0        0     1954 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/resolver/core.py
+-rw-r--r--   0        0        0    12774 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/resolver/providers.py
+-rw-r--r--   0        0        0     1580 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/resolver/python.py
+-rw-r--r--   0        0        0     3742 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/resolver/reporters.py
+-rw-r--r--   0        0        0     4027 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/signals.py
+-rw-r--r--   0        0        0     7966 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/termui.py
+-rw-r--r--   0        0        0    13770 2023-03-29 07:35:39.134348 pdm-2.5.0b0/src/pdm/utils.py
+-rw-r--r--   0        0        0       72 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/__init__.py
+-rw-r--r--   0        0        0     2631 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12370 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/test_add.py
+-rw-r--r--   0        0        0     5811 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/test_build.py
+-rw-r--r--   0        0        0     5277 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/test_cache.py
+-rw-r--r--   0        0        0     7603 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/test_config.py
+-rw-r--r--   0        0        0     1131 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/test_fix.py
+-rw-r--r--   0        0        0    10432 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/test_hooks.py
+-rw-r--r--   0        0        0     4505 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/test_init.py
+-rw-r--r--   0        0        0    11265 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/test_install.py
+-rw-r--r--   0        0        0    28032 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/test_list.py
+-rw-r--r--   0        0        0     4675 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/test_lock.py
+-rw-r--r--   0        0        0     6192 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/test_others.py
+-rw-r--r--   0        0        0     5740 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/test_publish.py
+-rw-r--r--   0        0        0     3872 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/test_remove.py
+-rw-r--r--   0        0        0    26440 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/test_run.py
+-rw-r--r--   0        0        0     3641 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/test_self_command.py
+-rw-r--r--   0        0        0     8806 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/test_update.py
+-rw-r--r--   0        0        0     2294 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/test_use.py
+-rw-r--r--   0        0        0    10565 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/cli/test_venv.py
+-rw-r--r--   0        0        0     3172 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/conftest.py
+-rw-r--r--   0        0        0      235 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/fixtures/Pipfile
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0    49497 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
+-rw-r--r--   0        0        0      546 2023-03-29 07:35:39.134348 pdm-2.5.0b0/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
+-rw-r--r--   0        0        0   422824 2023-03-29 07:35:39.138348 pdm-2.5.0b0/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1254 2023-03-29 07:35:39.138348 pdm-2.5.0b0/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
+-rw-r--r--   0        0        0     1254 2023-03-29 07:35:39.138348 pdm-2.5.0b0/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1038 2023-03-29 07:35:39.138348 pdm-2.5.0b0/tests/fixtures/artifacts/demo-0.0.1.tar.gz
+-rw-r--r--   0        0        0     2615 2023-03-29 07:35:39.138348 pdm-2.5.0b0/tests/fixtures/artifacts/demo-0.0.1.zip
+-rw-r--r--   0        0        0     4595 2023-03-29 07:35:39.138348 pdm-2.5.0b0/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     5359 2023-03-29 07:35:39.138348 pdm-2.5.0b0/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    56715 2023-03-29 07:35:39.138348 pdm-2.5.0b0/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
+-rw-r--r--   0        0        0     6138 2023-03-29 07:35:39.138348 pdm-2.5.0b0/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5786 2023-03-29 07:35:39.138348 pdm-2.5.0b0/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
+-rw-r--r--   0        0        0    17978 2023-03-29 07:35:39.138348 pdm-2.5.0b0/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
+-rw-r--r--   0        0        0    24489 2023-03-29 07:35:39.138348 pdm-2.5.0b0/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0   156727 2023-03-29 07:35:39.138348 pdm-2.5.0b0/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
+-rw-r--r--   0        0        0   305481 2023-03-29 07:35:39.142348 pdm-2.5.0b0/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0   531270 2023-03-29 07:35:39.142348 pdm-2.5.0b0/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
+-rw-r--r--   0        0        0  1232518 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
+-rw-r--r--   0        0        0    26662 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
+-rw-r--r--   0        0        0    35301 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5312 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
+-rw-r--r--   0        0        0      326 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/index/demo.html
+-rw-r--r--   0        0        0      511 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/index/future-fstrings.html
+-rw-r--r--   0        0        0      262 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/index/pep345-legacy.html
+-rw-r--r--   0        0        0      262 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/index/wheel.html
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/__init__.py
+-rw-r--r--   0        0        0       42 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-#-with-hash/demo.py
+-rw-r--r--   0        0        0      332 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-#-with-hash/setup.py
+-rw-r--r--   0        0        0       26 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      462 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-failure-no-dep/demo.py
+-rw-r--r--   0        0        0      246 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-failure-no-dep/setup.py
+-rw-r--r--   0        0        0       42 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-failure/demo.py
+-rw-r--r--   0        0        0      345 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-failure/setup.py
+-rw-r--r--   0        0        0       12 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       36 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      442 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0     3983 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
+-rw-r--r--   0        0        0      318 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
+-rw-r--r--   0        0        0       12 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-package/my_package/data.json
+-rw-r--r--   0        0        0    29800 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      574 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-package/requirements.ini
+-rw-r--r--   0        0        0     7521 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      211 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0      728 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-package/setup.txt
+-rw-r--r--   0        0        0       21 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       18 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-parent-package/README.md
+-rw-r--r--   0        0        0       22 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-parent-package/package-a/foo.py
+-rw-r--r--   0        0        0      120 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-parent-package/package-a/setup.py
+-rw-r--r--   0        0        0       22 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-parent-package/package-b/bar.py
+-rw-r--r--   0        0        0      197 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-prerelease/demo.py
+-rw-r--r--   0        0        0      334 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-prerelease/setup.py
+-rw-r--r--   0        0        0       12 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      456 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       42 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo/demo.py
+-rw-r--r--   0        0        0      332 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo/setup.py
+-rw-r--r--   0        0        0       26 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo_extras/demo.py
+-rw-r--r--   0        0        0      250 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/demo_extras/setup.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/flit-demo/README.rst
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/flit-demo/doc/index.html
+-rw-r--r--   0        0        0       49 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/flit-demo/flit.py
+-rw-r--r--   0        0        0      969 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/flit-demo/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/poetry-demo/mylib.py
+-rw-r--r--   0        0        0      863 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/poetry-demo/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/test-hatch-static/README.md
+-rw-r--r--   0        0        0      386 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/test-hatch-static/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/test-monorepo/README.md
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/test-monorepo/core/core.py
+-rw-r--r--   0        0        0      179 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/test-monorepo/core/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/test-monorepo/package_a/alice.py
+-rw-r--r--   0        0        0      231 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/test-monorepo/package_b/bob.py
+-rw-r--r--   0        0        0      231 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
+-rw-r--r--   0        0        0      237 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/test-monorepo/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/test-plugin-pdm/hello.py
+-rw-r--r--   0        0        0      312 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-03-29 07:35:39.150348 pdm-2.5.0b0/tests/fixtures/projects/test-plugin/hello.py
+-rw-r--r--   0        0        0      168 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/fixtures/projects/test-plugin/setup.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/fixtures/projects/test-removal/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/fixtures/projects/test-removal/bar.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/fixtures/projects/test-removal/foo.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/fixtures/projects/test-removal/subdir/__init__.py
+-rw-r--r--   0        0        0       10 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/fixtures/projects/test-setuptools/AUTHORS
+-rw-r--r--   0        0        0       12 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/fixtures/projects/test-setuptools/README.md
+-rw-r--r--   0        0        0       22 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/fixtures/projects/test-setuptools/mymodule.py
+-rw-r--r--   0        0        0      398 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/fixtures/projects/test-setuptools/setup.cfg
+-rw-r--r--   0        0        0      308 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/fixtures/projects/test-setuptools/setup.py
+-rw-r--r--   0        0        0     1525 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/fixtures/pypi.json
+-rw-r--r--   0        0        0     1329 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/fixtures/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/fixtures/requirements-include.txt
+-rw-r--r--   0        0        0      502 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/fixtures/requirements.txt
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/models/__init__.py
+-rw-r--r--   0        0        0     3820 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/models/test_backends.py
+-rw-r--r--   0        0        0    12991 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/models/test_candidates.py
+-rw-r--r--   0        0        0     1971 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/models/test_marker.py
+-rw-r--r--   0        0        0     2679 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/models/test_requirements.py
+-rw-r--r--   0        0        0     2526 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/models/test_setup_parsing.py
+-rw-r--r--   0        0        0     3418 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/models/test_specifiers.py
+-rw-r--r--   0        0        0     2703 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/models/test_versions.py
+-rw-r--r--   0        0        0        0 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/resolver/__init__.py
+-rw-r--r--   0        0        0    11567 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/resolver/test_resolve.py
+-rw-r--r--   0        0        0     7187 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/test_formats.py
+-rw-r--r--   0        0        0     7240 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/test_installer.py
+-rw-r--r--   0        0        0     1862 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/test_integration.py
+-rw-r--r--   0        0        0     2859 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/test_plugin.py
+-rw-r--r--   0        0        0    11182 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/test_project.py
+-rw-r--r--   0        0        0     1109 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/test_signals.py
+-rw-r--r--   0        0        0     4364 2023-03-29 07:35:39.154348 pdm-2.5.0b0/tests/test_utils.py
+-rw-r--r--   0        0        0     9912 1970-01-01 00:00:00.000000 pdm-2.5.0b0/PKG-INFO
```

### Comparing `pdm-2.5.0/CHANGELOG.md` & `pdm-2.5.0b0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Release v2.5.0 (2023-04-09)
----------------------------
-
-### Features & Improvements
-
-- When `resolution.respect-source-order` is enabled, sources are lazily evaluated. This means that if a match is found on the first source, the remaining sources will not be requested. [#1509](https://github.com/pdm-project/pdm/issues/1509)
-- New option `--venv <venv>` to run a command in the virtual environment with the given name. [#1705](https://github.com/pdm-project/pdm/issues/1705)
-- Allow to prefer binary distributions when locking and installing packages, via `PDM_PREFER_BINARY` environment variable. [#1817](https://github.com/pdm-project/pdm/issues/1817)
-
-### Bug Fixes
-
-- Do not validate selected groups against the locked grouped when running `pdm lock`. [#1796](https://github.com/pdm-project/pdm/issues/1796)
-- Avoid duplicate .pdm-python in .gitignore. [#1800](https://github.com/pdm-project/pdm/issues/1800)
-- Fix a backwards compatibility issue by adding back the `environment.is_global` property. [#1814](https://github.com/pdm-project/pdm/issues/1814)
-- Fix a resolution conflict when a relative path requirement resolves to the same path as another file requirement with absolute path. [#1822](https://github.com/pdm-project/pdm/issues/1822)
-- Fix an error when running `pdm init -p <dir>` if the target directory is not created yet. [#1822](https://github.com/pdm-project/pdm/issues/1822)
-
-
 Release v2.5.0b0 (2023-03-29)
 -----------------------------
 
 ### Breaking Changes
 
 - Switch the default build backend to `pdm-backend`. [#1684](https://github.com/pdm-project/pdm/issues/1684)
 - Only lock selected groups into the lockfile. Modify other commands to honor the groups included in the lockfile. [#1704](https://github.com/pdm-project/pdm/issues/1704)
```

### Comparing `pdm-2.5.0/LICENSE` & `pdm-2.5.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/README.md` & `pdm-2.5.0b0/README.md`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/pyproject.toml` & `pdm-2.5.0b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "certifi",
     "packaging>=20.9,!=22.0",
     "platformdirs",
     "rich>=12.3.0",
     "virtualenv>=20",
     "pyproject-hooks",
     "requests-toolbelt",
-    "unearth>=0.9.0",
+    "unearth>=0.8",
     "findpython>=0.2.2",
     "tomlkit>=0.11.1,<1",
     "shellingham>=1.3.2",
     "python-dotenv>=0.15",
     "resolvelib>=1.0.1",
     "installer<0.8,>=0.7",
     "cachecontrol[filecache]>=0.12.11",
@@ -38,15 +38,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "2.5.0"
+version = "2.5.0b0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://pdm.fming.dev"
 Repository = "https://github.com/pdm-project/pdm"
@@ -142,15 +142,14 @@
     "F",
     "PGH",
     "RUF",
     "W",
     "YTT",
 ]
 extend-ignore = [
-    "B018",
     "B019",
 ]
 src = [
     "src",
 ]
 extend-exclude = [
     "tests/fixtures",
```

### Comparing `pdm-2.5.0/src/pdm/_types.py` & `pdm-2.5.0b0/src/pdm/_types.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/builders/base.py` & `pdm-2.5.0b0/src/pdm/builders/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/builders/editable.py` & `pdm-2.5.0b0/src/pdm/builders/editable.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/builders/sdist.py` & `pdm-2.5.0b0/src/pdm/builders/sdist.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/builders/wheel.py` & `pdm-2.5.0b0/src/pdm/builders/wheel.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/cli/actions.py` & `pdm-2.5.0b0/src/pdm/cli/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,14 @@
     fail_fast: bool = False,
     hooks: HookManager | None = None,
 ) -> None:
     """Synchronize project"""
     hooks = hooks or HookManager(project)
     if requirements is None:
         requirements = []
-        selection.validate()
         for group in selection:
             requirements.extend(project.get_dependencies(group).values())
     candidates = resolve_candidates_from_lockfile(project, requirements)
     if tracked_names and dry_run:
         candidates = {name: c for name, c in candidates.items() if name in tracked_names}
     synchronizer = project.core.synchronizer_class(
         candidates,
@@ -236,16 +235,16 @@
     hooks = hooks or HookManager(project)
     check_project_file(project)
     if editables and no_editable:
         raise PdmUsageError("Cannot use --no-editable with editable packages given.")
     group = selection.one()
     tracked_names: set[str] = set()
     requirements: dict[str, Requirement] = {}
-    lock_groups = [] if project.lockfile.empty() else project.lockfile.groups
-    if lock_groups is not None and group not in lock_groups:
+    lock_groups = project.lockfile.groups
+    if lock_groups and group not in lock_groups:
         project.core.ui.echo(f"Adding group [success]{group}[/] to lockfile", err=True, style="info")
         lock_groups.append(group)
     if group == "default" or not selection.dev and group not in project.pyproject.settings.get("dev-dependencies", {}):
         if editables:
             raise PdmUsageError("Cannot add editables to the default or optional dependency group")
     for r in [parse_requirement(line, True) for line in editables] + [parse_requirement(line) for line in packages]:
         if project.name and normalize_name(project.name) == r.key and not r.extras:
@@ -340,15 +339,14 @@
         raise PdmUsageError("packages argument can't be used together with multiple -G or " "--no-default or --top.")
     all_dependencies = project.all_dependencies
     updated_deps: dict[str, dict[str, Requirement]] = defaultdict(dict)
     locked_groups = project.lockfile.groups
     if not packages:
         if prerelease:
             raise PdmUsageError("--prerelease must be used with packages given")
-        selection.validate()
         for group in selection:
             updated_deps[group] = all_dependencies[group]
     else:
         group = selection.one()
         if locked_groups and group not in locked_groups:
             raise ProjectError(f"Requested group not in lockfile: {group}")
         dependencies = all_dependencies[group]
@@ -566,40 +564,34 @@
 def do_use(
     project: Project,
     python: str = "",
     first: bool = False,
     ignore_remembered: bool = False,
     ignore_requires_python: bool = False,
     save: bool = True,
-    venv: str | None = None,
     hooks: HookManager | None = None,
 ) -> PythonInfo:
     """Use the specified python version and save in project config.
     The python can be a version string or interpreter path.
     """
-    from pdm.cli.commands.venv.utils import get_venv_python, get_venv_with_name
+    hooks = hooks or HookManager(project)
+
+    if python:
+        python = python.strip()
 
     def version_matcher(py_version: PythonInfo) -> bool:
         return py_version.valid and (
             ignore_requires_python or project.python_requires.contains(str(py_version.version), True)
         )
 
-    hooks = hooks or HookManager(project)
-
-    selected_python: PythonInfo | None = None
-    if venv:
-        venv_path = get_venv_with_name(project, venv)
-        selected_python = PythonInfo.from_path(get_venv_python(venv_path))
-
     if not project.cache_dir.exists():
         project.cache_dir.mkdir(parents=True)
     use_cache: JSONFileCache[str, str] = JSONFileCache(project.cache_dir / "use_cache.json")
-    if python:
-        python = python.strip()
-    if selected_python is None and python and not ignore_remembered:
+    selected_python: PythonInfo | None = None
+    if python and not ignore_remembered:
         if python in use_cache:
             path = use_cache.get(python)
             cached_python = PythonInfo.from_path(path)
             if not cached_python.valid:
                 project.core.ui.echo(
                     f"The last selection is corrupted. {path!r}",
                     style="error",
@@ -816,33 +808,33 @@
         state = json.loads(cache_file.read_text())
     current_time = datetime.datetime.utcnow().timestamp()
     if state.get("last-check") and current_time - state["last-check"] < 60 * 60 * 24 * 7:
         return cast(str, state["latest-version"])
     try:
         latest_version = get_latest_pdm_version_from_pypi(project)
     except Exception as e:
-        warnings.warn(f"Failed to get latest version: {e}", RuntimeWarning, stacklevel=1)
+        warnings.warn(f"Failed to get latest version: {e}", RuntimeWarning)
         latest_version = None
     if latest_version is None:
         return None
     state.update({"latest-version": latest_version, "last-check": current_time})
     with contextlib.suppress(OSError):
         cache_file.write_text(json.dumps(state))
     return latest_version
 
 
 def check_update(project: Project) -> None:
     """Check if there is a new version of PDM available"""
-    from packaging.version import Version
+    from packaging.version import parse as parse_version
 
     this_version = project.core.version
     latest_version = get_latest_version(project)
-    if latest_version is None or Version(this_version) >= Version(latest_version):
+    if latest_version is None or parse_version(this_version) >= parse_version(latest_version):
         return
-    install_command = "pdm self update" + (" --pre" if Version(latest_version).is_prerelease else "")
+    install_command = "pdm self update"
     disable_command = "pdm config check_update false"
 
     message = [
         f"\nPDM [primary]{this_version}[/]",
         f" is installed, while [primary]{latest_version}[/]",
         " is available.\n",
         f"Please run [req]`{install_command}`[/]",
```

### Comparing `pdm-2.5.0/src/pdm/cli/commands/add.py` & `pdm-2.5.0b0/src/pdm/cli/commands/add.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     lockfile_option,
     packages_group,
     prerelease_option,
     save_strategy_group,
     skip_option,
     unconstrained_option,
     update_strategy_group,
-    venv_option,
 )
 from pdm.exceptions import PdmUsageError
 from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Add package(s) to pyproject.toml and install them"""
@@ -29,15 +28,14 @@
         save_strategy_group,
         update_strategy_group,
         prerelease_option,
         unconstrained_option,
         packages_group,
         install_group,
         dry_run_option,
-        venv_option,
         skip_option,
     ]
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "-d",
             "--dev",
```

### Comparing `pdm-2.5.0/src/pdm/cli/commands/base.py` & `pdm-2.5.0b0/src/pdm/cli/commands/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,16 +41,16 @@
             description=help_text,
             help=help_text,
             formatter_class=PdmFormatter,
             **kwargs,
         )
         command = cls(parser)
         command.name = name
-        # Store the command instance in the parsed args. See pdm/core.py for more details
-        parser.set_defaults(command=command)
+        # A special attribute to store the command instance. See pdm/core.py for more details
+        parser.set_defaults(__command__=command)
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         """Manipulate the argument parser to add more arguments"""
         pass
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         """The command handler function.
```

### Comparing `pdm-2.5.0/src/pdm/cli/commands/build.py` & `pdm-2.5.0b0/src/pdm/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/cli/commands/cache.py` & `pdm-2.5.0b0/src/pdm/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/cli/commands/completion.py` & `pdm-2.5.0b0/src/pdm/cli/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/cli/commands/config.py` & `pdm-2.5.0b0/src/pdm/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/cli/commands/export.py` & `pdm-2.5.0b0/src/pdm/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/cli/commands/fix/__init__.py` & `pdm-2.5.0b0/src/pdm/cli/commands/fix/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/cli/commands/fix/fixers.py` & `pdm-2.5.0b0/src/pdm/cli/commands/fix/fixers.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,17 +44,16 @@
         )
 
     def _fix_gitignore(self) -> None:
         gitignore = self.project.root.joinpath(".gitignore")
         if not gitignore.exists():
             return
         content = gitignore.read_text("utf8")
-        if ".pdm-python" not in content:
-            content = re.sub(r"^\.pdm\.toml$", ".pdm-python", content, flags=re.M)
-            gitignore.write_text(content, "utf8")
+        content = re.sub(r"^\.pdm\.toml$", ".pdm-python", content, flags=re.M)
+        gitignore.write_text(content, "utf8")
 
     def fix(self) -> None:
         old_file = self.project.root.joinpath(".pdm.toml")
         config = Config(old_file).self_data
         if not self.project.root.joinpath(".pdm-python").exists() and config.get("python.path"):
             self.log("Creating .pdm-python...", verbosity=Verbosity.DETAIL)
             self.project.root.joinpath(".pdm-python").write_text(config["python.path"])
```

### Comparing `pdm-2.5.0/src/pdm/cli/commands/import_cmd.py` & `pdm-2.5.0b0/src/pdm/cli/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/cli/commands/info.py` & `pdm-2.5.0b0/src/pdm/cli/commands/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import argparse
 import json
 
 from pdm.cli.commands.base import BaseCommand
-from pdm.cli.options import ArgumentGroup, venv_option
+from pdm.cli.options import ArgumentGroup
 from pdm.cli.utils import check_project_file
 from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Show the project information"""
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
-        venv_option.add_to_parser(parser)
         group = ArgumentGroup("fields", is_mutually_exclusive=True)
         group.add_argument("--python", action="store_true", help="Show the interpreter path")
         group.add_argument(
             "--where",
             dest="where",
             action="store_true",
             help="Show the project root path",
         )
         group.add_argument("--packages", action="store_true", help="Show the local packages root")
         group.add_argument("--env", action="store_true", help="Show PEP 508 environment markers")
         group.add_to_parser(parser)
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         check_project_file(project)
-        interpreter = project.environment.interpreter
+        interpreter = project.python
         packages_path = ""
         if project.environment.is_local:
             packages_path = project.environment.packages_path  # type: ignore[attr-defined]
         if options.python:
             project.core.ui.echo(str(interpreter.executable))
         elif options.where:
             project.core.ui.echo(str(project.root))
```

### Comparing `pdm-2.5.0/src/pdm/cli/commands/init.py` & `pdm-2.5.0b0/src/pdm/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/cli/commands/install.py` & `pdm-2.5.0b0/src/pdm/cli/commands/install.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,30 +2,28 @@
 import sys
 
 from pdm import termui
 from pdm.cli import actions
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.filters import GroupSelection
 from pdm.cli.hooks import HookManager
-from pdm.cli.options import dry_run_option, groups_group, install_group, lockfile_option, skip_option, venv_option
+from pdm.cli.options import (
+    dry_run_option,
+    groups_group,
+    install_group,
+    lockfile_option,
+    skip_option,
+)
 from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Install dependencies from lock file"""
 
-    arguments = [
-        *BaseCommand.arguments,
-        groups_group,
-        install_group,
-        dry_run_option,
-        lockfile_option,
-        skip_option,
-        venv_option,
-    ]
+    arguments = [*BaseCommand.arguments, groups_group, install_group, dry_run_option, lockfile_option, skip_option]
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "--no-lock",
             dest="lock",
             action="store_false",
             default=True,
```

### Comparing `pdm-2.5.0/src/pdm/cli/commands/list.py` & `pdm-2.5.0b0/src/pdm/cli/commands/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import io
 import json
 from collections import defaultdict
 from typing import Iterable, Mapping, Sequence
 
 from pdm.cli import actions
 from pdm.cli.commands.base import BaseCommand
-from pdm.cli.options import venv_option
 from pdm.cli.utils import (
     DirectedGraph,
     Package,
     build_dependency_graph,
     check_project_file,
     get_dist_location,
     show_dependency_graph,
@@ -29,15 +28,14 @@
 
 class Command(BaseCommand):
     """List packages installed in the current working set"""
 
     DEFAULT_FIELDS = "name,version,location"
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
-        venv_option.add_to_parser(parser)
         graph = parser.add_mutually_exclusive_group()
 
         parser.add_argument(
             "--freeze",
             action="store_true",
             help="Show the installed dependencies in pip's requirements.txt format",
         )
```

### Comparing `pdm-2.5.0/src/pdm/cli/commands/lock.py` & `pdm-2.5.0b0/src/pdm/cli/commands/lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/cli/commands/publish/__init__.py` & `pdm-2.5.0b0/src/pdm/cli/commands/publish/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/cli/commands/publish/package.py` & `pdm-2.5.0b0/src/pdm/cli/commands/publish/package.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/cli/commands/publish/repository.py` & `pdm-2.5.0b0/src/pdm/cli/commands/publish/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         project: Project,
         url: str,
         username: str | None,
         password: str | None,
         ca_certs: str | None,
     ) -> None:
         self.url = url
-        self.session = project.environment._build_session([])
+        self.session = project.environment._build_session([], [])
         if ca_certs is not None:
             self.session.set_ca_certificates(pathlib.Path(ca_certs))
         self._credentials_to_save: tuple[str, str, str] | None = None
         username, password = self._ensure_credentials(username, password)
         self.session.auth = (username, password)
         weakref.finalize(self, self.session.close)
         self.ui = project.core.ui
```

### Comparing `pdm-2.5.0/src/pdm/cli/commands/remove.py` & `pdm-2.5.0b0/src/pdm/cli/commands/remove.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import argparse
 
 from pdm.cli import actions
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.filters import GroupSelection
 from pdm.cli.hooks import HookManager
-from pdm.cli.options import dry_run_option, install_group, lockfile_option, skip_option, venv_option
+from pdm.cli.options import dry_run_option, install_group, lockfile_option, skip_option
 from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Remove packages from pyproject.toml"""
 
-    arguments = [*BaseCommand.arguments, install_group, dry_run_option, lockfile_option, skip_option, venv_option]
+    arguments = [*BaseCommand.arguments, install_group, dry_run_option, lockfile_option, skip_option]
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "-d",
             "--dev",
             default=False,
             action="store_true",
```

### Comparing `pdm-2.5.0/src/pdm/cli/commands/run.py` & `pdm-2.5.0b0/src/pdm/cli/commands/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import sys
 from types import FrameType
 from typing import Any, Callable, Iterator, Mapping, NamedTuple, Sequence, cast
 
 from pdm import termui
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.hooks import HookManager
-from pdm.cli.options import skip_option, venv_option
+from pdm.cli.options import skip_option
 from pdm.cli.utils import check_project_file, get_pep582_path
 from pdm.compat import TypedDict
 from pdm.exceptions import PdmUsageError
 from pdm.project import Project
 from pdm.signals import pdm_signals
 from pdm.utils import is_path_relative_to
 
@@ -159,15 +159,15 @@
             assert isinstance(args, str)
             expanded_args: str | Sequence[str] = os.path.expandvars(args)
         else:
             assert isinstance(args, Sequence)
             command, *args = args
             if command.endswith(".py"):
                 args = [command, *args]
-                command = str(project.environment.interpreter.executable)
+                command = str(project.python.executable)
             expanded_command = project_env.which(command)
             if not expanded_command:
                 raise PdmUsageError(f"Command [success]'{command}'[/] is not found in your PATH.")
             expanded_command = os.path.expanduser(os.path.expandvars(expanded_command))
             real_command = os.path.realpath(expanded_command)
             expanded_args = [os.path.expandvars(arg) for arg in [expanded_command, *args]]
             if (
@@ -301,54 +301,54 @@
         self.project.core.ui.display_columns(result, columns)
 
 
 class Command(BaseCommand):
     """Run commands or scripts with local packages loaded"""
 
     runner_cls: type[TaskRunner] = TaskRunner
-    arguments = [*BaseCommand.arguments, skip_option, venv_option]
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
+        skip_option.add_to_parser(parser)
         parser.add_argument(
             "-l",
             "--list",
             action="store_true",
             help="Show all available scripts defined in pyproject.toml",
         )
         parser.add_argument(
             "-s",
             "--site-packages",
             action="store_true",
             help="Load site-packages from the selected interpreter",
         )
-        parser.add_argument("script", nargs="?", help="The command to run")
+        parser.add_argument("command", nargs="?", help="The command to run")
         parser.add_argument(
             "args",
             nargs=argparse.REMAINDER,
             help="Arguments that will be passed to the command",
         )
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         check_project_file(project)
         hooks = HookManager(project, options.skip)
         runner = self.runner_cls(project, hooks=hooks)
         if options.list:
             return runner.show_list()
         if options.site_packages:
             runner.global_options.update({"site_packages": options.site_packages})
-        if not options.script:
+        if not options.command:
             project.core.ui.echo(
                 "No command is given, default to the Python REPL.",
                 style="warning",
                 err=True,
             )
-            options.script = "python"
-        hooks.try_emit("pre_run", script=options.script, args=options.args)
-        exit_code = runner.run(options.script, options.args)
-        hooks.try_emit("post_run", script=options.script, args=options.args)
+            options.command = "python"
+        hooks.try_emit("pre_run", script=options.command, args=options.args)
+        exit_code = runner.run(options.command, options.args)
+        hooks.try_emit("post_run", script=options.command, args=options.args)
         sys.exit(exit_code)
 
 
 def run_script_if_present(script_name: str) -> Callable:
     """Helper to create a signal handler to run specific script"""
 
     def handler(sender: Project, hooks: HookManager, **kwargs: Any) -> None:
```

### Comparing `pdm-2.5.0/src/pdm/cli/commands/search.py` & `pdm-2.5.0b0/src/pdm/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/cli/commands/self_cmd.py` & `pdm-2.5.0b0/src/pdm/cli/commands/self_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/cli/commands/show.py` & `pdm-2.5.0b0/src/pdm/cli/commands/show.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import argparse
 
 from packaging.version import Version
 
 from pdm.cli.commands.base import BaseCommand
-from pdm.cli.options import venv_option
 from pdm.exceptions import PdmUsageError
 from pdm.models.candidates import Candidate
 from pdm.models.project_info import ProjectInfo
 from pdm.models.requirements import parse_requirement
 from pdm.project import Project
 from pdm.utils import normalize_name
 
@@ -19,15 +18,14 @@
 
 class Command(BaseCommand):
     """Show the package information"""
 
     metadata_keys = ["name", "version", "summary", "license", "platform", "keywords"]
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
-        venv_option.add_to_parser(parser)
         parser.add_argument(
             "package",
             type=normalize_name,
             nargs=argparse.OPTIONAL,
             help="Specify the package name, or show this package if not given",
         )
         for option in self.metadata_keys:
```

### Comparing `pdm-2.5.0/src/pdm/cli/commands/sync.py` & `pdm-2.5.0b0/src/pdm/cli/commands/sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from pdm.cli.options import (
     clean_group,
     dry_run_option,
     groups_group,
     install_group,
     lockfile_option,
     skip_option,
-    venv_option,
 )
 from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Synchronize the current working set with lock file"""
 
@@ -23,15 +22,14 @@
         *BaseCommand.arguments,
         groups_group,
         dry_run_option,
         lockfile_option,
         skip_option,
         clean_group,
         install_group,
-        venv_option,
     ]
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "-r",
             "--reinstall",
             action="store_true",
```

### Comparing `pdm-2.5.0/src/pdm/cli/commands/update.py` & `pdm-2.5.0b0/src/pdm/cli/commands/update.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     install_group,
     lockfile_option,
     prerelease_option,
     save_strategy_group,
     skip_option,
     unconstrained_option,
     update_strategy_group,
-    venv_option,
 )
 from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Update package(s) in pyproject.toml"""
 
@@ -27,15 +26,14 @@
         install_group,
         lockfile_option,
         save_strategy_group,
         update_strategy_group,
         prerelease_option,
         unconstrained_option,
         skip_option,
-        venv_option,
     ]
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "-t",
             "--top",
             action="store_true",
```

### Comparing `pdm-2.5.0/src/pdm/cli/commands/use.py` & `pdm-2.5.0b0/src/pdm/cli/commands/use.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,19 +20,17 @@
         )
         parser.add_argument(
             "-i",
             "--ignore-remembered",
             action="store_true",
             help="Ignore the remembered selection",
         )
-        parser.add_argument("--venv", help="Use the interpreter in the virtual environment with the given name")
         parser.add_argument("python", nargs="?", help="Specify the Python version or path", default="")
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         actions.do_use(
             project,
             python=options.python,
             first=options.first,
             ignore_remembered=options.ignore_remembered,
-            venv=options.venv,
             hooks=HookManager(project, options.skip),
         )
```

### Comparing `pdm-2.5.0/src/pdm/cli/commands/venv/__init__.py` & `pdm-2.5.0b0/src/pdm/cli/commands/venv/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import argparse
 from pathlib import Path
-from pdm.cli.commands.venv.utils import get_venv_with_name, iter_venvs, get_venv_python
+from pdm.cli.commands.venv.utils import iter_venvs, get_venv_python
 
 from pdm.exceptions import PdmUsageError
 from pdm.project import Project
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.commands.venv.activate import ActivateCommand
 from pdm.cli.commands.venv.create import CreateCommand
 from pdm.cli.commands.venv.list import ListCommand
@@ -28,18 +28,29 @@
         CreateCommand.register_to(subparser, "create")
         ListCommand.register_to(subparser, "list")
         RemoveCommand.register_to(subparser, "remove")
         ActivateCommand.register_to(subparser, "activate")
         PurgeCommand.register_to(subparser, "purge")
         self.parser = parser
 
+    def _get_venv_with_name(self, project: Project, name: str) -> Path:
+        venv = next((venv for key, venv in iter_venvs(project) if key == name), None)
+        if not venv:
+            project.core.ui.echo(
+                f"No virtualenv with key [success]{name}[/] is found",
+                style="warning",
+                err=True,
+            )
+            raise SystemExit(1)
+        return venv
+
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         if options.path and options.python:
             raise PdmUsageError("--path and --python are mutually exclusive")
         if options.path:
-            venv = get_venv_with_name(project, options.path)
+            venv = self._get_venv_with_name(project, options.path)
             project.core.ui.echo(str(venv))
         elif options.python:
-            venv = get_venv_with_name(project, options.python)
+            venv = self._get_venv_with_name(project, options.python)
             project.core.ui.echo(str(get_venv_python(venv)))
         else:
             self.parser.print_help()
```

### Comparing `pdm-2.5.0/src/pdm/cli/commands/venv/activate.py` & `pdm-2.5.0b0/src/pdm/cli/commands/venv/activate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import shlex
 from pathlib import Path
 
 import shellingham
 
 from pdm.cli.commands.base import BaseCommand
-from pdm.cli.commands.venv.utils import BIN_DIR, iter_venvs, get_venv_with_name
+from pdm.cli.commands.venv.utils import BIN_DIR, iter_venvs
 from pdm.cli.options import verbose_option
 from pdm.project import Project
 from pdm.utils import get_venv_like_prefix
 
 
 class ActivateCommand(BaseCommand):
     """Activate the virtualenv with the given name"""
@@ -17,35 +17,41 @@
     arguments = [verbose_option]
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument("env", nargs="?", help="The key of the virtualenv")
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         if options.env:
-            venv = get_venv_with_name(project, options.env)
+            venv = next((venv for key, venv in iter_venvs(project) if key == options.env), None)
+            if not venv:
+                project.core.ui.echo(
+                    f"No virtualenv with key [success]{options.env}[/] is found",
+                    style="warning",
+                    err=True,
+                )
+                raise SystemExit(1)
         else:
             # Use what is saved in .pdm-python
             interpreter = project._saved_python
             if not interpreter:
                 project.core.ui.echo(
                     "The project doesn't have a saved python.path. Run [success]pdm use[/] to pick one.",
                     style="warning",
                     err=True,
                 )
                 raise SystemExit(1)
-            venv_like = get_venv_like_prefix(interpreter)
-            if venv_like is None:
+            venv = get_venv_like_prefix(interpreter)
+            if venv is None:
                 project.core.ui.echo(
                     f"Can't activate a non-venv Python [success]{interpreter}[/], "
                     "you can specify one with [success]pdm venv activate <env_name>[/]",
                     style="warning",
                     err=True,
                 )
                 raise SystemExit(1)
-            venv = venv_like
         project.core.ui.echo(self.get_activate_command(venv))
 
     def get_activate_command(self, venv: Path) -> str:  # pragma: no cover
         shell, _ = shellingham.detect_shell()
         if shell == "fish":
             command, filename = "source", "activate.fish"
         elif shell == "csh":
```

### Comparing `pdm-2.5.0/src/pdm/cli/commands/venv/backends.py` & `pdm-2.5.0b0/src/pdm/cli/commands/venv/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/cli/commands/venv/create.py` & `pdm-2.5.0b0/src/pdm/cli/commands/venv/create.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/cli/commands/venv/list.py` & `pdm-2.5.0b0/src/pdm/cli/commands/venv/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/cli/commands/venv/purge.py` & `pdm-2.5.0b0/src/pdm/cli/commands/venv/purge.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/cli/commands/venv/remove.py` & `pdm-2.5.0b0/src/pdm/cli/commands/venv/remove.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import shutil
 from pathlib import Path
 
 from pdm import termui
 from pdm.cli.commands.base import BaseCommand
-from pdm.cli.commands.venv.utils import get_venv_with_name, iter_venvs
+from pdm.cli.commands.venv.utils import iter_venvs
 from pdm.cli.options import verbose_option
 from pdm.project import Project
 
 
 class RemoveCommand(BaseCommand):
     """Remove the virtualenv with the given name"""
 
@@ -21,14 +21,23 @@
             action="store_true",
             help="Answer yes on the following question",
         )
         parser.add_argument("env", help="The key of the virtualenv")
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         project.core.ui.echo("Virtualenvs created with this project:")
-        venv = get_venv_with_name(project, options.env)
-        if options.yes or termui.confirm(f"[warning]Will remove: [success]{venv}[/], continue?", default=True):
-            shutil.rmtree(venv)
-            saved_python = project._saved_python
-            if saved_python and Path(saved_python).parent.parent == venv:
-                project._saved_python = None
-            project.core.ui.echo("Removed successfully!")
+        for ident, venv in iter_venvs(project):
+            if ident == options.env:
+                if options.yes or termui.confirm(f"[warning]Will remove: [success]{venv}[/], continue?", default=True):
+                    shutil.rmtree(venv)
+                    saved_python = project._saved_python
+                    if saved_python and Path(saved_python).parent.parent == venv:
+                        project._saved_python = None
+                    project.core.ui.echo("Removed successfully!")
+                break
+        else:
+            project.core.ui.echo(
+                f"No virtualenv with key [success]{options.env}[/] is found",
+                style="warning",
+                err=True,
+            )
+            raise SystemExit(1)
```

### Comparing `pdm-2.5.0/src/pdm/cli/commands/venv/utils.py` & `pdm-2.5.0b0/src/pdm/cli/commands/venv/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import hashlib
 import sys
 from pathlib import Path
 from typing import Iterable, TypeVar
 from findpython import PythonVersion
 
 from findpython.providers import BaseProvider
-from pdm.exceptions import PdmUsageError
 
 from pdm.project import Project
 
 IS_WIN = sys.platform == "win32"
 BIN_DIR = "Scripts" if IS_WIN else "bin"
 
 
@@ -77,18 +76,7 @@
         return None
 
     def find_pythons(self) -> Iterable[PythonVersion]:
         for _, venv in iter_venvs(self.project):
             python = get_venv_python(venv)
             if python.exists():
                 yield PythonVersion(python, _interpreter=python, keep_symlink=True)
-
-
-def get_venv_with_name(project: Project, name: str) -> Path:
-    all_venvs = dict(iter_venvs(project))
-    try:
-        return all_venvs[name]
-    except KeyError:
-        raise PdmUsageError(
-            f"No virtualenv with key '{name}' is found, must be one of {list(all_venvs)}.\n"
-            "You can create one with 'pdm venv create'.",
-        )
```

### Comparing `pdm-2.5.0/src/pdm/cli/completions/pdm.bash` & `pdm-2.5.0b0/src/pdm/cli/completions/pdm.bash`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     # completing for an option
     if [[ ${cur} == --* ]] ; then
         opts="--config --help --ignore-python --pep582 --verbose --version"
 
         case "$com" in
 
             (add)
-            opts="--dev --dry-run --editable --fail-fast --global --group --help --lockfile --no-editable --no-isolation --no-self --no-sync --prerelease --project --save-compatible --save-exact --save-minimum --save-wildcard --skip --unconstrained --update-all --update-eager --update-reuse --venv --verbose"
+            opts="--dev --dry-run --editable --fail-fast --global --group --help --lockfile --no-editable --no-isolation --no-self --no-sync --prerelease --project --save-compatible --save-exact --save-minimum --save-wildcard --skip --unconstrained --update-all --update-eager --update-reuse --verbose"
             ;;
 
             (build)
             opts="--config-setting --dest --help --no-clean --no-isolation --no-sdist --no-wheel --project --skip --verbose"
             ;;
 
             (cache)
@@ -57,27 +57,27 @@
             ;;
 
             (import)
             opts="--dev --format --global --group --help --project --verbose"
             ;;
 
             (info)
-            opts="--env --global --help --packages --project --python --venv --verbose --where"
+            opts="--env --global --help --packages --project --python --verbose --where"
             ;;
 
             (init)
             opts="--backend --global --help --lib --non-interactive --project --python --skip --verbose"
             ;;
 
             (install)
-            opts="--check --dev --dry-run --fail-fast --global --group --help --lockfile --no-default --no-editable --no-isolation --no-lock --no-self --production --project --skip --venv --verbose"
+            opts="--check --dev --dry-run --fail-fast --global --group --help --lockfile --no-default --no-editable --no-isolation --no-lock --no-self --production --project --skip --verbose"
             ;;
 
             (list)
-            opts="--csv --exclude --fields --freeze --global --graph --help --include --json --markdown --project --resolve --reverse --sort --venv --verbose"
+            opts="--csv --exclude --fields --freeze --global --graph --help --include --json --markdown --project --resolve --reverse --sort --verbose"
             ;;
 
             (lock)
             opts="--check --dev --global --group --help --lockfile --no-default --no-isolation --production --project --refresh --skip --verbose"
             ;;
 
             (plugin)
@@ -85,43 +85,43 @@
             ;;
 
             (publish)
             opts="--ca-certs --comment --help --identity --no-build --password --project --repository --sign --skip --username --verbose"
             ;;
 
             (remove)
-            opts="--dev --dry-run --fail-fast --global --group --help --lockfile --no-editable --no-isolation --no-self --no-sync --project --skip --venv --verbose"
+            opts="--dev --dry-run --fail-fast --global --group --help --lockfile --no-editable --no-isolation --no-self --no-sync --project --skip --verbose"
             ;;
 
             (run)
-            opts="--global --help --list --project --site-packages --skip --venv --verbose"
+            opts="--global --help --list --project --site-packages --skip --verbose"
             ;;
 
             (search)
             opts="--help --verbose"
             ;;
 
             (self)
             opts="--help --verbose"
             ;;
 
             (show)
-            opts="--global --help --keywords --license --name --platform --project --summary --venv --verbose --version"
+            opts="--global --help --keywords --license --name --platform --project --summary --verbose --version"
             ;;
 
             (sync)
-            opts="--clean --dev --dry-run --fail-fast --global --group --help --lockfile --no-default --no-editable --no-isolation --no-self --only-keep --production --project --reinstall --skip --venv --verbose"
+            opts="--clean --dev --dry-run --fail-fast --global --group --help --lockfile --no-default --no-editable --no-isolation --no-self --only-keep --production --project --reinstall --skip --verbose"
             ;;
 
             (update)
-            opts="--dev --fail-fast --global --group --help --lockfile --no-default --no-editable --no-isolation --no-self --no-sync --outdated --prerelease --production --project --save-compatible --save-exact --save-minimum --save-wildcard --skip --top --unconstrained --update-all --update-eager --update-reuse --venv --verbose"
+            opts="--dev --fail-fast --global --group --help --lockfile --no-default --no-editable --no-isolation --no-self --no-sync --outdated --prerelease --production --project --save-compatible --save-exact --save-minimum --save-wildcard --skip --top --unconstrained --update-all --update-eager --update-reuse --verbose"
             ;;
 
             (use)
-            opts="--first --global --help --ignore-remembered --project --skip --venv --verbose"
+            opts="--first --global --help --ignore-remembered --project --skip --verbose"
             ;;
 
             (venv)
             opts="--help --path --python"
             ;;
 
         esac
```

### Comparing `pdm-2.5.0/src/pdm/cli/completions/pdm.fish` & `pdm-2.5.0b0/src/pdm/cli/completions/pdm.fish`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     end
     return 0
 end
 
 # global options
 complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l config -d 'Specify another config file path(env var: PDM_CONFIG_FILE)'
 complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l help -d 'show this help message and exit'
-complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l ignore-python -d 'Ignore the Python path saved in .pdm-python. [env var: PDM_IGNORE_SAVED_PYTHON]'
+complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l ignore-python -d 'Ignore the Python path saved in .pdm-python'
 complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l pep582 -d 'Print the command line to be eval\'d by the shell'
 complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l verbose -d '-v for detailed output and -vv for more detailed'
 complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l version -d 'Show version'
 
 # commands
 complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a add -d 'Add package(s) to pyproject.toml and install them'
 complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a build -d 'Build artifacts for distribution'
@@ -66,15 +66,14 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l save-minimum -d 'Save minimum version specifiers'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l save-wildcard -d 'Save wildcard version specifiers'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l unconstrained -d 'Ignore the version constraint of packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l update-all -d 'Update all dependencies and sub-dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l update-eager -d 'Try to update the packages and their dependencies recursively'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l update-reuse -d 'Reuse pinned versions already present in lock file if possible'
-complete -c pdm -A -n '__fish_seen_subcommand_from add' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l verbose -d '-v for detailed output and -vv for more detailed'
 
 # build
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l config-setting -d 'Pass options to the backend. options with a value must be specified after "=": "--config-setting=--opt(=value)" or "-C--opt(=value)"'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l dest -d 'Target directory to put artifacts'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l help -d 'show this help message and exit'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l no-clean -d 'Do not clean the target directory'
@@ -131,18 +130,17 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from import' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from import' -l verbose -d '-v for detailed output and -vv for more detailed'
 
 # info
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l env -d 'Show PEP 508 environment markers'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l help -d 'show this help message and exit'
-complete -c pdm -A -n '__fish_seen_subcommand_from info' -l packages -d 'Show the local packages root'
+complete -c pdm -A -n '__fish_seen_subcommand_from info' -l packages -d 'Show the packages root'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l python -d 'Show the interpreter path'
-complete -c pdm -A -n '__fish_seen_subcommand_from info' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l verbose -d '-v for detailed output and -vv for more detailed'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l where -d 'Show the project root path'
 
 # init
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l backend -d 'Specify the build backend'
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l help -d 'show this help message and exit'
@@ -166,15 +164,14 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l no-editable -d 'Install non-editable versions for all packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l no-isolation -d 'Do not isolate the build in a clean environment'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l no-lock -d 'Don\'t do lock if the lock file is not found or outdated'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l no-self -d 'Don\'t install the project itself'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l production -d 'Unselect dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
-complete -c pdm -A -n '__fish_seen_subcommand_from install' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l verbose -d '-v for detailed output and -vv for more detailed'
 
 # list
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l csv -d 'Output dependencies in CSV document format'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l exclude -d 'Exclude dependency groups from the output'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l fields -d 'Select information to output as a comma separated string. For example: name,version,homepage,licenses,groups.'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l freeze -d 'Show the installed dependencies in pip\'s requirements.txt format'
@@ -184,15 +181,14 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l include -d 'Dependency groups to include in the output. By default all are included'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l json -d 'Output dependencies in JSON document format'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l markdown -d 'Output dependencies and legal notices in markdown document format - best effort basis'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l resolve -d 'Resolve all requirements to output licenses (instead of just showing those currently installed)'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l reverse -d 'Reverse the dependency graph'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l sort -d 'Sort the output using a given field name. If nothing is set, no sort is applied. Multiple fields can be combined with \',\'.'
-complete -c pdm -A -n '__fish_seen_subcommand_from list' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l verbose -d '-v for detailed output and -vv for more detailed'
 
 # lock
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l check -d 'Check if the lock file is up to date and quit'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l dev -d 'Select dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species.'
@@ -234,25 +230,23 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l no-editable -d 'Install non-editable versions for all packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l no-isolation -d 'Do not isolate the build in a clean environment'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l no-self -d 'Don\'t install the project itself'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l no-sync -d 'Only write pyproject.toml and do not uninstall packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
-complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l verbose -d '-v for detailed output and -vv for more detailed'
 
 # run
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l help -d 'show this help message and exit'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l list -d 'Show all available scripts defined in pyproject.toml'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l site-packages -d 'Load site-packages from the selected interpreter'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
-complete -c pdm -A -n '__fish_seen_subcommand_from run' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l verbose -d '-v for detailed output and -vv for more detailed'
 
 # search
 complete -c pdm -A -n '__fish_seen_subcommand_from search' -l help -d 'show this help message and exit'
 complete -c pdm -A -n '__fish_seen_subcommand_from search' -l verbose -d '-v for detailed output and -vv for more detailed'
 
 # self
@@ -264,15 +258,14 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l help -d 'show this help message and exit'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l keywords -d 'Show keywords'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l license -d 'Show license'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l name -d 'Show name'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l platform -d 'Show platform'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l summary -d 'Show summary'
-complete -c pdm -A -n '__fish_seen_subcommand_from show' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l verbose -d '-v for detailed output and -vv for more detailed'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l version -d 'Show version'
 
 # sync
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l clean -d 'clean packages not in the lockfile'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l dev -d 'Select dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l dry-run -d 'Show the difference only and don\'t perform any action'
@@ -286,15 +279,14 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l no-isolation -d 'Do not isolate the build in a clean environment'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l no-self -d 'Don\'t install the project itself'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l only-keep -d 'only keep the selected packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l production -d 'Unselect dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l reinstall -d 'Force reinstall existing dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
-complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l verbose -d '-v for detailed output and -vv for more detailed'
 
 # update
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l dev -d 'Select dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l fail-fast -d 'Abort on first installation error'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species.'
@@ -315,24 +307,22 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l save-wildcard -d 'Save wildcard version specifiers'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l top -d 'Only update those listed in pyproject.toml'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l unconstrained -d 'Ignore the version constraint of packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l update-all -d 'Update all dependencies and sub-dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l update-eager -d 'Try to update the packages and their dependencies recursively'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l update-reuse -d 'Reuse pinned versions already present in lock file if possible'
-complete -c pdm -A -n '__fish_seen_subcommand_from update' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l verbose -d '-v for detailed output and -vv for more detailed'
 
 # use
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l first -d 'Select the first matched interpreter'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l help -d 'show this help message and exit'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l ignore-remembered -d 'Ignore the remembered selection'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
-complete -c pdm -A -n '__fish_seen_subcommand_from use' -l venv -d 'Use the interpreter in the virtual environment with the given name'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l verbose -d '-v for detailed output and -vv for more detailed'
 
 # venv
 complete -c pdm -A -n '__fish_seen_subcommand_from venv' -l help -d 'show this help message and exit'
 complete -c pdm -A -n '__fish_seen_subcommand_from venv' -l path -d 'Show the path to the given virtualenv'
 complete -c pdm -A -n '__fish_seen_subcommand_from venv' -l python -d 'Show the python interpreter path for the given virtualenv'
```

### Comparing `pdm-2.5.0/src/pdm/cli/completions/pdm.ps1` & `pdm-2.5.0b0/src/pdm/cli/completions/pdm.ps1`

 * *Files 3% similar despite different names*

```diff
@@ -196,30 +196,28 @@
         [string[]]$commands = $words.Where( { $_ -notlike "-*" })
         $command = $commands[0]
         $completer = [Completer]::new()
         $completer.AddOpts(([Option]::new(("-h", "--help", "-v", "--verbose"))))
         $sectionOption = [Option]::new(@("-G", "--group")).WithValues(@(getSections))
         $projectOption = [Option]::new(@("-p", "--project")).WithValues(@())
         $skipOption = [Option]::new(@("-k", "--skip")).WithValues(@())
-        $venvOption = [Option]::new(@("--venv")).WithValues(@())
         $formatOption = [Option]::new(@("-f", "--format")).WithValues(@("setuppy", "requirements", "poetry", "flit"))
 
         Switch ($command) {
 
             "add" {
                 $completer.AddOpts(@(
                         [Option]::new((
                             "-d", "--dev", "--save-compatible", "--save-wildcard", "--dry-run", "--save-exact",
                             "--save-minimum", "--update-eager", "--update-reuse", "--update-all", "-g", "--global",
                             "--no-sync", "--no-editable", "--no-self", "-u", "--unconstrained", "--no-isolation",
                             "--pre", "--prerelease", "-L", "--lockfile", "--fail-fast", "-x"
                         )),
                         $sectionOption,
                         $projectOption,
-                        $venvOption,
                         $skipOption
                         [Option]::new(@("-e", "--editable")).WithValues(@(getPyPIPackages))
                     ))
                 $completer.AddParams(@(getPyPIPackages), $true)
                 break
             }
             "build" { $completer.AddOpts(@([Option]::new(@("-d", "--dest", "--no-clean", "--no-sdist", "--no-wheel", "-C", "--config-setting", "--no-isolation")), $projectOption, $skipOption)) }
@@ -270,16 +268,15 @@
                     ))
                 break
             }
             "info" {
                 $completer.AddOpts(
                     @(
                         [Option]::new(@("--env", "--global", "-g", "--python", "--where", "--packages")),
-                        $projectOption,
-                        $venvOption
+                        $projectOption
                     ))
                 break
             }
             "init" {
                 $completer.AddOpts(
                     @(
                         [Option]::new(@("-g", "--global", "--non-interactive", "-n", "--python", "--lib")),
@@ -294,24 +291,22 @@
                         [Option]::new((
                             "-d", "--dev", "-g", "--global", "--dry-run", "--no-default", "--no-lock", "--prod",
                             "--production", "--no-editable", "--no-self", "--no-isolation", "--check", "-L",
                             "--lockfile", "--fail-fast", "-x"
                         )),
                         $sectionOption,
                         $skipOption,
-                        $venvOption,
                         $projectOption
                     ))
                 break
             }
             "list" {
                 $completer.AddOpts(
                     @(
                         [Option]::new(@("--graph", "--global", "-g", "--reverse", "-r", "--freeze", "--json", "--csv", "--markdown", "--fields", "--sort", "--include", "--exclude", "--resolve")),
-                        $venvOption,
                         $projectOption
                     ))
                 break
             }
             "lock" {
                 $completer.AddOpts(
                     @(
@@ -362,50 +357,46 @@
                     @(
                         [Option]::new(@(
                             "--global", "-g", "--dev", "-d", "--dry-run", "--no-sync", "--no-editable", "--no-self",
                             "--no-isolation", "-L", "--lockfile", "--fail-fast", "-x"
                         )),
                         $projectOption,
                         $skipOption,
-                        $venvOption,
                         $sectionOption
                     ))
                 $completer.AddParams(@(getPdmPackages), $true)
                 break
             }
             "run" {
                 $completer.AddOpts(
                     @(
                         [Option]::new(@("--global", "-g", "-l", "--list", "-s", "--site-packages")),
                         $skipOption,
-                        $venvOption,
                         $projectOption
                     ))
                 $completer.AddParams(@(getScripts), $false)
                 break
             }
             "search" { break }
             "show" {
                 $completer.AddOpts(
                     @(
                         [Option]::new(@("--global", "-g", "--name", "--version", "--summary", "--license", "--platform", "--keywords")),
-                        $venvOption,
                         $projectOption
                     ))
                 break
             }
             "sync" {
                 $completer.AddOpts(@(
                         [Option]::new((
                             "-d", "--dev", "-g", "--global", "--no-default", "--clean", "--only-keep", "--dry-run",
                             "-r", "--reinstall", "--prod", "--production", "--no-editable", "--no-self", "--no-isolation",
                             "-L", "--lockfile", "--fail-fast", "-x"
                         )),
                         $sectionOption,
-                        $venvOption,
                         $skipOption,
                         $projectOption
                     ))
                 break
             }
             "update" {
                 $completer.AddOpts(@(
@@ -413,52 +404,50 @@
                             "-d", "--dev", "--save-compatible", "--prod", "--production", "--save-wildcard", "--save-exact",
                             "--save-minimum", "--update-eager", "--update-reuse", "--update-all", "-g", "--global", "--dry-run",
                             "--outdated", "--top", "-u", "--unconstrained", "--no-editable", "--no-self", "--no-isolation",
                             "--no-sync", "--pre", "--prerelease", "-L", "--lockfile", "--fail-fast", "-x"
                         )),
                         $sectionOption,
                         $skipOption,
-                        $venvOption,
                         $projectOption
                     ))
                 $completer.AddParams(@(getPdmPackages), $true)
                 break
             }
             "use" {
                 $completer.AddOpts(
                     @(
                         [Option]::new(@("--global", "-g", "-f", "--first", "-i", "--ignore-remembered", "--skip")),
-                        $venvOption,
                         $projectOption
                     ))
                 break
             }
             "venv" {
                 $subCommand = $commands[1]
                 switch ($subCommand) {
                     "create" {
                         $command = $subCommand
                         $completer.AddOpts((
                             [Option]::new(("--with", "-w")).WithValues(@("venv", "virtualenv", "conda")),
                             [Option]::new(("--name", "-n")).WithValues(@()),
-                            [Option]::new(("--with-pip", "-f", "--force"))
+                            [Option]::new(("--with-pip", "-f", "--force")),
                         ))
                     }
                     "list" {$command = $subCommand}
                     "remove" {
                         $command = $subCommand
                         $completer.AddOpts(([Option]::new(("-y", "--yes"))))
                     }
                     "activate" {$command = $subCommand}
                     "purge" {
                         $command = $subCommand
                         $completer.AddOpts(([Option]::new(("-i", "--interactive", "--force", "-f"))))
                     }
                     Default {
-                        $completer.AddOpts(([Option]::new(("--python", "--path"))))
+                        $completer.AddOpts(([Option]::new(("--python", "--path"))
                         $completer.AddParams(@("create", "list", "remove", "activate", "purge"), $false)
                         break
                     }
                 }
                 break
             }
```

### Comparing `pdm-2.5.0/src/pdm/cli/completions/pdm.zsh` & `pdm-2.5.0b0/src/pdm/cli/completions/pdm.zsh`

 * *Files 5% similar despite different names*

```diff
@@ -69,15 +69,14 @@
         '--save-exact[Save exact version specifiers]'
         '--save-minimum[Save minimum version specifiers]'
         '--update-reuse[Reuse pinned versions already present in lock file if possible]'
         '--update-eager[Try to update the packages and their dependencies recursively]'
         '--update-all[Update all dependencies and sub-dependencies]'
         '--no-editable[Install non-editable versions for all packages]'
         "--no-self[Don't install the project itself]"
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]]:venv:'
         {-k,--skip}'[Skip some tasks and/or hooks by their comma-separated names]'
         {-u,--unconstrained}'[Ignore the version constraint of packages]'
         {--pre,--prerelease}'[Allow prereleases to be pinned]'
         {-e+,--editable+}'[Specify editable packages]:packages'
         {-x,--fail-fast}'[Abort on first installation error]'
         "--no-isolation[do not isolate the build in a clean environment]"
         "--dry-run[Show the difference only without modifying the lockfile content]"
@@ -170,15 +169,14 @@
     info)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         '--python[Show the interpreter path]'
         '--where[Show the project root path]'
         '--env[Show PEP 508 environment markers]'
         '--packages[Show the packages root]'
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]]:venv:'
       )
       ;;
     init)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-n,--non-interactive}"[Don't ask questions but use default values]"
         {-k,--skip}'[Skip some tasks and/or hooks by their comma-separated names]'
@@ -199,15 +197,14 @@
         "--no-default[Don\'t include dependencies from the default group]"
         '--no-editable[Install non-editable versions for all packages]'
         "--no-self[Don't install the project itself]"
         {-x,--fail-fast}'[Abort on first installation error]'
         "--no-isolation[do not isolate the build in a clean environment]"
         "--dry-run[Show the difference only without modifying the lock file content]"
         "--check[Check if the lock file is up to date and fail otherwise]"
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]]:venv:'
       )
       ;;
     list)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-r,--reverse}'[Reverse the dependency graph]'
         '--fields[Select information to output as a comma separated string.]:fields:'
@@ -216,15 +213,14 @@
         '--csv[Output dependencies in CSV document format]'
         '--markdown[Output dependencies and legal notices in markdown document format - best effort basis]'
         '--graph[Display a graph of dependencies]'
         "--freeze[Show the installed dependencies as pip's requirements.txt format]"
         "--include[Dependency groups to include in the output. By default all are included]:include:"
         "--exclude[Dependency groups to exclude from the output]:exclude:"
         "--resolve[Resolve all requirements to output licenses (instead of just showing those currently installed)"
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]]:venv:'
       )
       ;;
     lock)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-L,--lockfile}'[Specify another lockfile path, or use `PDM_LOCKFILE` env variable. Default: pdm.lock]:lockfile:_files'
         "--no-isolation[Do not isolate the build in a clean environment]"
@@ -308,25 +304,23 @@
         {-k,--skip}'[Skip some tasks and/or hooks by their comma-separated names]'
         "--no-sync[Only write pyproject.toml and do not uninstall packages]"
         '--no-editable[Install non-editable versions for all packages]'
         "--no-self[Don't install the project itself]"
         {-x,--fail-fast}'[Abort on first installation error]'
         "--no-isolation[do not isolate the build in a clean environment]"
         "--dry-run[Show the difference only without modifying the lockfile content]"
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]]:venv:'
         "*:packages:_pdm_packages"
       )
       ;;
     run)
       _arguments -s \
         {-g,--global}'[Use the global project, supply the project root with `-p` option]' \
         {-l,--list}'[Show all available scripts defined in pyproject.toml]' \
         {-k,--skip}'[Skip some tasks and/or hooks by their comma-separated names]' \
         {-s,--site-packages}'[Load site-packages from the selected interpreter]' \
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]]:venv:' \
         '(-)1:command:->command' \
         '*:arguments: _normal ' && return 0
       if [[ $state == command ]]; then
         _command_names -e
         local local_commands=($(_pdm_scripts))
         _describe "local command" local_commands
         return 0
@@ -342,15 +336,14 @@
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         '--name[Show name]'
         '--version[Show version]'
         '--summary[Show summary]'
         '--license[Show license]'
         '--platform[Show platform]'
         '--keywords[Show keywords]'
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]]:venv:'
         '1:package:'
       )
       ;;
     sync)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-G+,--group+}'[Select group of optional-dependencies or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species]:group:_pdm_groups'
@@ -363,15 +356,14 @@
         '--clean[Clean unused packages]'
         "--only-keep[Only keep the selected packages]"
         "--no-default[Don\'t include dependencies from the default group]"
         {-x,--fail-fast}'[Abort on first installation error]'
         '--no-editable[Install non-editable versions for all packages]'
         "--no-self[Don't install the project itself]"
         "--no-isolation[do not isolate the build in a clean environment]"
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]]:venv:'
       )
       ;;
     update)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-G+,--group+}'[Select group of optional-dependencies or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species]:group:_pdm_groups'
         {-L,--lockfile}'[Specify another lockfile path, or use `PDM_LOCKFILE` env variable. Default: pdm.lock]:lockfile:_files'
@@ -392,23 +384,21 @@
         {--prod,--production}"[Unselect dev dependencies]"
         "--no-default[Don\'t include dependencies from the default group]"
         {-t,--top}'[Only update those list in pyproject.toml]'
         "--dry-run[Show the difference only without modifying the lockfile content]"
         "--outdated[Show the difference only without modifying the lockfile content]"
         {-x,--fail-fast}'[Abort on first installation error]'
         "--no-isolation[do not isolate the build in a clean environment]"
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]]:venv:'
         "*:packages:_pdm_packages"
       )
       ;;
     use)
       arguments+=(
         {-f,--first}'[Select the first matched interpreter]'
         {-i,--ignore-remembered}'[Ignore the remembered selection]'
-        '--venv[Use the interpreter in the virtual environment with the given name]:venv:'
         '*:python:_files'
       )
       ;;
     venv)
       _arguments -C \
         $arguments \
         ': :->command' \
```

### Comparing `pdm-2.5.0/src/pdm/cli/filters.py` & `pdm-2.5.0b0/src/pdm/cli/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,24 +83,22 @@
         invalid_groups = groups_set - set(project.iter_groups())
         if invalid_groups:
             project.core.ui.echo(
                 "[d]Ignoring non-existing groups: [success]" f"{', '.join(invalid_groups)}[/]",
                 err=True,
             )
             groups_set -= invalid_groups
+        extra_groups = project.lockfile.compare_groups(groups_set)
+        if extra_groups:
+            raise PdmUsageError(f"Requested groups not in lockfile: {','.join(extra_groups)}")
         # Sorts the result in ascending order instead of in random order
         # to make this function pure
         result = sorted(groups_set)
         if default:
             result.insert(0, "default")
         return result
 
-    def validate(self) -> None:
-        extra_groups = self.project.lockfile.compare_groups(self._translated_groups)
-        if extra_groups:
-            raise PdmUsageError(f"Requested groups not in lockfile: {','.join(extra_groups)}")
-
     def __iter__(self) -> Iterator[str]:
         return iter(self._translated_groups)
 
     def __contains__(self, group: str) -> bool:
         return group in self._translated_groups
```

### Comparing `pdm-2.5.0/src/pdm/cli/hooks.py` & `pdm-2.5.0b0/src/pdm/cli/hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/cli/options.py` & `pdm-2.5.0b0/src/pdm/cli/options.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 
 import argparse
 import os
-import sys
-from functools import partial
-from typing import Any, Sequence, cast
+from typing import Any, Sequence
 
-from pdm.cli.actions import print_pep582_command
 from pdm.compat import Protocol
-from pdm.project import Project
 
 
 class ActionCallback(Protocol):
-    def __call__(self, project: Project, namespace: argparse.Namespace, values: str | Sequence[Any] | None) -> None:
+    def __call__(
+        self,
+        parser: argparse.ArgumentParser,
+        namespace: argparse.Namespace,
+        values: str | Sequence[Any] | None,
+        option_string: str | None,
+    ) -> None:
         ...
 
 
 class Option:
     """A reusable option object which delegates all arguments
     to parser.add_argument().
     """
@@ -27,35 +29,28 @@
 
     def add_to_parser(self, parser: argparse._ActionsContainer) -> None:
         parser.add_argument(*self.args, **self.kwargs)
 
     def add_to_group(self, group: argparse._ArgumentGroup) -> None:
         group.add_argument(*self.args, **self.kwargs)
 
-    def __call__(self, func: ActionCallback) -> Option:
-        self.kwargs.update(action=CallbackAction, callback=func)
-        return self
-
 
 class CallbackAction(argparse.Action):
     def __init__(self, *args: Any, callback: ActionCallback, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.callback = callback
 
     def __call__(
         self,
         parser: argparse.ArgumentParser,
         namespace: argparse.Namespace,
         values: str | Sequence[Any] | None,
         option_string: str | None = None,
     ) -> None:
-        if not hasattr(namespace, "callbacks"):
-            namespace.callbacks = []
-        callback = partial(self.callback, values=values)
-        namespace.callbacks.append(callback)
+        return self.callback(parser, namespace, values, option_string=option_string)
 
 
 class ArgumentGroup(Option):
     """A reusable argument group object which can call `add_argument()`
     to add more arguments. And itself will be registered to the parser later.
     """
 
@@ -134,28 +129,28 @@
 dry_run_option = Option(
     "--dry-run",
     action="store_true",
     default=False,
     help="Show the difference only and don't perform any action",
 )
 
-
 lockfile_option = Option(
     "-L",
     "--lockfile",
     default=os.getenv("PDM_LOCKFILE"),
     help="Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]",
 )
 
-
-@Option("--pep582", const="AUTO", metavar="SHELL", nargs="?", help="Print the command line to be eval'd by the shell")
-def pep582_option(project: Project, namespace: argparse.Namespace, values: str | Sequence[Any] | None) -> None:
-    print_pep582_command(project, cast(str, values))
-    sys.exit(0)
-
+pep582_option = Option(
+    "--pep582",
+    const="AUTO",
+    metavar="SHELL",
+    nargs="?",
+    help="Print the command line to be eval'd by the shell",
+)
 
 install_group = ArgumentGroup("Install options")
 install_group.add_argument(
     "--no-editable",
     action="store_true",
     dest="no_editable",
     help="Install non-editable versions for all packages",
@@ -165,19 +160,31 @@
     action="store_true",
     dest="no_self",
     help="Don't install the project itself",
 )
 install_group.add_argument("--fail-fast", "-x", action="store_true", help="Abort on first installation error")
 
 
-@Option("--no-isolation", dest="build_isolation", nargs=0, help="Do not isolate the build in a clean environment")
-def no_isolation_option(project: Project, namespace: argparse.Namespace, values: str | Sequence[Any] | None) -> None:
+def no_isolation_callback(
+    parser: argparse.ArgumentParser,
+    namespace: argparse.Namespace,
+    values: str | Sequence[Any] | None,
+    option_string: str | None,
+) -> None:
     os.environ["PDM_BUILD_ISOLATION"] = "no"
 
 
+no_isolation_option = Option(
+    "--no-isolation",
+    dest="build_isolation",
+    action=CallbackAction,
+    nargs=0,
+    help="Do not isolate the build in a clean environment",
+    callback=no_isolation_callback,
+)
 install_group.options.append(no_isolation_option)
 
 groups_group = ArgumentGroup("Dependencies selection")
 groups_group.add_argument(
     "-G",
     "--group",
     dest="groups",
@@ -310,24 +317,22 @@
     dest="editables",
     action="append",
     help="Specify editable packages",
     default=[],
 )
 packages_group.add_argument("packages", nargs="*", help="Specify packages")
 
-
-@Option(
+ignore_python_option = Option(
     "-I",
     "--ignore-python",
+    action=CallbackAction,
     nargs=0,
-    help="Ignore the Python path saved in .pdm-python. [env var: PDM_IGNORE_SAVED_PYTHON]",
+    help="Ignore the Python path saved in .pdm-python",
+    callback=lambda *args, **kwargs: os.environ.update({"PDM_IGNORE_SAVED_PYTHON": "1"}),
 )
-def ignore_python_option(project: Project, namespace: argparse.Namespace, values: str | Sequence[Any] | None) -> None:
-    os.environ.update({"PDM_IGNORE_SAVED_PYTHON": "1"})
-
 
 prerelease_option = Option(
     "--pre",
     "--prerelease",
     action="store_true",
     dest="prerelease",
     help="Allow prereleases to be pinned",
@@ -335,18 +340,7 @@
 unconstrained_option = Option(
     "-u",
     "--unconstrained",
     action="store_true",
     default=False,
     help="Ignore the version constraint of packages",
 )
-
-
-venv_option = Option(
-    "--venv",
-    dest="use_venv",
-    metavar="NAME",
-    nargs="?",
-    const="in-project",
-    help="Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]",
-    default=os.getenv("PDM_USE_VENV"),
-)
```

### Comparing `pdm-2.5.0/src/pdm/cli/utils.py` & `pdm-2.5.0b0/src/pdm/cli/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -656,18 +656,7 @@
     script_dir = project.global_config.config_file.parent / "pep582"
     if script_dir.joinpath("sitecustomize.py").exists():
         return str(script_dir)
     script_dir.mkdir(parents=True, exist_ok=True)
     with resources_open_binary("pdm.pep582", "sitecustomize.py") as f:
         script_dir.joinpath("sitecustomize.py").write_bytes(f.read())
     return str(script_dir)
-
-
-def use_venv(project: Project, name: str) -> None:
-    from pdm.cli.commands.venv.utils import get_venv_python, get_venv_with_name
-    from pdm.environments import PythonEnvironment
-
-    venv = get_venv_with_name(project, cast(str, name))
-    project.core.ui.echo(
-        f"In virtual environment: [success]{venv}[/]", err=True, style="info", verbosity=termui.Verbosity.DETAIL
-    )
-    project.environment = PythonEnvironment(project, python=str(get_venv_python(venv)))
```

### Comparing `pdm-2.5.0/src/pdm/compat.py` & `pdm-2.5.0b0/src/pdm/compat.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/core.py` & `pdm-2.5.0b0/src/pdm/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from pathlib import Path
 from typing import Any, Iterable, cast
 
 from resolvelib import Resolver
 
 from pdm import termui
 from pdm.__version__ import __version__
-from pdm.cli.actions import check_update
+from pdm.cli.actions import check_update, print_pep582_command
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.options import ignore_python_option, pep582_option, verbose_option
 from pdm.cli.utils import ErrorArgumentParser, PdmFormatter
 from pdm.compat import importlib_metadata
 from pdm.exceptions import PdmArgumentError, PdmUsageError
 from pdm.installers import InstallManager, Synchronizer
 from pdm.models.repositories import PyPIRepository
@@ -100,14 +100,17 @@
 
             default_root = None if global_project or getattr(options, "search_parent", True) else "."
             project = self.create_project(
                 getattr(options, "project_path", None) or default_root,
                 is_global=global_project,
                 global_config=options.config or os.getenv("PDM_CONFIG_FILE"),
             )
+
+        if getattr(options, "lockfile", None):
+            project.set_lockfile(options.lockfile)
         return project
 
     def create_project(
         self,
         root_path: str | Path | None = None,
         is_global: bool = False,
         global_config: str | None = None,
@@ -124,33 +127,26 @@
         """
         return self.project_class(self, root_path, is_global, global_config)
 
     def before_invoke(self, project: Project, command: BaseCommand | None, options: argparse.Namespace) -> None:
         """Called before command invocation"""
         from pdm.cli.commands.fix import Command as FixCommand
         from pdm.cli.hooks import HookManager
-        from pdm.cli.utils import use_venv
 
         self.ui.set_verbosity(options.verbose)
         self.ui.set_theme(project.global_config.load_theme())
-
         hooks = HookManager(project, getattr(options, "skip", None))
         hooks.try_emit("pre_invoke", command=command.name if command else None, options=options)
 
-        if not isinstance(command, FixCommand):
+        if not isinstance(getattr(options, "__command__", None), FixCommand):
             FixCommand.check_problems(project)
 
-        for callback in getattr(options, "callbacks", []):
-            callback(project, options)
-
-        if getattr(options, "lockfile", None):
-            project.set_lockfile(cast(str, options.lockfile))
-
-        if getattr(options, "use_venv", None):
-            use_venv(project, cast(str, options.use_venv))
+        if options.pep582:
+            print_pep582_command(project, options.pep582)
+            sys.exit(0)
 
     def main(
         self,
         args: list[str] | None = None,
         prog_name: str | None = None,
         obj: Project | None = None,
         **extra: Any,
@@ -172,24 +168,25 @@
                 self.parser.error(str(e.__cause__))
             try:
                 options = self.parser.parse_args(["run", *args])
             except PdmArgumentError as e:
                 self.parser.error(str(e.__cause__))
 
         project = self.ensure_project(options, obj)
-        command = getattr(options, "command", None)
+        command = getattr(options, "__command__", None)
+        self.before_invoke(project, command, options)
 
         if root_script and root_script not in project.scripts:
             self.parser.error(f"Script unknown: {root_script}")
 
         if command is None:
-            self.parser.error("No command given")
+            self.parser.print_help(sys.stderr)
+            sys.exit(1)
         assert isinstance(command, BaseCommand)
         try:
-            self.before_invoke(project, command, options)
             command.handle(project, options)
         except Exception:
             etype, err, traceback = sys.exc_info()
             should_show_tb = not isinstance(err, PdmUsageError)
             if self.ui.verbosity > termui.Verbosity.NORMAL and should_show_tb:
                 raise cast(Exception, err).with_traceback(traceback) from None
             self.ui.echo(
```

### Comparing `pdm-2.5.0/src/pdm/environments/__init__.py` & `pdm-2.5.0b0/src/pdm/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/environments/base.py` & `pdm-2.5.0b0/src/pdm/environments/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pdm.compat import cached_property
 from pdm.exceptions import BuildError, PdmUsageError
 from pdm.models.auth import PdmBasicAuth
 from pdm.models.in_process import get_pep508_environment, get_python_abi_tag
 from pdm.models.python import PythonInfo
 from pdm.models.session import PDMSession
 from pdm.models.working_set import WorkingSet
-from pdm.utils import get_trusted_hosts, is_pip_compatible_with_python
+from pdm.utils import get_index_urls, is_pip_compatible_with_python
 
 if TYPE_CHECKING:
     from pdm._types import RepositoryConfig
     from pdm.project import Project
 
 
 class BaseEnvironment(abc.ABC):
@@ -41,19 +41,14 @@
         self.project = project
         self.auth = PdmBasicAuth(
             self.project.sources,
             self.project.core.ui.verbosity >= termui.Verbosity.DETAIL,
         )
 
     @property
-    def is_global(self) -> bool:
-        """For backward compatibility, it is opposite to ``is_local``."""
-        return not self.is_local
-
-    @property
     def interpreter(self) -> PythonInfo:
         return self.project.python
 
     @abc.abstractmethod
     def get_paths(self) -> dict[str, str]:
         """Get paths like ``sysconfig.get_paths()`` for installation."""
         ...
@@ -69,18 +64,19 @@
 
     @cached_property
     def target_python(self) -> unearth.TargetPython:
         python_version = self.interpreter.version_tuple
         python_abi_tag = get_python_abi_tag(str(self.interpreter.executable))
         return unearth.TargetPython(python_version, [python_abi_tag])
 
-    def _build_session(self, trusted_hosts: list[str]) -> PDMSession:
+    def _build_session(self, index_urls: list[str], trusted_hosts: list[str]) -> PDMSession:
         ca_certs = self.project.config.get("pypi.ca_certs")
         session = PDMSession(
             cache_dir=self.project.cache("http"),
+            index_urls=index_urls,
             trusted_hosts=trusted_hosts,
             ca_certificates=Path(ca_certs) if ca_certs is not None else None,
         )
         certfn = self.project.config.get("pypi.client_cert")
         if certfn:
             keyfn = self.project.config.get("pypi.client_key")
             session.cert = (Path(certfn), Path(keyfn) if keyfn else None)
@@ -105,35 +101,30 @@
         if not sources:
             raise PdmUsageError(
                 "You must specify at least one index in pyproject.toml or config.\n"
                 "The 'pypi.ignore_stored_index' config value is "
                 f"{self.project.config['pypi.ignore_stored_index']}"
             )
 
-        trusted_hosts = get_trusted_hosts(sources)
+        index_urls, find_links, trusted_hosts = get_index_urls(sources)
 
-        session = self._build_session(trusted_hosts)
+        session = self._build_session(index_urls, trusted_hosts)
         finder = unearth.PackageFinder(
             session=session,
+            index_urls=index_urls,
+            find_links=find_links,
             target_python=self.target_python,
             ignore_compatibility=ignore_compatibility,
             no_binary=os.getenv("PDM_NO_BINARY", "").split(","),
             only_binary=os.getenv("PDM_ONLY_BINARY", "").split(","),
-            prefer_binary=os.getenv("PDM_PREFER_BINARY", "").split(","),
             respect_source_order=self.project.pyproject.settings.get("resolution", {}).get(
                 "respect-source-order", False
             ),
             verbosity=self.project.core.ui.verbosity,
         )
-        for source in sources:
-            assert source.url
-            if source.type == "find_links":
-                finder.add_find_links(source.url)
-            else:
-                finder.add_index_url(source.url)
         try:
             yield finder
         finally:
             session.close()
 
     def get_working_set(self) -> WorkingSet:
         """Get the working set based on local packages directory."""
```

### Comparing `pdm-2.5.0/src/pdm/environments/local.py` & `pdm-2.5.0b0/src/pdm/environments/local.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/environments/prefix.py` & `pdm-2.5.0b0/src/pdm/environments/prefix.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/environments/python.py` & `pdm-2.5.0b0/src/pdm/environments/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/exceptions.py` & `pdm-2.5.0b0/src/pdm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/formats/__init__.py` & `pdm-2.5.0b0/src/pdm/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/formats/base.py` & `pdm-2.5.0b0/src/pdm/formats/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/formats/flit.py` & `pdm-2.5.0b0/src/pdm/formats/flit.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/formats/pipfile.py` & `pdm-2.5.0b0/src/pdm/formats/pipfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/formats/poetry.py` & `pdm-2.5.0b0/src/pdm/formats/poetry.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/formats/requirements.py` & `pdm-2.5.0b0/src/pdm/formats/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/formats/setup_py.py` & `pdm-2.5.0b0/src/pdm/formats/setup_py.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/installers/core.py` & `pdm-2.5.0b0/src/pdm/installers/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/installers/installers.py` & `pdm-2.5.0b0/src/pdm/installers/installers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/installers/manager.py` & `pdm-2.5.0b0/src/pdm/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/installers/packages.py` & `pdm-2.5.0b0/src/pdm/installers/packages.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/installers/synchronizers.py` & `pdm-2.5.0b0/src/pdm/installers/synchronizers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/installers/uninstallers.py` & `pdm-2.5.0b0/src/pdm/installers/uninstallers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/models/auth.py` & `pdm-2.5.0b0/src/pdm/models/auth.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/models/backends.py` & `pdm-2.5.0b0/src/pdm/models/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/models/caches.py` & `pdm-2.5.0b0/src/pdm/models/caches.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/models/candidates.py` & `pdm-2.5.0b0/src/pdm/models/candidates.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         :param version: the version of the candidate.
         :param link: the file link of the candidate.
         """
         self.req = req
         self.name = name or self.req.project_name
         self.version = version
         if link is None and not req.is_named:
-            link = cast(Link, req.as_file_link())  # type: ignore[attr-defined]
+            link = req.as_file_link()  # type: ignore[attr-defined]
         self.link = link
         self.summary = ""
         self.hashes: dict[Link, str] | None = None
 
         self._requires_python: str | None = None
         self._prepared: PreparedCandidate | None = None
```

### Comparing `pdm-2.5.0/src/pdm/models/in_process/__init__.py` & `pdm-2.5.0b0/src/pdm/models/in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/models/in_process/get_abi_tag.py` & `pdm-2.5.0b0/src/pdm/models/in_process/get_abi_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     var is unset or unavailable."""
     val = get_config_var(var)
     if val is None:
         if warn:
             warnings.warn(
                 "Config variable '{}' is unset, Python ABI tag may be incorrect".format(var),
                 RuntimeWarning,
-                stacklevel=2,
+                2,
             )
         return fallback
     return val == expected
 
 
 if __name__ == "__main__":
     soabi = get_config_var("SOABI")
```

### Comparing `pdm-2.5.0/src/pdm/models/in_process/parse_setup.py` & `pdm-2.5.0b0/src/pdm/models/in_process/parse_setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/models/in_process/pep508.py` & `pdm-2.5.0b0/src/pdm/models/in_process/pep508.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/models/in_process/sysconfig_get_paths.py` & `pdm-2.5.0b0/src/pdm/models/in_process/sysconfig_get_paths.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/models/markers.py` & `pdm-2.5.0b0/src/pdm/models/markers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/models/project_info.py` & `pdm-2.5.0b0/src/pdm/models/project_info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/models/python.py` & `pdm-2.5.0b0/src/pdm/models/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/models/repositories.py` & `pdm-2.5.0b0/src/pdm/models/repositories.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
 import dataclasses
 import posixpath
 import sys
-from functools import wraps
+from functools import lru_cache, wraps
 from typing import TYPE_CHECKING, Any, Callable, Iterable, Mapping, TypeVar, cast
 
 from unearth import Link
-from unearth.utils import LazySequence
 
 from pdm import termui
 from pdm.exceptions import CandidateInfoNotFound, CandidateNotFound
 from pdm.models.candidates import Candidate, make_candidate
 from pdm.models.requirements import (
     Requirement,
     filter_requirements_with_extras,
@@ -141,66 +140,65 @@
         """
         # `allow_prereleases` is None means leave it to specifier to decide whether to
         # include prereleases
 
         if self.is_this_package(requirement):
             return [self.make_this_candidate(requirement)]
         requires_python = requirement.requires_python & self.environment.python_requires
-        cans = LazySequence(self._find_candidates(requirement))
-        applicable_cans = LazySequence(
+        cans = list(self._find_candidates(requirement))
+        applicable_cans = [
             c
             for c in cans
             if requirement.specifier.contains(c.version, allow_prereleases)  # type: ignore[arg-type, union-attr]
-        )
+        ]
 
-        applicable_cans_python_compatible = LazySequence(
+        applicable_cans_python_compatible = [
             c for c in applicable_cans if ignore_requires_python or requires_python.is_subset(c.requires_python)
-        )
+        ]
         # Evaluate data-requires-python attr and discard incompatible candidates
         # to reduce the number of candidates to resolve.
         if applicable_cans_python_compatible:
             applicable_cans = applicable_cans_python_compatible
 
         if not applicable_cans:
             termui.logger.debug("\tCould not find any matching candidates.")
 
         if not applicable_cans and allow_prereleases is None:
             # No non-pre-releases is found, force pre-releases now
-            applicable_cans = LazySequence(
+            applicable_cans = [
                 c for c in cans if requirement.specifier.contains(c.version, True)  # type: ignore[arg-type, union-attr]
-            )
-            applicable_cans_python_compatible = LazySequence(
+            ]
+            applicable_cans_python_compatible = [
                 c for c in applicable_cans if ignore_requires_python or requires_python.is_subset(c.requires_python)
-            )
+            ]
             if applicable_cans_python_compatible:
                 applicable_cans = applicable_cans_python_compatible
 
             if not applicable_cans:
                 termui.logger.debug(
                     "\tCould not find any matching candidates even when considering pre-releases.",
                 )
 
-        def log_candidates(title: str, candidates: Iterable[Candidate], max_lines: int = 10) -> None:
+        def print_candidates(title: str, candidates: list[Candidate], max_lines: int = 10) -> None:
             termui.logger.debug("\t" + title)
             logged_lines = set()
             for can in candidates:
                 new_line = f"\t  {can!r}"
                 if new_line not in logged_lines:
                     logged_lines.add(new_line)
                     if len(logged_lines) > max_lines:
-                        termui.logger.debug("\t  ... [more]")
+                        termui.logger.debug(f"\t  ... [{len(candidates)-max_lines} more candidate(s)]")
                         break
                     else:
                         termui.logger.debug(new_line)
 
-        if self.environment.project.core.ui.verbosity >= termui.Verbosity.DEBUG:
-            if applicable_cans:
-                log_candidates("Found matching candidates:", applicable_cans)
-            elif cans:
-                log_candidates("Found but non-matching candidates:", cans)
+        if applicable_cans:
+            print_candidates("Found matching candidates:", applicable_cans)
+        elif cans:
+            print_candidates("Found but non-matching candidates:", cans)
 
         return applicable_cans
 
     def _get_dependencies_from_cache(self, candidate: Candidate) -> CandidateInfo:
         try:
             result = self._candidate_info_cache.get(candidate)
         except KeyError:
@@ -224,38 +222,33 @@
             or candidate.req.is_file_or_url
             and candidate.req.is_local_dir  # type: ignore[attr-defined]
         ):
             return None
         if candidate.hashes:
             return candidate.hashes
         req = candidate.req.as_pinned_version(candidate.version)
-        comes_from = candidate.link.comes_from if candidate.link else None
-        result: dict[str, str] = {}
-        logged = False
-        respect_source_order = self.environment.project.pyproject.settings.get("resolution", {}).get(
-            "respect-source-order", False
-        )
-        if req.is_named and respect_source_order and comes_from:
-            sources = [s for s in self.sources if comes_from.startswith(s.url)]
+        if candidate.req.is_file_or_url:
+            matching_candidates: Iterable[Candidate] = [candidate]
         else:
-            sources = self.sources
-        with self.environment.get_finder(sources, self.ignore_compatibility) as finder:
-            if req.is_file_or_url:
-                this_link = cast(Link, candidate.prepare(self.environment).link)
-                links: list[Link] = [this_link]
-            else:  # the req must be a named requirement
-                links = [package.link for package in finder.find_matches(req.as_line())]
-            for link in links:
-                if not link or link.is_vcs or link.is_file and link.file_path.is_dir():
-                    # The links found can still be a local directory or vcs, skippping it.
+            matching_candidates = self.find_candidates(req, ignore_requires_python=True)
+        result: dict[str, str] = {}
+        with self.environment.get_finder(self.sources) as finder:
+            for c in matching_candidates:
+                assert c.link is not None
+                # Prepare the candidate to replace vars in the link URL
+                prepared_link = c.prepare(self.environment).link
+                if (
+                    not prepared_link
+                    or prepared_link.is_vcs
+                    or prepared_link.is_file
+                    and prepared_link.file_path.is_dir()
+                ):
                     continue
-                if not logged:
-                    termui.logger.info("Fetching hashes for %s", candidate)
-                    logged = True
-                result[link] = self._hash_cache.get_hash(link, finder.session)
+                termui.logger.info("Fetching hashes for %s", candidate)
+                result[c.link] = self._hash_cache.get_hash(prepared_link, finder.session)
         return result or None
 
     def dependency_generators(self) -> Iterable[Callable[[Candidate], CandidateInfo]]:
         """Return an iterable of getter functions to get dependencies, which will be
         called one by one.
         """
         raise NotImplementedError
@@ -311,21 +304,22 @@
 
     def dependency_generators(self) -> Iterable[Callable[[Candidate], CandidateInfo]]:
         yield self._get_dependencies_from_cache
         if self.environment.project.config["pypi.json_api"]:
             yield self._get_dependencies_from_json
         yield self._get_dependencies_from_metadata
 
+    @lru_cache()
     def _find_candidates(self, requirement: Requirement) -> Iterable[Candidate]:
         sources = self.get_filtered_sources(requirement)
         with self.environment.get_finder(sources, self.ignore_compatibility) as finder:
-            cans = LazySequence(
+            cans = [
                 Candidate.from_installation_candidate(c, requirement)
                 for c in finder.find_all_packages(requirement.project_name, allow_yanked=requirement.is_pinned)
-            )
+            ]
         if not cans:
             raise CandidateNotFound(
                 f"Unable to find candidates for {requirement.project_name}. There may "
                 "exist some issues with the package name or network condition."
             )
         return cans
```

### Comparing `pdm-2.5.0/src/pdm/models/requirements.py` & `pdm-2.5.0b0/src/pdm/models/requirements.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,15 +432,15 @@
         else:
             req_extras = set()
         if req_extras and not req_extras.isdisjoint(extras) or not req_extras and (include_default or not extras):
             result.append(_r.as_line())
 
     extras_not_found = [e for e in extras if e not in extras_in_meta]
     if extras_not_found:
-        warnings.warn(ExtrasWarning(project_name, extras_not_found), stacklevel=2)
+        warnings.warn(ExtrasWarning(project_name, extras_not_found))
 
     return result
 
 
 def parse_as_pkg_requirement(line: str) -> PackageRequirement:
     """Parse a requirement line as packaging.requirement.Requirement"""
     try:
```

### Comparing `pdm-2.5.0/src/pdm/models/search.py` & `pdm-2.5.0b0/src/pdm/models/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/models/session.py` & `pdm-2.5.0b0/src/pdm/models/session.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/models/setup.py` & `pdm-2.5.0b0/src/pdm/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/models/specifiers.py` & `pdm-2.5.0b0/src/pdm/models/specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/models/versions.py` & `pdm-2.5.0b0/src/pdm/models/versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/models/working_set.py` & `pdm-2.5.0b0/src/pdm/models/working_set.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/pep582/sitecustomize.py` & `pdm-2.5.0b0/src/pdm/pep582/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/project/config.py` & `pdm-2.5.0b0/src/pdm/project/config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/project/core.py` & `pdm-2.5.0b0/src/pdm/project/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,14 @@
                 data = tomlkit.load(fp)
                 if data.get("python", {}).get("path"):
                     return data["python"]["path"]
         return None
 
     @_saved_python.setter
     def _saved_python(self, value: str | None) -> None:
-        self.root.mkdir(parents=True, exist_ok=True)
         python_file = self.root.joinpath(".pdm-python")
         if value is None:
             with contextlib.suppress(FileNotFoundError):
                 python_file.unlink()
             return
         python_file.write_text(value, "utf-8")
 
@@ -188,27 +187,22 @@
         from pdm.cli.commands.venv.utils import get_venv_python, iter_venvs
 
         def match_version(python: PythonInfo) -> bool:
             return python.valid and self.python_requires.contains(python.version, True)
 
         def note(message: str) -> None:
             if not self.is_global:
-                self.core.ui.echo(message, style="info", err=True)
+                self.core.ui.echo(message, style="warning", err=True)
 
         config = self.config
         saved_path = self._saved_python
         if saved_path and not os.getenv("PDM_IGNORE_SAVED_PYTHON"):
             python = PythonInfo.from_path(saved_path)
             if match_version(python):
                 return python
-            else:
-                note(
-                    "The saved Python interpreter doesn't match the project's requirement. "
-                    "Trying to find another one."
-                )
             self._saved_python = None  # Clear the saved path if it doesn't match
 
         if config.get("python.use_venv") and not self.is_global and not os.getenv("PDM_IGNORE_ACTIVE_VENV"):
             # Resolve virtual environments from env-vars
             venv_in_env = os.getenv("VIRTUAL_ENV", os.getenv("CONDA_PREFIX"))
             if venv_in_env:
                 python = PythonInfo.from_path(get_venv_python(Path(venv_in_env)))
```

### Comparing `pdm-2.5.0/src/pdm/project/lockfile.py` & `pdm-2.5.0b0/src/pdm/project/lockfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/project/project_file.py` & `pdm-2.5.0b0/src/pdm/project/project_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/project/toml_file.py` & `pdm-2.5.0b0/src/pdm/project/toml_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/pytest.py` & `pdm-2.5.0b0/src/pdm/pytest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/resolver/core.py` & `pdm-2.5.0b0/src/pdm/resolver/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/resolver/providers.py` & `pdm-2.5.0b0/src/pdm/resolver/providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
             )
 
         return matches_gen
 
     def _compare_file_reqs(self, req1: FileRequirement, req2: FileRequirement) -> bool:
         backend = self.repository.environment.project.backend
         if req1.path and req2.path:
-            return os.path.normpath(req1.path.absolute()) == os.path.normpath(req2.path.absolute())
+            return os.path.normpath(req1.path) == os.path.normpath(req2.path)
         left = backend.expand_line(url_without_fragments(req1.get_full_url()))
         right = backend.expand_line(url_without_fragments(req2.get_full_url()))
         return left == right
 
     def is_satisfied_by(self, requirement: Requirement, candidate: Candidate) -> bool:
         if isinstance(requirement, PythonRequirement):
             return is_python_satisfied_by(requirement, candidate)
```

### Comparing `pdm-2.5.0/src/pdm/resolver/python.py` & `pdm-2.5.0b0/src/pdm/resolver/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/resolver/reporters.py` & `pdm-2.5.0b0/src/pdm/resolver/reporters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/signals.py` & `pdm-2.5.0b0/src/pdm/signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/termui.py` & `pdm-2.5.0b0/src/pdm/termui.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/src/pdm/utils.py` & `pdm-2.5.0b0/src/pdm/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,25 +42,33 @@
     def clean_up() -> None:
         shutil.rmtree(name, ignore_errors=True)
 
     atexit.register(clean_up)
     return name
 
 
-def get_trusted_hosts(sources: list[RepositoryConfig]) -> list[str]:
-    """Parse the project sources and return the trusted hosts"""
-    trusted_hosts = []
+def get_index_urls(
+    sources: list[RepositoryConfig],
+) -> tuple[list[str], list[str], list[str]]:
+    """Parse the project sources and return
+    (index_urls, find_link_urls, trusted_hosts)
+    """
+    index_urls, find_link_urls, trusted_hosts = [], [], []
     for source in sources:
         assert source.url
         url = source.url
         netloc = parse.urlparse(url).netloc
         host = netloc.rsplit("@", 1)[-1]
         if host not in trusted_hosts and source.verify_ssl is False:
             trusted_hosts.append(host)
-    return trusted_hosts
+        if source.type == "find_links":
+            find_link_urls.append(url)
+        else:
+            index_urls.append(url)
+    return index_urls, find_link_urls, trusted_hosts
 
 
 def url_without_fragments(url: str) -> str:
     return parse.urlunparse(parse.urlparse(url)._replace(fragment=""))
 
 
 def join_list_with(items: list[Any], sep: Any) -> list[Any]:
```

### Comparing `pdm-2.5.0/tests/cli/conftest.py` & `pdm-2.5.0b0/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/cli/test_add.py` & `pdm-2.5.0b0/tests/cli/test_add.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/cli/test_build.py` & `pdm-2.5.0b0/tests/cli/test_build.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/cli/test_cache.py` & `pdm-2.5.0b0/tests/cli/test_cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/cli/test_config.py` & `pdm-2.5.0b0/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/cli/test_fix.py` & `pdm-2.5.0b0/tests/cli/test_fix.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/cli/test_hooks.py` & `pdm-2.5.0b0/tests/cli/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/cli/test_init.py` & `pdm-2.5.0b0/tests/cli/test_init.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/cli/test_install.py` & `pdm-2.5.0b0/tests/cli/test_install.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/cli/test_list.py` & `pdm-2.5.0b0/tests/cli/test_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -695,36 +695,14 @@
     assert "[PdmUsageError]" in result.outputs
     assert "--include groups must be selected from" in result.outputs
     assert "dev" in result.outputs
     assert "default" in result.outputs
     assert ":sub" in result.outputs
 
 
-@pytest.mark.usefixtures("local_finder")
-def test_list_packages_in_given_venv(project, pdm):
-    project.pyproject.metadata["requires-python"] = ">=3.7"
-    project.pyproject.write()
-    project.global_config["python.use_venv"] = True
-    pdm(["venv", "create"], obj=project, strict=True)
-    pdm(["venv", "create", "--name", "second"], obj=project, strict=True)
-    project._saved_python = None
-    pdm(["add", "first", "--no-self"], obj=project, strict=True)
-    second_lockfile = str(project.root / "pdm.2.lock")
-    pdm(
-        ["add", "-G", "second", "--no-self", "-L", second_lockfile, "--venv", "second", "editables"],
-        obj=project,
-        strict=True,
-    )
-    project.environment = None
-    result1 = pdm(["list", "--freeze"], obj=project, strict=True)
-    result2 = pdm(["list", "--freeze", "--venv", "second"], obj=project, strict=True)
-    assert result1.output.strip() == "first==2.0.2"
-    assert result2.output.strip() == "editables==0.2"
-
-
 @pytest.mark.usefixtures("working_set", "repository")
 def test_list_csv_include_exclude(project, pdm):
     project.environment.python_requires = PySpecSet(">=3.6")
     dep_path = FIXTURES.joinpath("projects/demo").as_posix()
     pdm(["add", "-de", f"{dep_path}[security]"], obj=project, strict=True)
 
     # Show all groups.
```

### Comparing `pdm-2.5.0/tests/cli/test_lock.py` & `pdm-2.5.0b0/tests/cli/test_lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/cli/test_others.py` & `pdm-2.5.0b0/tests/cli/test_others.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from pathlib import Path
-
 import pytest
 
 from pdm.cli import actions
 from pdm.models.requirements import parse_requirement
 from pdm.utils import cd
 from tests import FIXTURES
 
@@ -21,175 +19,158 @@
 def test_project_no_init_error(project_no_init, pdm):
     for command in ("add", "lock", "update"):
         result = pdm([command], obj=project_no_init)
         assert result.exit_code != 0
         assert "The pyproject.toml has not been initialized yet" in result.stderr
 
 
-def test_help_option(pdm):
-    result = pdm(["--help"])
+def test_help_option(invoke):
+    result = invoke(["--help"])
     assert "Usage: pdm [-h]" in result.output
 
 
-def test_info_command(project, pdm):
-    result = pdm(["info"], obj=project)
+def test_info_command(project, invoke):
+    result = invoke(["info"], obj=project)
     assert "Project Root:" in result.output
     assert project.root.as_posix() in result.output
 
-    result = pdm(["info", "--python"], obj=project)
+    result = invoke(["info", "--python"], obj=project)
     assert result.output.strip() == str(project.python.executable)
 
-    result = pdm(["info", "--where"], obj=project)
+    result = invoke(["info", "--where"], obj=project)
     assert result.output.strip() == str(project.root)
 
-    result = pdm(["info", "--env"], obj=project)
+    result = invoke(["info", "--env"], obj=project)
     assert result.exit_code == 0
 
 
-def test_info_global_project(pdm, tmp_path):
+def test_info_global_project(invoke, tmp_path):
     with cd(tmp_path):
-        result = pdm(["info", "-g", "--where"])
+        result = invoke(["info", "-g", "--where"])
     assert "global-project" in result.output.strip()
 
 
-def test_info_with_multiple_venvs(pdm, project):
-    project.global_config["python.use_venv"] = True
-    pdm(["venv", "create"], obj=project, strict=True)
-    pdm(["venv", "create", "--name", "test"], obj=project, strict=True)
-    project._saved_python = None
-    result = pdm(["info", "--python"], obj=project, strict=True)
-    assert Path(result.output.strip()).parent.parent == project.root / ".venv"
-    venv_location = project.config["venv.location"]
-    result = pdm(["info", "--python", "--venv", "test"], obj=project, strict=True)
-    assert Path(result.output.strip()).parent.parent.parent == project.root / venv_location
-
-    result = pdm(["info", "--python", "--venv", "test"], obj=project, strict=True, env={"PDM_USE_VENV": "test"})
-    assert Path(result.output.strip()).parent.parent.parent == project.root / venv_location
-    result = pdm(["info", "--python", "--venv", "default"], obj=project)
-    assert "No virtualenv with key 'default' is found" in result.stderr
-
-
-def test_global_project_other_location(pdm, project):
-    result = pdm(["info", "-g", "-p", project.root.as_posix(), "--where"])
+def test_global_project_other_location(invoke, project):
+    result = invoke(["info", "-g", "-p", project.root.as_posix(), "--where"])
     assert result.stdout.strip() == str(project.root)
 
 
-def test_uncaught_error(pdm, mocker):
+def test_uncaught_error(invoke, mocker):
     mocker.patch.object(actions, "do_lock", side_effect=RuntimeError("test error"))
-    result = pdm(["lock"])
+    result = invoke(["lock"])
     assert "[RuntimeError]: test error" in result.stderr
 
-    result = pdm(["lock", "-v"])
+    result = invoke(["lock", "-v"])
     assert isinstance(result.exception, RuntimeError)
 
 
 @pytest.mark.parametrize(
     "filename",
     [
         "requirements.txt",
         "Pipfile",
         "pyproject.toml",
         "projects/flit-demo/pyproject.toml",
     ],
 )
-def test_import_other_format_file(project, pdm, filename):
+def test_import_other_format_file(project, invoke, filename):
     requirements_file = FIXTURES / filename
-    result = pdm(["import", str(requirements_file)], obj=project)
+    result = invoke(["import", str(requirements_file)], obj=project)
     assert result.exit_code == 0
 
 
-def test_import_requirement_no_overwrite(project, pdm, tmp_path):
+def test_import_requirement_no_overwrite(project, invoke, tmp_path):
     project.add_dependencies({"requests": parse_requirement("requests")})
     tmp_path.joinpath("reqs.txt").write_text("flask\nflask-login\n")
-    result = pdm(["import", "-dGweb", str(tmp_path.joinpath("reqs.txt"))], obj=project)
+    result = invoke(["import", "-dGweb", str(tmp_path.joinpath("reqs.txt"))], obj=project)
     assert result.exit_code == 0, result.stderr
     assert list(project.get_dependencies()) == ["requests"]
     assert list(project.get_dependencies("web")) == ["flask", "flask-login"]
 
 
 @pytest.mark.network
-def test_search_package(pdm, tmp_path):
+def test_search_package(invoke, tmp_path):
     with cd(tmp_path):
-        result = pdm(["search", "requests"])
+        result = invoke(["search", "requests"])
     assert result.exit_code == 0
     assert len(result.output.splitlines()) > 0
     assert not tmp_path.joinpath("__pypackages__").exists()
     assert not tmp_path.joinpath(".pdm-python").exists()
 
 
 @pytest.mark.network
-def test_show_package_on_pypi(pdm):
-    result = pdm(["show", "ipython"])
+def test_show_package_on_pypi(invoke):
+    result = invoke(["show", "ipython"])
     assert result.exit_code == 0
     assert "ipython" in result.output.splitlines()[0]
 
-    result = pdm(["show", "requests"])
+    result = invoke(["show", "requests"])
     assert result.exit_code == 0
     assert "requests" in result.output.splitlines()[0]
 
-    result = pdm(["show", "--name", "requests"])
+    result = invoke(["show", "--name", "requests"])
     assert result.exit_code == 0
     assert "requests" in result.output.splitlines()[0]
 
-    result = pdm(["show", "--name", "sphinx-data-viewer"])
+    result = invoke(["show", "--name", "sphinx-data-viewer"])
     assert result.exit_code == 0
     assert "sphinx-data-viewer" in result.output.splitlines()[0]
 
 
-def test_show_self_package(project, pdm):
-    result = pdm(["show"], obj=project)
+def test_show_self_package(project, invoke):
+    result = invoke(["show"], obj=project)
     assert result.exit_code == 0, result.stderr
 
-    result = pdm(["show", "--name", "--version"], obj=project)
+    result = invoke(["show", "--name", "--version"], obj=project)
     assert result.exit_code == 0
     assert "test_project\n0.0.0\n" == result.output
 
 
-def test_export_to_requirements_txt(pdm, fixture_project):
+def test_export_to_requirements_txt(invoke, fixture_project):
     project = fixture_project("demo-package")
     requirements_txt = project.root / "requirements.txt"
     requirements_no_hashes = project.root / "requirements_simple.txt"
     requirements_pyproject = project.root / "requirements.ini"
 
-    result = pdm(["export"], obj=project)
+    result = invoke(["export"], obj=project)
     assert result.exit_code == 0
     assert result.output.strip() == requirements_txt.read_text().strip()
 
-    result = pdm(["export", "--without-hashes"], obj=project)
+    result = invoke(["export", "--without-hashes"], obj=project)
     assert result.exit_code == 0
     assert result.output.strip() == requirements_no_hashes.read_text().strip()
 
-    result = pdm(["export", "--pyproject"], obj=project)
+    result = invoke(["export", "--pyproject"], obj=project)
     assert result.exit_code == 0
     assert result.output.strip() == requirements_pyproject.read_text().strip()
 
-    result = pdm(["export", "-o", str(project.root / "requirements_output.txt")], obj=project)
+    result = invoke(["export", "-o", str(project.root / "requirements_output.txt")], obj=project)
     assert result.exit_code == 0
     assert (project.root / "requirements_output.txt").read_text() == requirements_txt.read_text()
 
 
-def test_export_doesnt_include_dep_with_extras(pdm, fixture_project):
+def test_export_doesnt_include_dep_with_extras(invoke, fixture_project):
     project = fixture_project("demo-package-has-dep-with-extras")
     requirements_txt = project.root / "requirements.txt"
 
-    result = pdm(["export", "--without-hashes"], obj=project)
+    result = invoke(["export", "--without-hashes"], obj=project)
     assert result.exit_code == 0
     assert result.output.strip() == requirements_txt.read_text().strip()
 
 
-def test_completion_command(pdm):
-    result = pdm(["completion", "bash"])
+def test_completion_command(invoke):
+    result = invoke(["completion", "bash"])
     assert result.exit_code == 0
     assert "(completion)" in result.output
 
 
 @pytest.mark.network
-def test_show_update_hint(pdm, project, monkeypatch):
+def test_show_update_hint(invoke, project, monkeypatch):
     monkeypatch.delenv("PDM_CHECK_UPDATE", raising=False)
     prev_version = project.core.version
     try:
         project.core.version = "0.0.0"
-        r = pdm(["config"], obj=project)
+        r = invoke(["config"], obj=project)
     finally:
         project.core.version = prev_version
     assert "to upgrade." in r.stderr
     assert "Run `pdm config check_update false` to disable the check." in r.stderr
```

### Comparing `pdm-2.5.0/tests/cli/test_publish.py` & `pdm-2.5.0b0/tests/cli/test_publish.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/cli/test_remove.py` & `pdm-2.5.0b0/tests/cli/test_remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/cli/test_run.py` & `pdm-2.5.0b0/tests/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/cli/test_self_command.py` & `pdm-2.5.0b0/tests/cli/test_self_command.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/cli/test_update.py` & `pdm-2.5.0b0/tests/cli/test_update.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/cli/test_use.py` & `pdm-2.5.0b0/tests/cli/test_use.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,20 +66,7 @@
     assert not cache._cache
     actions.do_use(project, "3", first=True)
     cache._read_cache()
     assert "3" in cache
     mocker.patch.object(project, "find_interpreters")
     actions.do_use(project, "3")
     project.find_interpreters.assert_not_called()
-
-
-def test_use_venv_python(project, pdm):
-    pdm(["venv", "create"], obj=project, strict=True)
-    pdm(["venv", "create", "--name", "test"], obj=project, strict=True)
-    project.global_config["python.use_venv"] = True
-    venv_location = project.config["venv.location"]
-    actions.do_use(project, venv="in-project")
-    assert project.python.executable.parent.parent == project.root.joinpath(".venv")
-    actions.do_use(project, venv="test")
-    assert project.python.executable.parent.parent.parent == Path(venv_location)
-    with pytest.raises(Exception, match="No virtualenv with key 'non-exists' is found"):
-        actions.do_use(project, venv="non-exists")
```

### Comparing `pdm-2.5.0/tests/cli/test_venv.py` & `pdm-2.5.0b0/tests/cli/test_venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/conftest.py` & `pdm-2.5.0b0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl` & `pdm-2.5.0b0/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz` & `pdm-2.5.0b0/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl` & `pdm-2.5.0b0/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl` & `pdm-2.5.0b0/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl` & `pdm-2.5.0b0/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/demo-0.0.1.tar.gz` & `pdm-2.5.0b0/tests/fixtures/artifacts/demo-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/demo-0.0.1.zip` & `pdm-2.5.0b0/tests/fixtures/artifacts/demo-0.0.1.zip`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl` & `pdm-2.5.0b0/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl` & `pdm-2.5.0b0/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl` & `pdm-2.5.0b0/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl` & `pdm-2.5.0b0/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz` & `pdm-2.5.0b0/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl` & `pdm-2.5.0b0/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl` & `pdm-2.5.0b0/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl` & `pdm-2.5.0b0/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl` & `pdm-2.5.0b0/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl` & `pdm-2.5.0b0/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl` & `pdm-2.5.0b0/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl` & `pdm-2.5.0b0/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl` & `pdm-2.5.0b0/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl` & `pdm-2.5.0b0/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock` & `pdm-2.5.0b0/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/projects/demo-package/pdm.lock` & `pdm-2.5.0b0/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm-2.5.0b0/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/projects/demo-package/requirements.txt` & `pdm-2.5.0b0/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/projects/demo-package/setup.txt` & `pdm-2.5.0b0/tests/fixtures/projects/demo-package/setup.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/projects/flit-demo/pyproject.toml` & `pdm-2.5.0b0/tests/fixtures/projects/flit-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/projects/poetry-demo/pyproject.toml` & `pdm-2.5.0b0/tests/fixtures/projects/poetry-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/pypi.json` & `pdm-2.5.0b0/tests/fixtures/pypi.json`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/fixtures/pyproject.toml` & `pdm-2.5.0b0/tests/fixtures/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/models/test_backends.py` & `pdm-2.5.0b0/tests/models/test_backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/models/test_candidates.py` & `pdm-2.5.0b0/tests/models/test_candidates.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/models/test_marker.py` & `pdm-2.5.0b0/tests/models/test_marker.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/models/test_requirements.py` & `pdm-2.5.0b0/tests/models/test_requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/models/test_setup_parsing.py` & `pdm-2.5.0b0/tests/models/test_setup_parsing.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/models/test_specifiers.py` & `pdm-2.5.0b0/tests/models/test_specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/models/test_versions.py` & `pdm-2.5.0b0/tests/models/test_versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/resolver/test_resolve.py` & `pdm-2.5.0b0/tests/resolver/test_resolve.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/test_formats.py` & `pdm-2.5.0b0/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/test_installer.py` & `pdm-2.5.0b0/tests/test_installer.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/test_integration.py` & `pdm-2.5.0b0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/test_plugin.py` & `pdm-2.5.0b0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/test_project.py` & `pdm-2.5.0b0/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/test_signals.py` & `pdm-2.5.0b0/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/tests/test_utils.py` & `pdm-2.5.0b0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.0/PKG-INFO` & `pdm-2.5.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm
-Version: 2.5.0
+Version: 2.5.0b0
 Summary: A modern Python package and dependency manager supporting the latest PEP standards
 Keywords: packaging dependency workflow
 Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -21,15 +21,15 @@
 Requires-Dist: certifi
 Requires-Dist: packaging!=22.0,>=20.9
 Requires-Dist: platformdirs
 Requires-Dist: rich>=12.3.0
 Requires-Dist: virtualenv>=20
 Requires-Dist: pyproject-hooks
 Requires-Dist: requests-toolbelt
-Requires-Dist: unearth>=0.9.0
+Requires-Dist: unearth>=0.8
 Requires-Dist: findpython>=0.2.2
 Requires-Dist: tomlkit<1,>=0.11.1
 Requires-Dist: shellingham>=1.3.2
 Requires-Dist: python-dotenv>=0.15
 Requires-Dist: resolvelib>=1.0.1
 Requires-Dist: installer<0.8,>=0.7
 Requires-Dist: cachecontrol[filecache]>=0.12.11
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1 Name: pdm Version: 2.5.0 Summary: A modern Python package
-and dependency manager supporting the latest PEP standards Keywords: packaging
-dependency workflow Author-Email: Frost Ming
+Metadata-Version: 2.1 Name: pdm Version: 2.5.0b0 Summary: A modern Python
+package and dependency manager supporting the latest PEP standards Keywords:
+packaging dependency workflow Author-Email: Frost Ming
 gmail.com> License: MIT Classifier: Topic :: Software Development :: Build
 Tools Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Homepage, https://pdm.fming.dev Project-URL: Repository, https://
 github.com/pdm-project/pdm Project-URL: Documentation, https://pdm.fming.dev
 Project-URL: Changelog, https://pdm.fming.dev/latest/dev/changelog/ Requires-
 Python: >=3.7 Requires-Dist: blinker Requires-Dist: certifi Requires-Dist:
 packaging!=22.0,>=20.9 Requires-Dist: platformdirs Requires-Dist: rich>=12.3.0
 Requires-Dist: virtualenv>=20 Requires-Dist: pyproject-hooks Requires-Dist:
-requests-toolbelt Requires-Dist: unearth>=0.9.0 Requires-Dist:
-findpython>=0.2.2 Requires-Dist: tomlkit<1,>=0.11.1 Requires-Dist:
-shellingham>=1.3.2 Requires-Dist: python-dotenv>=0.15 Requires-Dist:
-resolvelib>=1.0.1 Requires-Dist: installer<0.8,>=0.7 Requires-Dist:
-cachecontrol[filecache]>=0.12.11 Requires-Dist: tomli>=1.1.0; python_version <
-"3.11" Requires-Dist: typing-extensions; python_version < "3.8" Requires-Dist:
-importlib-metadata>=3.6; python_version < "3.10" Requires-Dist: pytest; extra
-== "pytest" Requires-Dist: pytest-mock; extra == "pytest" Provides-Extra:
-pytest Description-Content-Type: text/markdown
+requests-toolbelt Requires-Dist: unearth>=0.8 Requires-Dist: findpython>=0.2.2
+Requires-Dist: tomlkit<1,>=0.11.1 Requires-Dist: shellingham>=1.3.2 Requires-
+Dist: python-dotenv>=0.15 Requires-Dist: resolvelib>=1.0.1 Requires-Dist:
+installer<0.8,>=0.7 Requires-Dist: cachecontrol[filecache]>=0.12.11 Requires-
+Dist: tomli>=1.1.0; python_version < "3.11" Requires-Dist: typing-extensions;
+python_version < "3.8" Requires-Dist: importlib-metadata>=3.6; python_version <
+"3.10" Requires-Dist: pytest; extra == "pytest" Requires-Dist: pytest-mock;
+extra == "pytest" Provides-Extra: pytest Description-Content-Type: text/
+markdown
 # PDM A modern Python package and dependency manager supporting the latest PEP
       standards. [ä¸­æçæ¬è¯´æ](README_zh.md) ![PDM logo](https://
 raw.githubusercontent.com/pdm-project/pdm/main/docs/docs/assets/logo_big.png)
  [![Docs](https://img.shields.io/badge/Docs-mkdocs-blue?style=for-the-badge)]
   (https://pdm.fming.dev) [![Twitter Follow](https://img.shields.io/twitter/
    follow/pdm_project?label=get%20updates&logo=twitter&style=for-the-badge)]
  (https://twitter.com/pdm_project) [![Discord](https://img.shields.io/discord/
```

