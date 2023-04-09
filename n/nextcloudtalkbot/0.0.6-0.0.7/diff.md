# Comparing `tmp/nextcloudtalkbot-0.0.6.tar.gz` & `tmp/nextcloudtalkbot-0.0.7.tar.gz`

## Comparing `nextcloudtalkbot-0.0.6.tar` & `nextcloudtalkbot-0.0.7.tar`

### file list

```diff
@@ -1,82 +1,67 @@
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/.readthedocs.yaml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/mkdocs.yml
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/docs/FirstRunSetup.md
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/docs/NextcloudFileOperations.md
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/docs/NextcloudTalkExtractor.md
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/docs/NextcloudUser.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/docs/index.md
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/docs/requirements.txt
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/nextcloud_talk_bot/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/nextcloud_talk_bot/check_local_user_enviroment.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/nextcloud_talk_bot/constants.py
--rw-r--r--   0        0        0     7766 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/nextcloud_talk_bot/first_run_setup.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/nextcloud_talk_bot/headers.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/nextcloud_talk_bot/nextcloud_activities.py
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/nextcloud_talk_bot/nextcloud_file_operations.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/nextcloud_talk_bot/nextcloud_requests.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/nextcloud_talk_bot/nextcloud_talk_extractor.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/nextcloud_talk_bot/nextcloud_user.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/nextcloud_talk_bot/nextcloudtalkbot.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/nextcloud_talk_bot/permissions_map.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/nextcloud_talk_bot/read_data.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/nextcloud_talk_bot/send_message.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/nextcloud_talk_bot/translations.py
--rw-r--r--   0        0        0     4171 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/404.html
--rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/index.html
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/requirements.txt
--rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/search.html
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/sitemap.xml
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/sitemap.xml.gz
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/FirstRunSetup/index.html
--rw-r--r--   0        0        0     7056 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/NextcloudFileOperations/index.html
--rw-r--r--   0        0        0     7915 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/NextcloudTalkExtractor/index.html
--rw-r--r--   0        0        0     7863 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/NextcloudUser/index.html
--rw-r--r--   0        0        0   129978 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/css/theme.css
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/css/theme_extra.css
--rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/img/favicon.ico
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/js/html5shiv.min.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/js/theme.js
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/js/theme_extra.js
--rw-r--r--   0        0        0    99805 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/search/lunr.js
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/search/main.js
--rw-r--r--   0        0        0    15361 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/search/search_index.json
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/site/search/worker.js
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/src/nextcloud_talk_bot/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/src/nextcloud_talk_bot/check_local_user_enviroment.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/src/nextcloud_talk_bot/constants.py
--rw-r--r--   0        0        0     7766 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/src/nextcloud_talk_bot/first_run_setup.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/src/nextcloud_talk_bot/headers.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/src/nextcloud_talk_bot/nextcloud_activities.py
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/src/nextcloud_talk_bot/nextcloud_file_operations.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/src/nextcloud_talk_bot/nextcloud_requests.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/src/nextcloud_talk_bot/nextcloud_talk_extractor.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/src/nextcloud_talk_bot/nextcloud_user.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/src/nextcloud_talk_bot/nextcloudtalkbot.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/src/nextcloud_talk_bot/permissions_map.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/src/nextcloud_talk_bot/read_data.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/src/nextcloud_talk_bot/send_message.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/src/nextcloud_talk_bot/translations.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/tests/test_encrypt_password
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/LICENSE
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/README.md
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/.readthedocs.yaml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/mkdocs.yml
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/docs/FirstRunSetup.md
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/docs/NextcloudFileOperations.md
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/docs/NextcloudTalkExtractor.md
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/docs/NextcloudUser.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/docs/index.md
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/docs/requirements.txt
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/nextcloud_talk_bot/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/nextcloud_talk_bot/check_local_user_enviroment.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/nextcloud_talk_bot/constants.py
+-rw-r--r--   0        0        0     7766 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/nextcloud_talk_bot/first_run_setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/nextcloud_talk_bot/headers.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/nextcloud_talk_bot/nextcloud_activities.py
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/nextcloud_talk_bot/nextcloud_file_operations.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/nextcloud_talk_bot/nextcloud_requests.py
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/nextcloud_talk_bot/nextcloud_talk_extractor.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/nextcloud_talk_bot/nextcloud_user.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/nextcloud_talk_bot/nextcloudtalkbot.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/nextcloud_talk_bot/permissions_map.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/nextcloud_talk_bot/read_data.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/nextcloud_talk_bot/send_message.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/nextcloud_talk_bot/translations.py
+-rw-r--r--   0        0        0     4171 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/404.html
+-rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/index.html
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/requirements.txt
+-rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/search.html
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/sitemap.xml
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/sitemap.xml.gz
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/FirstRunSetup/index.html
+-rw-r--r--   0        0        0     7056 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/NextcloudFileOperations/index.html
+-rw-r--r--   0        0        0     7915 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/NextcloudTalkExtractor/index.html
+-rw-r--r--   0        0        0     7863 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/NextcloudUser/index.html
+-rw-r--r--   0        0        0   129978 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/css/theme.css
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/css/theme_extra.css
+-rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/img/favicon.ico
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/js/html5shiv.min.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/js/theme.js
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/js/theme_extra.js
+-rw-r--r--   0        0        0    99805 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/search/lunr.js
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/search/main.js
+-rw-r--r--   0        0        0    15361 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/search/search_index.json
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/site/search/worker.js
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/tests/test_encrypt_password
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/LICENSE
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/README.md
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.7/PKG-INFO
```

### Comparing `nextcloudtalkbot-0.0.6/docs/FirstRunSetup.md` & `nextcloudtalkbot-0.0.7/docs/FirstRunSetup.md`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/docs/NextcloudFileOperations.md` & `nextcloudtalkbot-0.0.7/docs/NextcloudFileOperations.md`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/docs/NextcloudTalkExtractor.md` & `nextcloudtalkbot-0.0.7/docs/NextcloudTalkExtractor.md`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/docs/NextcloudUser.md` & `nextcloudtalkbot-0.0.7/docs/NextcloudUser.md`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/docs/requirements.txt` & `nextcloudtalkbot-0.0.7/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/nextcloud_talk_bot/check_local_user_enviroment.py` & `nextcloudtalkbot-0.0.7/nextcloud_talk_bot/check_local_user_enviroment.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/nextcloud_talk_bot/first_run_setup.py` & `nextcloudtalkbot-0.0.7/nextcloud_talk_bot/first_run_setup.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/nextcloud_talk_bot/headers.py` & `nextcloudtalkbot-0.0.7/nextcloud_talk_bot/headers.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/nextcloud_talk_bot/nextcloud_activities.py` & `nextcloudtalkbot-0.0.7/nextcloud_talk_bot/nextcloud_activities.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/nextcloud_talk_bot/nextcloud_file_operations.py` & `nextcloudtalkbot-0.0.7/nextcloud_talk_bot/nextcloud_file_operations.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/nextcloud_talk_bot/nextcloud_requests.py` & `nextcloudtalkbot-0.0.7/nextcloud_talk_bot/nextcloud_requests.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/nextcloud_talk_bot/nextcloud_talk_extractor.py` & `nextcloudtalkbot-0.0.7/nextcloud_talk_bot/nextcloud_talk_extractor.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/nextcloud_talk_bot/nextcloud_user.py` & `nextcloudtalkbot-0.0.7/nextcloud_talk_bot/nextcloud_user.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/nextcloud_talk_bot/read_data.py` & `nextcloudtalkbot-0.0.7/nextcloud_talk_bot/read_data.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/nextcloud_talk_bot/send_message.py` & `nextcloudtalkbot-0.0.7/nextcloud_talk_bot/send_message.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/404.html` & `nextcloudtalkbot-0.0.7/site/404.html`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/index.html` & `nextcloudtalkbot-0.0.7/site/index.html`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/requirements.txt` & `nextcloudtalkbot-0.0.7/site/requirements.txt`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/search.html` & `nextcloudtalkbot-0.0.7/site/search.html`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/sitemap.xml` & `nextcloudtalkbot-0.0.7/site/sitemap.xml`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/FirstRunSetup/index.html` & `nextcloudtalkbot-0.0.7/site/FirstRunSetup/index.html`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/NextcloudFileOperations/index.html` & `nextcloudtalkbot-0.0.7/site/NextcloudFileOperations/index.html`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/NextcloudTalkExtractor/index.html` & `nextcloudtalkbot-0.0.7/site/NextcloudTalkExtractor/index.html`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/NextcloudUser/index.html` & `nextcloudtalkbot-0.0.7/site/NextcloudUser/index.html`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/css/theme.css` & `nextcloudtalkbot-0.0.7/site/css/theme.css`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/css/theme_extra.css` & `nextcloudtalkbot-0.0.7/site/css/theme_extra.css`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/css/fonts/Roboto-Slab-Bold.woff` & `nextcloudtalkbot-0.0.7/site/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/css/fonts/Roboto-Slab-Bold.woff2` & `nextcloudtalkbot-0.0.7/site/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/css/fonts/Roboto-Slab-Regular.woff` & `nextcloudtalkbot-0.0.7/site/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/css/fonts/Roboto-Slab-Regular.woff2` & `nextcloudtalkbot-0.0.7/site/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/css/fonts/fontawesome-webfont.eot` & `nextcloudtalkbot-0.0.7/site/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/css/fonts/fontawesome-webfont.svg` & `nextcloudtalkbot-0.0.7/site/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/css/fonts/fontawesome-webfont.ttf` & `nextcloudtalkbot-0.0.7/site/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/css/fonts/fontawesome-webfont.woff` & `nextcloudtalkbot-0.0.7/site/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/css/fonts/fontawesome-webfont.woff2` & `nextcloudtalkbot-0.0.7/site/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/css/fonts/lato-bold-italic.woff` & `nextcloudtalkbot-0.0.7/site/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/css/fonts/lato-bold-italic.woff2` & `nextcloudtalkbot-0.0.7/site/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/css/fonts/lato-bold.woff` & `nextcloudtalkbot-0.0.7/site/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/css/fonts/lato-bold.woff2` & `nextcloudtalkbot-0.0.7/site/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/css/fonts/lato-normal-italic.woff` & `nextcloudtalkbot-0.0.7/site/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/css/fonts/lato-normal-italic.woff2` & `nextcloudtalkbot-0.0.7/site/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/css/fonts/lato-normal.woff` & `nextcloudtalkbot-0.0.7/site/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/css/fonts/lato-normal.woff2` & `nextcloudtalkbot-0.0.7/site/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/img/favicon.ico` & `nextcloudtalkbot-0.0.7/site/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/js/html5shiv.min.js` & `nextcloudtalkbot-0.0.7/site/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/js/jquery-3.6.0.min.js` & `nextcloudtalkbot-0.0.7/site/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/js/theme.js` & `nextcloudtalkbot-0.0.7/site/js/theme.js`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/search/lunr.js` & `nextcloudtalkbot-0.0.7/site/search/lunr.js`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/search/main.js` & `nextcloudtalkbot-0.0.7/site/search/main.js`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/search/search_index.json` & `nextcloudtalkbot-0.0.7/site/search/search_index.json`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/site/search/worker.js` & `nextcloudtalkbot-0.0.7/site/search/worker.js`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/tests/test_encrypt_password` & `nextcloudtalkbot-0.0.7/tests/test_encrypt_password`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/LICENSE` & `nextcloudtalkbot-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/README.md` & `nextcloudtalkbot-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.6/pyproject.toml` & `nextcloudtalkbot-0.0.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nextcloudtalkbot"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Massoud Ahmed", email="okko@okxo.de", homepage="https://okxo.de"},
 ]
 homepage = "https://okxo.de"
 description = "Python3 library for creating a Nextcloud Talk bot."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `nextcloudtalkbot-0.0.6/PKG-INFO` & `nextcloudtalkbot-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcloudtalkbot
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python3 library for creating a Nextcloud Talk bot.
 Project-URL: Homepage, https://github.com/sowoi/nextcloud-talk-bot
 Project-URL: Bug Tracker, https://github.com/sowoi/nextcloud-talk-bot/issues
 Project-URL: Documentation, https://nextcloud-talk-bot.readthedocs.io
 Author-email: Massoud Ahmed <okko@okxo.de>
 License-File: LICENSE
 Keywords: bot,nextcloud,nextcloud talk
```

