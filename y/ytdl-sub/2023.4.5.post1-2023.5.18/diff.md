# Comparing `tmp/ytdl-sub-2023.4.5.post1.tar.gz` & `tmp/ytdl-sub-2023.5.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl-sub-2023.4.5.post1.tar", last modified: Wed Apr  5 19:43:38 2023, max compression
+gzip compressed data, was "ytdl-sub-2023.5.18.tar", last modified: Thu May 18 05:35:02 2023, max compression
```

## Comparing `ytdl-sub-2023.4.5.post1.tar` & `ytdl-sub-2023.5.18.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.071415 ytdl-sub-2023.4.5.post1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-04-05 19:43:38.071415 ytdl-sub-2023.4.5.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-05 19:43:38.071415 ytdl-sub-2023.4.5.post1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.055415 ytdl-sub-2023.4.5.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.059414 ytdl-sub-2023.4.5.post1/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-05 19:43:22.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.059414 ytdl-sub-2023.4.5.post1/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/cli/download_args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/cli/main_args_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.059414 ytdl-sub-2023.4.5.post1/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/config/preset_class_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12656 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.059414 ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/base_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.059414 ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.063415 ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21203 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/url/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/url/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.063415 ytdl-sub-2023.4.5.post1/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.063415 ytdl-sub-2023.4.5.post1/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19114 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/entries/variables/entry_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/entries/variables/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.063415 ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/file_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.063415 ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.063415 ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.063415 ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.063415 ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.067415 ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.067415 ytdl-sub-2023.4.5.post1/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.067415 ytdl-sub-2023.4.5.post1/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.067415 ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.071415 ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.071415 ytdl-sub-2023.4.5.post1/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-04-05 19:43:21.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:43:38.059414 ytdl-sub-2023.4.5.post1/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-04-05 19:43:38.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-05 19:43:38.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 19:43:38.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-05 19:43:38.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-05 19:43:38.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-05 19:43:38.000000 ytdl-sub-2023.4.5.post1/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.277402 ytdl-sub-2023.5.18/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-05-18 05:35:02.277402 ytdl-sub-2023.5.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-18 05:35:02.277402 ytdl-sub-2023.5.18/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.253402 ytdl-sub-2023.5.18/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.257402 ytdl-sub-2023.5.18/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.257402 ytdl-sub-2023.5.18/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/cli/download_args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/cli/main_args_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.261402 ytdl-sub-2023.5.18/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/config/preset_class_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.261402 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/base_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.261402 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.261402 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21203 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.265402 ytdl-sub-2023.5.18/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.265402 ytdl-sub-2023.5.18/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19114 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/entries/variables/entry_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/entries/variables/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.269402 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/file_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.269402 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.269402 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.269402 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.269402 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.269402 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.269402 ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.269402 ytdl-sub-2023.5.18/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.273402 ytdl-sub-2023.5.18/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.277402 ytdl-sub-2023.5.18/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.277402 ytdl-sub-2023.5.18/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.257402 ytdl-sub-2023.5.18/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-05-18 05:35:02.000000 ytdl-sub-2023.5.18/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-18 05:35:02.000000 ytdl-sub-2023.5.18/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 05:35:02.000000 ytdl-sub-2023.5.18/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-18 05:35:02.000000 ytdl-sub-2023.5.18/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-18 05:35:02.000000 ytdl-sub-2023.5.18/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 05:35:02.000000 ytdl-sub-2023.5.18/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl-sub-2023.4.5.post1/LICENSE` & `ytdl-sub-2023.5.18/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/PKG-INFO` & `ytdl-sub-2023.5.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.4.5.post1
+Version: 2023.5.18
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.4.5.post1/README.md` & `ytdl-sub-2023.5.18/README.md`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/pyproject.toml` & `ytdl-sub-2023.5.18/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/setup.cfg` & `ytdl-sub-2023.5.18/setup.cfg`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/cli/download_args_parser.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/cli/download_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/cli/main.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/cli/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/cli/main_args_parser.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/cli/main_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/config/config_file.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/config/config_validator.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/config/preset.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/config/preset.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/config/preset_class_mappings.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/config/preset_class_mappings.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/config/preset_options.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/config/preset_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,17 +106,53 @@
                        - "en"
 
 
     where each key is a ytdl argument. Include in the example are some popular ytdl_options.
     """
 
 
+class OverridesVariables(DictFormatterValidator):
+    """
+    Override variables that are automatically added to every subscription.
+    """
+
+    def _add_override_variable(self, key_name: str, format_string: str, sanitize: bool = False):
+        if sanitize:
+            key_name = f"{key_name}_sanitized"
+            format_string = sanitize_filename(format_string)
+
+        self._value[key_name] = StringFormatterValidator(
+            name="__should_never_fail__",
+            value=format_string,
+        )
+
+    def __init__(self, name, value):
+        super().__init__(name, value)
+
+        # Add sanitized and non-sanitized override variables
+        for sanitize in [True, False]:
+            self._add_override_variable(
+                key_name="subscription_name",
+                format_string=self.subscription_name,
+                sanitize=sanitize,
+            )
+
+    @property
+    def subscription_name(self) -> str:
+        """
+        Returns
+        -------
+        Name of the subscription
+        """
+        return self._root_name
+
+
 # Disable for proper docstring formatting
 # pylint: disable=line-too-long
-class Overrides(DictFormatterValidator):
+class Overrides(OverridesVariables):
     """
     Optional. This section allows you to define variables that can be used in any string formatter.
     For example, if you want your file and thumbnail files to match without copy-pasting a large
     format string, you can define something like:
 
     .. code-block:: yaml
 
@@ -138,24 +174,14 @@
     In addition, any override variable defined will automatically create a ``sanitized`` variable
     for use. In the example above, ``output_directory_sanitized`` will exist and perform
     sanitization on the value when used.
     """
 
     # pylint: enable=line-too-long
 
-    def _add_override_variable(self, key_name: str, format_string: str, sanitize: bool = False):
-        if sanitize:
-            key_name = f"{key_name}_sanitized"
-            format_string = sanitize_filename(format_string)
-
-        self._value[key_name] = StringFormatterValidator(
-            name="__should_never_fail__",
-            value=format_string,
-        )
-
     def __init__(self, name, value):
         super().__init__(name, value)
 
         # Add sanitized overrides
         for key in self._keys:
             self._add_override_variable(
                 key_name=key,
```

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/base_downloader.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/base_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/url/multi_url.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/multi_url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/url/url.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/url/validators.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/entries/base_entry.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/entries/base_entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/entries/entry.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/entries/entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/entries/entry_parent.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/entries/entry_parent.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/entries/variables/entry_variables.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/entries/variables/entry_variables.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/entries/variables/kwargs.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/entries/variables/kwargs.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 
 COLLECTION_URL = _("collection_url", backend=True)
 DOWNLOAD_INDEX = _("download_index", backend=True)
 UPLOAD_DATE_INDEX = _("upload_date_index", backend=True)
 REQUESTED_SUBTITLES = _("requested_subtitles", backend=True)
 CHAPTERS = _("chapters", backend=True)
 YTDL_SUB_CUSTOM_CHAPTERS = _("ytdl_sub_custom_chapters", backend=True)
+YTDL_SUB_REGEX_SOURCE_VARS = _("ytdl_sub_regex_source_vars", backend=True)
 SPONSORBLOCK_CHAPTERS = _("sponsorblock_chapters", backend=True)
 SPLIT_BY_CHAPTERS_PARENT_ENTRY = _("split_by_chapters_parent_entry", backend=True)
 COMMENTS = _("comments", backend=True)
 UID = _("id")
 EXTRACTOR = _("extractor")
 IE_KEY = _("ie_key")
 EPOCH = _("epoch")
```

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/main.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/audio_extract.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/audio_extract.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/chapters.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/chapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,29 +298,32 @@
 
         Returns
         -------
         entry
         """
         chapters = Chapters.from_empty()
 
+        # If there are no embedded chapters, and comment chapters are allowed...
         if not _contains_any_chapters(entry) and self.plugin_options.allow_chapters_from_comments:
+            # Try to get chapters from comments
             for comment in entry.kwargs_get(COMMENTS, []):
                 chapters = Chapters.from_string(comment.get("text", ""))
-                if not chapters.is_empty():
+                if chapters.contains_any_chapters():
                     break
 
-        if not chapters.is_empty():
-            entry.add_kwargs({YTDL_SUB_CUSTOM_CHAPTERS: chapters.to_file_metadata_dict()})
-
-            if not self.is_dry_run:
-                set_ffmpeg_metadata_chapters(
-                    file_path=entry.get_download_file_path(),
-                    chapters=chapters,
-                    file_duration_sec=entry.kwargs("duration"),
-                )
+            # If some are actually found, add a special kwarg and embed them
+            if chapters.contains_any_chapters():
+                entry.add_kwargs({YTDL_SUB_CUSTOM_CHAPTERS: chapters.to_file_metadata_dict()})
+
+                if not self.is_dry_run:
+                    set_ffmpeg_metadata_chapters(
+                        file_path=entry.get_download_file_path(),
+                        chapters=chapters,
+                        file_duration_sec=entry.kwargs("duration"),
+                    )
 
         return entry
 
     def post_process_entry(self, entry: Entry) -> Optional[FileMetadata]:
         """
         Parameters
         ----------
```

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/date_range.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/date_range.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/file_convert.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/file_convert.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/internal/view.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/internal/view.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/match_filters.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/match_filters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/music_tags.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/music_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/plugin.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/regex.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/regex.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from yt_dlp.utils import sanitize_filename
 
 from ytdl_sub.entries.entry import Entry
+from ytdl_sub.entries.variables.kwargs import YTDL_SUB_REGEX_SOURCE_VARS
 from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.plugins.plugin import PluginOptions
 from ytdl_sub.plugins.plugin import PluginPriority
 from ytdl_sub.utils.exceptions import RegexNoMatchException
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.validators.regex_validator import RegexListValidator
 from ytdl_sub.validators.source_variable_validator import SourceVariableNameListValidator
@@ -241,34 +242,60 @@
 
 class RegexPlugin(Plugin[RegexOptions]):
     plugin_options_type = RegexOptions
     priority = PluginPriority(
         modify_entry=PluginPriority.MODIFY_ENTRY_AFTER_SPLIT + 0,
     )
 
-    def modify_entry(self, entry: Entry) -> Optional[Entry]:
+    @classmethod
+    def _add_processed_regex_source_var(cls, entry: Entry, source_var: str) -> None:
+        if not entry.kwargs_contains(YTDL_SUB_REGEX_SOURCE_VARS):
+            entry.add_kwargs({YTDL_SUB_REGEX_SOURCE_VARS: []})
+
+        entry.kwargs(YTDL_SUB_REGEX_SOURCE_VARS).append(source_var)
+
+    @classmethod
+    def _contains_processed_regex_source_var(cls, entry: Entry, source_var: str) -> bool:
+        return source_var in entry.kwargs_get(YTDL_SUB_REGEX_SOURCE_VARS, [])
+
+    def _modify_entry_metadata(self, entry: Entry, is_metadata_stage: bool) -> Optional[Entry]:
         """
         Parameters
         ----------
         entry
             Entry to add source variables to
+        is_metadata_stage
+            Whether this is called at the metadata stage or modify stage
 
         Returns
         -------
         Entry with regex capture variables added to its source variables
 
         Raises
         ------
         ValidationException
             If no capture and no defaults
         """
         entry_variable_dict = entry.to_dict()
 
         # Iterate each source var to capture and add to the entry
         for source_var, regex_options in self.plugin_options.source_variable_capture_dict.items():
+
+            # Record which regex source variables are processed, to
+            # process as many variables as possible in the metadata stage, then the rest
+            # after the media file has been downloaded.
+            if self._contains_processed_regex_source_var(entry, source_var):
+                continue
+
+            # Continue if the source var isn't in the dict since entry variables could be added
+            # after the metadata stage
+            if is_metadata_stage and source_var not in entry_variable_dict:
+                continue
+
+            self._add_processed_regex_source_var(entry, source_var)
             maybe_capture = regex_options.match.match_any(input_str=entry_variable_dict[source_var])
 
             # If no capture
             if maybe_capture is None:
                 # and no defaults
                 if not regex_options.has_defaults:
                     # Skip the entry if toggled
@@ -327,7 +354,19 @@
                             capture
                         )
                         for i, capture in enumerate(maybe_capture)
                     },
                 )
 
         return entry
+
+    def modify_entry_metadata(self, entry: Entry) -> Optional[Entry]:
+        """
+        Perform regex at the metadata stage
+        """
+        return self._modify_entry_metadata(entry, is_metadata_stage=True)
+
+    def modify_entry(self, entry: Entry) -> Optional[Entry]:
+        """
+        Perform regex at the metadata stage
+        """
+        return self._modify_entry_metadata(entry, is_metadata_stage=False)
```

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,22 +160,15 @@
         return entry, metadata
 
     def split(self, entry: Entry) -> Optional[List[Tuple[Entry, FileMetadata]]]:
         """
         Tags the entry's audio file using values defined in the metadata options
         """
         split_videos_and_metadata: List[Tuple[Entry, FileMetadata]] = []
-
-        if self.is_dry_run:
-            chapters = Chapters.from_entry_chapters(entry=entry)
-        else:
-            chapters = Chapters.from_embedded_chapters(
-                ffprobe_path=FFMPEG.ffprobe_path(),
-                file_path=entry.get_download_file_path(),
-            )
+        chapters = Chapters.from_entry_chapters(entry=entry)
 
         # If no chapters, do not split anything
         if not chapters.contains_any_chapters():
             if self.plugin_options.when_no_chapters == "pass":
                 entry.add_variables(
                     {
                         "chapter_title": entry.title,
```

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/subtitles.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/subtitles.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/plugins/video_tags.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/video_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/helpers/__init__.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 presets:
 
-  _plex_tv_show:
+
+  _plex_tv_show: # Default Highest Resolution, No AV1, which is not currently supported by plex
     preset:
       - "_plex_base"
       - "_episode_base"
       - "_episode_video_tags"
     ytdl_options:
-      format: "bestvideo[ext=mp4]+bestaudio[ext=m4a]/best[ext=mp4]/best"
+      format: "(bv*[ext=mp4][vcodec~='^((he|a)vc|h26[45])']+ba[ext=m4a]) / (bv[ext=mp4]*+ba[ext=m4a]/b)"
     overrides:
       tv_show_poster_file_name: "poster.jpg"
       tv_show_fanart_file_name: "fanart.jpg"
       season_poster_file_name: "Season {season_number_padded}/Season{season_number_padded}.jpg"
-    file_convert:  # Plex currently does not support webm
-      convert_to: "mp4"
 
   _jellyfin_tv_show:
     preset:
       - "_base"
       - "_episode_base"
       - "_episode_video_tags"
       - "_episode_nfo_tags"
```

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/subscriptions/subscription.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/chapters.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/utils/chapters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import json
 import re
-import subprocess
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 from ytdl_sub.entries.entry import Entry
+from ytdl_sub.entries.variables.kwargs import CHAPTERS
+from ytdl_sub.entries.variables.kwargs import YTDL_SUB_CUSTOM_CHAPTERS
 from ytdl_sub.utils.file_handler import FileMetadata
 
 
 class Timestamp:
 
     # Captures the following formats:
     # 0:00 title
@@ -198,70 +198,30 @@
         -------
         Chapters
             Could be empty
         """
         timestamps: List[Timestamp] = []
         titles: List[str] = []
 
+        # Try to accumulate chapters by parsing lines individually
         for line in input_str.split("\n"):
             # Timestamp captured, store it
             if match := Timestamp.TIMESTAMP_REGEX.search(line):
                 timestamp_str = match.group(1)
                 timestamps.append(Timestamp.from_str(timestamp_str))
 
                 # Remove timestamp and surrounding whitespace from it
                 title_str = re.sub(f"\\s*{re.escape(timestamp_str)}\\s*", " ", line).strip()
                 titles.append(title_str)
-            elif len(timestamps) >= 3:
-                return Chapters(timestamps=timestamps, titles=titles)
-            # Timestamp was not stored, if only contained 1, reset
-            else:
-                timestamps = []
-                titles = []
 
-        return Chapters(timestamps=timestamps, titles=titles)
-
-    @classmethod
-    def from_embedded_chapters(cls, ffprobe_path: str, file_path: str) -> "Chapters":
-        """
-        Parameters
-        ----------
-        ffprobe_path
-            Path to ffprobe executable
-        file_path
-            File to read ffmpeg chapter metadata from
-
-        Returns
-        -------
-        Chapters object
-        """
-        proc = subprocess.run(
-            [
-                ffprobe_path,
-                "-loglevel",
-                "quiet",
-                "-print_format",
-                "json",
-                "-show_chapters",
-                "--",
-                file_path,
-            ],
-            check=True,
-            stdout=subprocess.PIPE,
-            encoding="utf-8",
-        )
-
-        embedded_chapters = json.loads(proc.stdout)
-        timestamps: List[Timestamp] = []
-        titles: List[str] = []
-        for chapter in embedded_chapters["chapters"]:
-            timestamps.append(Timestamp.from_seconds(int(float(chapter["start_time"]))))
-            titles.append(chapter["tags"]["title"])
-
-        return Chapters(timestamps=timestamps, titles=titles)
+        # If more than 3 timestamps were parsed, return it
+        if len(timestamps) >= 3:
+            return Chapters(timestamps=timestamps, titles=titles)
+        # Otherwise return empty chapters
+        return Chapters(timestamps=[], titles=[])
 
     @classmethod
     def from_entry_chapters(cls, entry: Entry) -> "Chapters":
         """
         Parameters
         ----------
         entry
@@ -270,21 +230,22 @@
         Returns
         -------
         Chapters object
         """
         timestamps: List[Timestamp] = []
         titles: List[str] = []
 
-        chapters = {}
-        if entry.kwargs_contains("chapters"):
-            chapters = entry.kwargs("chapters") or []
-
-        for chapter in chapters:
-            timestamps.append(Timestamp.from_seconds(int(float(chapter["start_time"]))))
-            titles.append(chapter["title"])
+        if entry.kwargs_contains(CHAPTERS):
+            for chapter in entry.kwargs_get(CHAPTERS, []):
+                timestamps.append(Timestamp.from_seconds(int(float(chapter["start_time"]))))
+                titles.append(chapter["title"])
+        elif entry.kwargs_contains(YTDL_SUB_CUSTOM_CHAPTERS):
+            for start_time, title in entry.kwargs_get(YTDL_SUB_CUSTOM_CHAPTERS, {}).items():
+                timestamps.append(Timestamp.from_str(start_time))
+                titles.append(title)
 
         return Chapters(timestamps=timestamps, titles=titles)
 
     @classmethod
     def from_empty(cls) -> "Chapters":
         """
         Initialize empty chapters
```

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/datetime.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/exceptions.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/ffmpeg.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/file_handler.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/file_lock.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/logger.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/retry.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/utils/retry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/thumbnail.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/xml.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/utils/yaml.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/file_path_validators.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/nfo_validators.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/regex_validator.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/string_datetime.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/string_select_validator.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/validators/validators.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/validators/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,14 +177,24 @@
 
     def __init__(self, name, value):
         super().__init__(name, value)
         self.__validator_dict: Dict[str, Validator] = {}
 
     @final
     @property
+    def _root_name(self) -> str:
+        """
+        Returns
+        -------
+        "first" from the first.element.of.the.name
+        """
+        return self._name.split(".")[0]
+
+    @final
+    @property
     def _dict(self) -> dict:
         """
         Returns
         -------
         Dictionary value
         """
         return self._value
```

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl-sub-2023.5.18/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub.egg-info/PKG-INFO` & `ytdl-sub-2023.5.18/src/ytdl_sub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.4.5.post1
+Version: 2023.5.18
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.4.5.post1/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl-sub-2023.5.18/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

