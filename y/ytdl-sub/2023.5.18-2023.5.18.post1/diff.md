# Comparing `tmp/ytdl-sub-2023.5.18.tar.gz` & `tmp/ytdl-sub-2023.5.18.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl-sub-2023.5.18.tar", last modified: Thu May 18 05:35:02 2023, max compression
+gzip compressed data, was "ytdl-sub-2023.5.18.post1.tar", last modified: Thu May 18 16:53:39 2023, max compression
```

## Comparing `ytdl-sub-2023.5.18.tar` & `ytdl-sub-2023.5.18.post1.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.277402 ytdl-sub-2023.5.18/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-05-18 05:35:02.277402 ytdl-sub-2023.5.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-18 05:35:02.277402 ytdl-sub-2023.5.18/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.253402 ytdl-sub-2023.5.18/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.257402 ytdl-sub-2023.5.18/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.257402 ytdl-sub-2023.5.18/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/cli/download_args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/cli/main_args_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.261402 ytdl-sub-2023.5.18/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/config/preset_class_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.261402 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/base_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.261402 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.261402 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21203 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.265402 ytdl-sub-2023.5.18/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.265402 ytdl-sub-2023.5.18/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19114 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/entries/variables/entry_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/entries/variables/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.269402 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/file_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.269402 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.269402 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.269402 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.269402 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.269402 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.269402 ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.269402 ytdl-sub-2023.5.18/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.273402 ytdl-sub-2023.5.18/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.277402 ytdl-sub-2023.5.18/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.277402 ytdl-sub-2023.5.18/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-05-18 05:34:42.000000 ytdl-sub-2023.5.18/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:35:02.257402 ytdl-sub-2023.5.18/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-05-18 05:35:02.000000 ytdl-sub-2023.5.18/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-18 05:35:02.000000 ytdl-sub-2023.5.18/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 05:35:02.000000 ytdl-sub-2023.5.18/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-18 05:35:02.000000 ytdl-sub-2023.5.18/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-18 05:35:02.000000 ytdl-sub-2023.5.18/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 05:35:02.000000 ytdl-sub-2023.5.18/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.091501 ytdl-sub-2023.5.18.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-05-18 16:53:39.091501 ytdl-sub-2023.5.18.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-18 16:53:39.095502 ytdl-sub-2023.5.18.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.075500 ytdl-sub-2023.5.18.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.079501 ytdl-sub-2023.5.18.post1/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.079501 ytdl-sub-2023.5.18.post1/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/cli/download_args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/cli/main_args_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.079501 ytdl-sub-2023.5.18.post1/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/config/preset_class_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.083501 ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/base_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.083501 ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.083501 ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21911 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/url/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/url/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.083501 ytdl-sub-2023.5.18.post1/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.083501 ytdl-sub-2023.5.18.post1/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19114 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/entries/variables/entry_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/entries/variables/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.087501 ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/file_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.087501 ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.087501 ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.087501 ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.087501 ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.087501 ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.087501 ytdl-sub-2023.5.18.post1/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.087501 ytdl-sub-2023.5.18.post1/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.091501 ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.091501 ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.091501 ytdl-sub-2023.5.18.post1/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-05-18 16:53:20.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:53:39.079501 ytdl-sub-2023.5.18.post1/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-05-18 16:53:39.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-18 16:53:39.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 16:53:39.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-18 16:53:39.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-18 16:53:39.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 16:53:39.000000 ytdl-sub-2023.5.18.post1/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl-sub-2023.5.18/LICENSE` & `ytdl-sub-2023.5.18.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/PKG-INFO` & `ytdl-sub-2023.5.18.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.5.18
+Version: 2023.5.18.post1
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.5.18/README.md` & `ytdl-sub-2023.5.18.post1/README.md`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/pyproject.toml` & `ytdl-sub-2023.5.18.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/setup.cfg` & `ytdl-sub-2023.5.18.post1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/cli/download_args_parser.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/cli/download_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/cli/main.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/cli/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/cli/main_args_parser.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/cli/main_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/config/config_file.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/config/config_validator.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/config/preset.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/config/preset.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/config/preset_class_mappings.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/config/preset_class_mappings.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/config/preset_options.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/config/preset_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/base_downloader.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/base_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from typing import Iterable
 from typing import Iterator
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Tuple
 
+from yt_dlp.utils import RejectedVideoReached
+
 from ytdl_sub.config.preset_options import Overrides
 from ytdl_sub.downloaders.base_downloader import BaseDownloader
 from ytdl_sub.downloaders.base_downloader import BaseDownloaderOptionsT
 from ytdl_sub.downloaders.base_downloader import BaseDownloaderPlugin
 from ytdl_sub.downloaders.base_downloader import BaseDownloaderValidator
 from ytdl_sub.downloaders.url.validators import MultiUrlValidator
 from ytdl_sub.downloaders.url.validators import UrlThumbnailListValidator
@@ -27,14 +29,15 @@
 from ytdl_sub.entries.variables.kwargs import COMMENTS
 from ytdl_sub.entries.variables.kwargs import DOWNLOAD_INDEX
 from ytdl_sub.entries.variables.kwargs import PLAYLIST_ENTRY
 from ytdl_sub.entries.variables.kwargs import REQUESTED_SUBTITLES
 from ytdl_sub.entries.variables.kwargs import SOURCE_ENTRY
 from ytdl_sub.entries.variables.kwargs import SPONSORBLOCK_CHAPTERS
 from ytdl_sub.entries.variables.kwargs import UPLOAD_DATE_INDEX
+from ytdl_sub.entries.variables.kwargs import YTDL_SUB_MATCH_FILTER_REJECT
 from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.utils.thumbnail import ThumbnailTypes
 from ytdl_sub.utils.thumbnail import convert_download_thumbnail
 from ytdl_sub.utils.thumbnail import download_and_convert_url_thumbnail
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
@@ -519,22 +522,37 @@
         ----------
         entry
             Entry to download
 
         Returns
         -------
         The entry that was downloaded successfully
+
+        Raises
+        ------
+        RejectedVideoReached
+          If a video was rejected and was not from match_filter
         """
         download_logger.info(
             "Downloading entry %d/%d: %s",
             self._url_state.entries_downloaded,
             self._url_state.entries_total,
             entry.title,
         )
-        download_entry = self._extract_entry_info_with_retry(entry=entry)
+
+        # Match-filters are applied at the download stage (not metadata stage).
+        # If the download is rejected, and match_filter is present in the ytdl options,
+        # then filter downstream in the match_filter plugin
+        try:
+            download_entry = self._extract_entry_info_with_retry(entry=entry)
+        except RejectedVideoReached:
+            if "match_filter" in self.download_ytdl_options:
+                entry.add_kwargs({YTDL_SUB_MATCH_FILTER_REJECT: True})
+                return entry
+            raise
 
         upload_date_idx = self._enhanced_download_archive.mapping.get_num_entries_with_upload_date(
             upload_date_standardized=entry.upload_date_standardized
         )
         download_idx = self._enhanced_download_archive.num_entries
 
         entry.add_kwargs(
```

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/multi_url.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/url/multi_url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/url.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/url/url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/url/validators.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/url/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/entries/base_entry.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/entries/base_entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/entries/entry.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/entries/entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/entries/entry_parent.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/entries/entry_parent.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/entries/variables/entry_variables.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/entries/variables/entry_variables.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/entries/variables/kwargs.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/entries/variables/kwargs.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 COLLECTION_URL = _("collection_url", backend=True)
 DOWNLOAD_INDEX = _("download_index", backend=True)
 UPLOAD_DATE_INDEX = _("upload_date_index", backend=True)
 REQUESTED_SUBTITLES = _("requested_subtitles", backend=True)
 CHAPTERS = _("chapters", backend=True)
 YTDL_SUB_CUSTOM_CHAPTERS = _("ytdl_sub_custom_chapters", backend=True)
 YTDL_SUB_REGEX_SOURCE_VARS = _("ytdl_sub_regex_source_vars", backend=True)
+YTDL_SUB_MATCH_FILTER_REJECT = _("ytdl_sub_match_filter_reject", backend=True)
 SPONSORBLOCK_CHAPTERS = _("sponsorblock_chapters", backend=True)
 SPLIT_BY_CHAPTERS_PARENT_ENTRY = _("split_by_chapters_parent_entry", backend=True)
 COMMENTS = _("comments", backend=True)
 UID = _("id")
 EXTRACTOR = _("extractor")
 IE_KEY = _("ie_key")
 EPOCH = _("epoch")
```

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/main.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/audio_extract.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/audio_extract.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/chapters.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/date_range.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/date_range.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/file_convert.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/file_convert.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/internal/view.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/internal/view.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/match_filters.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/match_filters.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from yt_dlp import match_filter_func
 
+from ytdl_sub.entries.entry import Entry
+from ytdl_sub.entries.variables.kwargs import YTDL_SUB_MATCH_FILTER_REJECT
 from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.plugins.plugin import PluginOptions
+from ytdl_sub.plugins.plugin import PluginPriority
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.validators.validators import StringListValidator
 
 logger = Logger.get("match_filters")
 
 
 class MatchFiltersOptions(PluginOptions):
@@ -59,20 +62,34 @@
         conditions are met.
         """
         return [validator.value for validator in self._filters]
 
 
 class MatchFiltersPlugin(Plugin[MatchFiltersOptions]):
     plugin_options_type = MatchFiltersOptions
+    priority = PluginPriority(modify_entry=PluginPriority.MODIFY_ENTRY_FIRST)
 
     def ytdl_options(self) -> Optional[Dict]:
         """
         Returns
         -------
         match_filter after calling the utility function for it
         """
         match_filters: List[str] = []
         for filter_str in self.plugin_options.filters:
             logger.debug("Adding match-filter %s", filter_str)
             match_filters.append(filter_str)
 
-        return {"match_filter": match_filter_func(match_filters)}
+        return {
+            "match_filter": match_filter_func(match_filters),
+        }
+
+    def modify_entry(self, entry: Entry) -> Optional[Entry]:
+        """
+        If an entry is marked as not being downloaded due to a match_filter reject,
+        do not propagate the entry further (especially since there is no entry file!)
+        """
+        if entry.kwargs_get(YTDL_SUB_MATCH_FILTER_REJECT, False):
+            logger.info("Entry rejected by match-filter, skipping ..")
+            return None
+
+        return entry
```

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/music_tags.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/music_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/plugin.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,17 @@
     """
     Defines priority for plugins, 0 is highest priority
     """
 
     # If modify_entry priority is >= to this value, run after split
     MODIFY_ENTRY_AFTER_SPLIT = 10
 
-    def __init__(self, modify_entry: int = 0, post_process: int = 0):
+    MODIFY_ENTRY_FIRST = 0
+
+    def __init__(self, modify_entry: int = 5, post_process: int = 5):
         self.modify_entry = modify_entry
         self.post_process = post_process
 
     @property
     def modify_entry_after_split(self) -> bool:
         """
         Returns
```

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/regex.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/subtitles.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/subtitles.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/plugins/video_tags.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/plugins/video_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/helpers/__init__.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/subscription.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,18 @@
         return {
             "skip_download": True,
             "writethumbnail": False,
             "writeinfojson": True,
         }
 
     @property
+    def _download_only_options(self) -> Dict:
+        return {"break_on_reject": True}
+
+    @property
     def _output_options(self) -> Dict:
         ytdl_options = {}
 
         if self._preset.output_options.maintain_download_archive:
             ytdl_options["download_archive"] = str(
                 Path(self._working_directory) / self._enhanced_download_archive.archive_file_name
             )
@@ -106,34 +110,34 @@
         YTDLOptionsBuilder
             Builder with values set for fetching metadata (.info.json) only
         """
         return YTDLOptionsBuilder().add(
             self._global_options,
             self._output_options,
             self._plugin_ytdl_options(DateRangePlugin),
-            self._plugin_ytdl_options(MatchFiltersPlugin),
             self._user_ytdl_options,  # user ytdl options...
             self._info_json_only_options,  # then info_json_only options
         )
 
     def download_builder(self) -> YTDLOptionsBuilder:
         """
         Returns
         -------
         YTDLOptionsBuilder
             Builder with values set based on the subscription for actual downloading
         """
         ytdl_options_builder = YTDLOptionsBuilder().add(
             self._global_options,
             self._output_options,
-            self._plugin_ytdl_options(DateRangePlugin),
+            self._plugin_ytdl_options(MatchFiltersPlugin),
             self._plugin_ytdl_options(FileConvertPlugin),
             self._plugin_ytdl_options(SubtitlesPlugin),
             self._plugin_ytdl_options(ChaptersPlugin),
             self._plugin_ytdl_options(AudioExtractPlugin),
             self._user_ytdl_options,  # user ytdl options...
+            self._download_only_options,  # then download_only options
         )
         # Add dry run options last if enabled
         if self._dry_run:
             ytdl_options_builder.add(self._dry_run_options)
 
         return ytdl_options_builder
```

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/utils/chapters.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/utils/datetime.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/utils/exceptions.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/utils/ffmpeg.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/utils/file_handler.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/utils/file_lock.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/utils/logger.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/utils/retry.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/retry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/utils/thumbnail.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/utils/xml.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/utils/yaml.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/validators/file_path_validators.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/validators/nfo_validators.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/validators/regex_validator.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/validators/string_datetime.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/validators/string_select_validator.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/validators/validators.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/validators/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub.egg-info/PKG-INFO` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.5.18
+Version: 2023.5.18.post1
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.5.18/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl-sub-2023.5.18.post1/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

