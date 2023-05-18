# Comparing `tmp/TPEduBot-0.5.6.tar.gz` & `tmp/TPEduBot-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TPEduBot-0.5.6.tar", last modified: Thu May 18 04:19:41 2023, max compression
+gzip compressed data, was "TPEduBot-0.5.7.tar", last modified: Thu May 18 05:20:12 2023, max compression
```

## Comparing `TPEduBot-0.5.6.tar` & `TPEduBot-0.5.7.tar`

### file list

```diff
@@ -1,129 +1,126 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 04:19:41.062750 TPEduBot-0.5.6/
--rw-rw-rw-   0        0        0      242 2023-05-18 04:19:41.059694 TPEduBot-0.5.6/PKG-INFO
--rw-rw-rw-   0        0        0      723 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 04:19:39.336938 TPEduBot-0.5.6/TPEduBot.egg-info/
--rw-rw-rw-   0        0        0      242 2023-05-18 04:19:39.000000 TPEduBot-0.5.6/TPEduBot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6176 2023-05-18 04:19:39.000000 TPEduBot-0.5.6/TPEduBot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 04:19:39.000000 TPEduBot-0.5.6/TPEduBot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-18 04:19:39.000000 TPEduBot-0.5.6/TPEduBot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 04:19:39.615384 TPEduBot-0.5.6/buildABot/
--rw-rw-rw-   0        0        0    40255 2023-05-17 19:55:47.000000 TPEduBot-0.5.6/buildABot/Analytics.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:19:39.617336 TPEduBot-0.5.6/buildABot/Data/
-drwxrwxrwx   0        0        0        0 2023-05-18 04:19:40.107532 TPEduBot-0.5.6/buildABot/Data/Default - Learn/
--rw-rw-rw-   0        0        0     1062 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Default Fallback Intent.json
--rw-rw-rw-   0        0        0     1096 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Default Welcome Intent - fallback.json
--rw-rw-rw-   0        0        0     3158 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Default Welcome Intent.json
--rw-rw-rw-   0        0        0      244 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Default Welcome Intent_usersays_en.json
--rw-rw-rw-   0        0        0     1131 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Downvote.json
--rw-rw-rw-   0        0        0      982 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Downvote_usersays_en.json
--rw-rw-rw-   0        0        0     3785 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Email Enquiry.json
--rw-rw-rw-   0        0        0     2453 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json
--rw-rw-rw-   0        0        0     1518 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Exit Conversation.json
--rw-rw-rw-   0        0        0     2173 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json
--rw-rw-rw-   0        0        0      682 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Fallback - Logged In - fallback.json
--rw-rw-rw-   0        0        0     1525 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Fallback - Logged In - no.json
--rw-rw-rw-   0        0        0    10929 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Fallback - Logged In - no_usersays_en.json
--rw-rw-rw-   0        0        0     1074 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Fallback - Logged In - yes.json
--rw-rw-rw-   0        0        0    10255 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Fallback - Logged In - yes_usersays_en.json
--rw-rw-rw-   0        0        0     1164 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Remember Name.json
--rw-rw-rw-   0        0        0      239 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Remember Name_usersays_en.json
--rw-rw-rw-   0        0        0     2186 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Results - Password - Correct.json
--rw-rw-rw-   0        0        0      613 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Results - Password - Correct_usersays_en.json
--rw-rw-rw-   0        0        0     1177 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback - fallback.json
--rw-rw-rw-   0        0        0     1238 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback.json
--rw-rw-rw-   0        0        0     1197 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Results - Password - fallback.json
--rw-rw-rw-   0        0        0     2257 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Results - Password.json
--rw-rw-rw-   0        0        0      752 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Results - Password_usersays_en.json
--rw-rw-rw-   0        0        0      249 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Sentiment (Awesome)_usersays_en.json
--rw-rw-rw-   0        0        0      252 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Sentiment (Doing Fine)_usersays_en.json
--rw-rw-rw-   0        0        0      264 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Sentiment (It's been a rough week)_usersays_en.json
--rw-rw-rw-   0        0        0      261 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Sentiment (Still Hanging There)_usersays_en.json
--rw-rw-rw-   0        0        0     1665 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In.json
--rw-rw-rw-   0        0        0      597 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In_usersays_en.json
--rw-rw-rw-   0        0        0     1741 2023-05-17 19:35:50.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Menu - Main.json
--rw-rw-rw-   0        0        0     2454 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Menu - Main_usersays_en.json
--rw-rw-rw-   0        0        0     1079 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Thankyou.json
--rw-rw-rw-   0        0        0     1496 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Thankyou_usersays_en.json
--rw-rw-rw-   0        0        0      891 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Upvote.json
--rw-rw-rw-   0        0        0      241 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Learn/Upvote_usersays_en.json
-drwxrwxrwx   0        0        0        0 2023-05-18 04:19:40.371742 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/
--rw-rw-rw-   0        0        0     1062 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Default Fallback Intent.json
--rw-rw-rw-   0        0        0     1096 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Default Welcome Intent - fallback.json
--rw-rw-rw-   0        0        0     3158 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Default Welcome Intent.json
--rw-rw-rw-   0        0        0      244 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Default Welcome Intent_usersays_en.json
--rw-rw-rw-   0        0        0     1131 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Downvote.json
--rw-rw-rw-   0        0        0      982 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Downvote_usersays_en.json
--rw-rw-rw-   0        0        0     3785 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Email Enquiry.json
--rw-rw-rw-   0        0        0     2453 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json
--rw-rw-rw-   0        0        0     1518 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Exit Conversation.json
--rw-rw-rw-   0        0        0     2173 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json
--rw-rw-rw-   0        0        0      682 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Fallback - Logged In - fallback.json
--rw-rw-rw-   0        0        0     1525 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Fallback - Logged In - no.json
--rw-rw-rw-   0        0        0    10929 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Fallback - Logged In - no_usersays_en.json
--rw-rw-rw-   0        0        0     1074 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Fallback - Logged In - yes.json
--rw-rw-rw-   0        0        0    10255 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Fallback - Logged In - yes_usersays_en.json
--rw-rw-rw-   0        0        0     1164 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Remember Name.json
--rw-rw-rw-   0        0        0      239 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Remember Name_usersays_en.json
--rw-rw-rw-   0        0        0     2186 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct.json
--rw-rw-rw-   0        0        0      613 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct_usersays_en.json
--rw-rw-rw-   0        0        0     2219 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Results - Password - Template.json
--rw-rw-rw-   0        0        0     1177 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback - fallback.json
--rw-rw-rw-   0        0        0     1238 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback.json
--rw-rw-rw-   0        0        0     1197 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback.json
--rw-rw-rw-   0        0        0      752 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Results - Password_usersays_en.json
--rw-rw-rw-   0        0        0      249 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Sentiment (Awesome)_usersays_en.json
--rw-rw-rw-   0        0        0      252 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Sentiment (Doing Fine)_usersays_en.json
--rw-rw-rw-   0        0        0      264 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Sentiment (It's been a rough week)_usersays_en.json
--rw-rw-rw-   0        0        0      261 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Sentiment (Still Hanging There)_usersays_en.json
--rw-rw-rw-   0        0        0     1665 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In.json
--rw-rw-rw-   0        0        0      597 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In_usersays_en.json
--rw-rw-rw-   0        0        0     2076 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Menu - Main.json
--rw-rw-rw-   0        0        0     2454 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json
--rw-rw-rw-   0        0        0     1079 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Thankyou.json
--rw-rw-rw-   0        0        0     1496 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json
--rw-rw-rw-   0        0        0      891 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Upvote.json
--rw-rw-rw-   0        0        0      241 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Upvote_usersays_en.json
-drwxrwxrwx   0        0        0        0 2023-05-18 04:19:40.380544 TPEduBot-0.5.6/buildABot/Data/Entities/
--rw-rw-rw-   0        0        0      208 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Entities/LoginID.json
-drwxrwxrwx   0        0        0        0 2023-05-18 04:19:40.785730 TPEduBot-0.5.6/buildABot/Data/WebApp/
--rw-rw-rw-   0        0        0    26827 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/WebApp/index_template_LEARN.html
--rw-rw-rw-   0        0        0    21879 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/WebApp/index_template_RECO.html
--rw-rw-rw-   0        0        0   817197 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/WebApp/reset_template_RECO.js
-drwxrwxrwx   0        0        0        0 2023-05-18 04:19:40.915321 TPEduBot-0.5.6/buildABot/Data/Webhook/
--rw-rw-rw-   0        0        0     2162 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Webhook/CheckPwd_Template_RECO.js
--rw-rw-rw-   0        0        0     4597 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js
--rw-rw-rw-   0        0        0     7331 2023-05-17 19:11:48.000000 TPEduBot-0.5.6/buildABot/Data/Webhook/index_template_LEARN.js
--rw-rw-rw-   0        0        0    10693 2023-05-12 06:25:07.000000 TPEduBot-0.5.6/buildABot/Data/Webhook/index_template_RECO.js
--rw-rw-rw-   0        0        0       89 2023-05-15 04:03:04.000000 TPEduBot-0.5.6/buildABot/Data/__init__.py
--rw-rw-rw-   0        0        0    15847 2023-05-17 19:55:48.000000 TPEduBot-0.5.6/buildABot/Entities.py
--rw-rw-rw-   0        0        0    12267 2023-05-17 19:55:48.000000 TPEduBot-0.5.6/buildABot/FallbackSocialTag.py
--rw-rw-rw-   0        0        0    12103 2023-05-17 19:55:48.000000 TPEduBot-0.5.6/buildABot/Firebase_Learn.py
--rw-rw-rw-   0        0        0    14879 2023-05-17 19:55:48.000000 TPEduBot-0.5.6/buildABot/Firebase_Reco.py
--rw-rw-rw-   0        0        0    36243 2023-05-17 19:55:48.000000 TPEduBot-0.5.6/buildABot/Intents.py
--rw-rw-rw-   0        0        0    42171 2023-05-17 19:55:48.000000 TPEduBot-0.5.6/buildABot/LearnMenu.py
--rw-rw-rw-   0        0        0    77771 2023-05-18 04:18:41.000000 TPEduBot-0.5.6/buildABot/Manager.py
--rw-rw-rw-   0        0        0    15947 2023-05-17 19:55:48.000000 TPEduBot-0.5.6/buildABot/Paraphraser.py
--rw-rw-rw-   0        0        0     6151 2023-05-17 19:55:48.000000 TPEduBot-0.5.6/buildABot/Password.py
--rw-rw-rw-   0        0        0    44723 2023-05-17 19:55:48.000000 TPEduBot-0.5.6/buildABot/RecommendedMenu.py
--rw-rw-rw-   0        0        0     8791 2023-05-17 19:55:48.000000 TPEduBot-0.5.6/buildABot/TelegramLogs.py
--rw-rw-rw-   0        0        0     7539 2023-05-17 19:55:48.000000 TPEduBot-0.5.6/buildABot/WebApp_Learn.py
--rw-rw-rw-   0        0        0    11283 2023-05-17 19:55:48.000000 TPEduBot-0.5.6/buildABot/WebApp_Reco.py
--rw-rw-rw-   0        0        0     9259 2023-05-17 19:55:48.000000 TPEduBot-0.5.6/buildABot/Webhook_Learn.py
--rw-rw-rw-   0        0        0    19235 2023-05-17 19:55:48.000000 TPEduBot-0.5.6/buildABot/Webhook_Reco.py
--rw-rw-rw-   0        0        0    23915 2023-05-16 14:52:33.000000 TPEduBot-0.5.6/buildABot/Worksheets.py
--rw-rw-rw-   0        0        0    23951 2023-05-17 19:55:48.000000 TPEduBot-0.5.6/buildABot/Worksheets_Learn.py
--rw-rw-rw-   0        0        0    24123 2023-05-17 19:55:48.000000 TPEduBot-0.5.6/buildABot/Worksheets_Reco.py
--rw-rw-rw-   0        0        0     5075 2023-05-17 19:55:48.000000 TPEduBot-0.5.6/buildABot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:19:40.942693 TPEduBot-0.5.6/buildABot/pytransform/
--rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPEduBot-0.5.6/buildABot/pytransform/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:19:41.017817 TPEduBot-0.5.6/parrot/
--rw-rw-rw-   0        0        0     1219 2023-05-16 14:54:08.000000 TPEduBot-0.5.6/parrot/__init__.py
--rw-rw-rw-   0        0        0     3643 2023-05-16 14:54:08.000000 TPEduBot-0.5.6/parrot/demo.py
--rw-rw-rw-   0        0        0    25523 2023-05-16 14:54:08.000000 TPEduBot-0.5.6/parrot/filters.py
--rw-rw-rw-   0        0        0    16591 2023-05-16 14:54:08.000000 TPEduBot-0.5.6/parrot/parrot.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:19:41.036084 TPEduBot-0.5.6/parrot/pytransform/
--rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPEduBot-0.5.6/parrot/pytransform/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:19:41.056543 TPEduBot-0.5.6/pytransform/
--rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPEduBot-0.5.6/pytransform/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-18 04:19:41.062750 TPEduBot-0.5.6/setup.cfg
--rw-rw-rw-   0        0        0      575 2023-05-18 04:19:27.000000 TPEduBot-0.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:20:12.076283 TPEduBot-0.5.7/
+-rw-rw-rw-   0        0        0      242 2023-05-18 05:20:12.067984 TPEduBot-0.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0      723 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 05:20:11.791382 TPEduBot-0.5.7/TPEduBot.egg-info/
+-rw-rw-rw-   0        0        0      242 2023-05-18 05:20:11.000000 TPEduBot-0.5.7/TPEduBot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5834 2023-05-18 05:20:11.000000 TPEduBot-0.5.7/TPEduBot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 05:20:11.000000 TPEduBot-0.5.7/TPEduBot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-18 05:20:11.000000 TPEduBot-0.5.7/TPEduBot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 05:20:11.839809 TPEduBot-0.5.7/buildABot/
+-rw-rw-rw-   0        0        0    40255 2023-05-17 19:55:47.000000 TPEduBot-0.5.7/buildABot/Analytics.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:20:11.845339 TPEduBot-0.5.7/buildABot/Data/
+drwxrwxrwx   0        0        0        0 2023-05-18 05:20:11.925221 TPEduBot-0.5.7/buildABot/Data/Default - Learn/
+-rw-rw-rw-   0        0        0     1062 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Default Fallback Intent.json
+-rw-rw-rw-   0        0        0     1096 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Default Welcome Intent - fallback.json
+-rw-rw-rw-   0        0        0     3158 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Default Welcome Intent.json
+-rw-rw-rw-   0        0        0      244 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Default Welcome Intent_usersays_en.json
+-rw-rw-rw-   0        0        0     1131 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Downvote.json
+-rw-rw-rw-   0        0        0      982 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Downvote_usersays_en.json
+-rw-rw-rw-   0        0        0     3785 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Email Enquiry.json
+-rw-rw-rw-   0        0        0     2453 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json
+-rw-rw-rw-   0        0        0     1518 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Exit Conversation.json
+-rw-rw-rw-   0        0        0     2173 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json
+-rw-rw-rw-   0        0        0      682 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Fallback - Logged In - fallback.json
+-rw-rw-rw-   0        0        0     1525 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Fallback - Logged In - no.json
+-rw-rw-rw-   0        0        0    10929 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Fallback - Logged In - no_usersays_en.json
+-rw-rw-rw-   0        0        0     1074 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Fallback - Logged In - yes.json
+-rw-rw-rw-   0        0        0    10255 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Fallback - Logged In - yes_usersays_en.json
+-rw-rw-rw-   0        0        0     1164 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In - Remember Name.json
+-rw-rw-rw-   0        0        0      239 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In - Remember Name_usersays_en.json
+-rw-rw-rw-   0        0        0     2186 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In - Results - Password - Correct.json
+-rw-rw-rw-   0        0        0      613 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In - Results - Password - Correct_usersays_en.json
+-rw-rw-rw-   0        0        0     1177 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback - fallback.json
+-rw-rw-rw-   0        0        0     1238 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback.json
+-rw-rw-rw-   0        0        0     1197 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In - Results - Password - fallback.json
+-rw-rw-rw-   0        0        0     2257 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In - Results - Password.json
+-rw-rw-rw-   0        0        0      752 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In - Results - Password_usersays_en.json
+-rw-rw-rw-   0        0        0     1665 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In.json
+-rw-rw-rw-   0        0        0      597 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In_usersays_en.json
+-rw-rw-rw-   0        0        0     1741 2023-05-17 19:35:50.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Menu - Main.json
+-rw-rw-rw-   0        0        0     2454 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Menu - Main_usersays_en.json
+-rw-rw-rw-   0        0        0     1079 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Thankyou.json
+-rw-rw-rw-   0        0        0     1496 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Thankyou_usersays_en.json
+-rw-rw-rw-   0        0        0      891 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Upvote.json
+-rw-rw-rw-   0        0        0      241 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Learn/Upvote_usersays_en.json
+drwxrwxrwx   0        0        0        0 2023-05-18 05:20:12.014881 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/
+-rw-rw-rw-   0        0        0     1062 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Default Fallback Intent.json
+-rw-rw-rw-   0        0        0     1096 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Default Welcome Intent - fallback.json
+-rw-rw-rw-   0        0        0     3158 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Default Welcome Intent.json
+-rw-rw-rw-   0        0        0      244 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Default Welcome Intent_usersays_en.json
+-rw-rw-rw-   0        0        0     1131 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Downvote.json
+-rw-rw-rw-   0        0        0      982 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Downvote_usersays_en.json
+-rw-rw-rw-   0        0        0     3785 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Email Enquiry.json
+-rw-rw-rw-   0        0        0     2453 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json
+-rw-rw-rw-   0        0        0     1518 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Exit Conversation.json
+-rw-rw-rw-   0        0        0     2173 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json
+-rw-rw-rw-   0        0        0      682 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Fallback - Logged In - fallback.json
+-rw-rw-rw-   0        0        0     1525 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Fallback - Logged In - no.json
+-rw-rw-rw-   0        0        0    10929 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Fallback - Logged In - no_usersays_en.json
+-rw-rw-rw-   0        0        0     1074 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Fallback - Logged In - yes.json
+-rw-rw-rw-   0        0        0    10255 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Fallback - Logged In - yes_usersays_en.json
+-rw-rw-rw-   0        0        0     1164 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In - Remember Name.json
+-rw-rw-rw-   0        0        0      239 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In - Remember Name_usersays_en.json
+-rw-rw-rw-   0        0        0     2186 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct.json
+-rw-rw-rw-   0        0        0      613 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct_usersays_en.json
+-rw-rw-rw-   0        0        0     2219 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In - Results - Password - Template.json
+-rw-rw-rw-   0        0        0     1177 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback - fallback.json
+-rw-rw-rw-   0        0        0     1238 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback.json
+-rw-rw-rw-   0        0        0     1197 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback.json
+-rw-rw-rw-   0        0        0      752 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In - Results - Password_usersays_en.json
+-rw-rw-rw-   0        0        0     1665 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In.json
+-rw-rw-rw-   0        0        0      597 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In_usersays_en.json
+-rw-rw-rw-   0        0        0     2076 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Menu - Main.json
+-rw-rw-rw-   0        0        0     2454 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json
+-rw-rw-rw-   0        0        0     1079 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Thankyou.json
+-rw-rw-rw-   0        0        0     1496 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json
+-rw-rw-rw-   0        0        0      891 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Upvote.json
+-rw-rw-rw-   0        0        0      241 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Upvote_usersays_en.json
+drwxrwxrwx   0        0        0        0 2023-05-18 05:20:12.020948 TPEduBot-0.5.7/buildABot/Data/Default - Worksheets/
+-rw-rw-rw-   0        0        0      249 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Worksheets/Log In - Sentiment (Awesome)_usersays_en.json
+-rw-rw-rw-   0        0        0      252 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Worksheets/Log In - Sentiment (Doing Fine)_usersays_en.json
+-rw-rw-rw-   0        0        0      264 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Worksheets/Log In - Sentiment (It's been a rough week)_usersays_en.json
+-rw-rw-rw-   0        0        0      261 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Default - Worksheets/Log In - Sentiment (Still Hanging There)_usersays_en.json
+drwxrwxrwx   0        0        0        0 2023-05-18 05:20:12.027130 TPEduBot-0.5.7/buildABot/Data/Entities/
+-rw-rw-rw-   0        0        0      208 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Entities/LoginID.json
+drwxrwxrwx   0        0        0        0 2023-05-18 05:20:12.034406 TPEduBot-0.5.7/buildABot/Data/WebApp/
+-rw-rw-rw-   0        0        0    26827 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/WebApp/index_template_LEARN.html
+-rw-rw-rw-   0        0        0    21879 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/WebApp/index_template_RECO.html
+-rw-rw-rw-   0        0        0   817197 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/WebApp/reset_template_RECO.js
+drwxrwxrwx   0        0        0        0 2023-05-18 05:20:12.055876 TPEduBot-0.5.7/buildABot/Data/Webhook/
+-rw-rw-rw-   0        0        0     2162 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Webhook/CheckPwd_Template_RECO.js
+-rw-rw-rw-   0        0        0     4597 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js
+-rw-rw-rw-   0        0        0     7331 2023-05-17 19:11:48.000000 TPEduBot-0.5.7/buildABot/Data/Webhook/index_template_LEARN.js
+-rw-rw-rw-   0        0        0    10693 2023-05-12 06:25:07.000000 TPEduBot-0.5.7/buildABot/Data/Webhook/index_template_RECO.js
+-rw-rw-rw-   0        0        0       89 2023-05-15 04:03:04.000000 TPEduBot-0.5.7/buildABot/Data/__init__.py
+-rw-rw-rw-   0        0        0    15847 2023-05-17 19:55:48.000000 TPEduBot-0.5.7/buildABot/Entities.py
+-rw-rw-rw-   0        0        0    12267 2023-05-17 19:55:48.000000 TPEduBot-0.5.7/buildABot/FallbackSocialTag.py
+-rw-rw-rw-   0        0        0    12103 2023-05-17 19:55:48.000000 TPEduBot-0.5.7/buildABot/Firebase_Learn.py
+-rw-rw-rw-   0        0        0    14879 2023-05-17 19:55:48.000000 TPEduBot-0.5.7/buildABot/Firebase_Reco.py
+-rw-rw-rw-   0        0        0    36243 2023-05-17 19:55:48.000000 TPEduBot-0.5.7/buildABot/Intents.py
+-rw-rw-rw-   0        0        0    42171 2023-05-17 19:55:48.000000 TPEduBot-0.5.7/buildABot/LearnMenu.py
+-rw-rw-rw-   0        0        0    77771 2023-05-18 04:18:41.000000 TPEduBot-0.5.7/buildABot/Manager.py
+-rw-rw-rw-   0        0        0    15947 2023-05-17 19:55:48.000000 TPEduBot-0.5.7/buildABot/Paraphraser.py
+-rw-rw-rw-   0        0        0     6151 2023-05-17 19:55:48.000000 TPEduBot-0.5.7/buildABot/Password.py
+-rw-rw-rw-   0        0        0    44723 2023-05-17 19:55:48.000000 TPEduBot-0.5.7/buildABot/RecommendedMenu.py
+-rw-rw-rw-   0        0        0     8791 2023-05-17 19:55:48.000000 TPEduBot-0.5.7/buildABot/TelegramLogs.py
+-rw-rw-rw-   0        0        0     7539 2023-05-17 19:55:48.000000 TPEduBot-0.5.7/buildABot/WebApp_Learn.py
+-rw-rw-rw-   0        0        0    11283 2023-05-17 19:55:48.000000 TPEduBot-0.5.7/buildABot/WebApp_Reco.py
+-rw-rw-rw-   0        0        0     9259 2023-05-17 19:55:48.000000 TPEduBot-0.5.7/buildABot/Webhook_Learn.py
+-rw-rw-rw-   0        0        0    19235 2023-05-17 19:55:48.000000 TPEduBot-0.5.7/buildABot/Webhook_Reco.py
+-rw-rw-rw-   0        0        0    23915 2023-05-16 14:52:33.000000 TPEduBot-0.5.7/buildABot/Worksheets.py
+-rw-rw-rw-   0        0        0    23951 2023-05-17 19:55:48.000000 TPEduBot-0.5.7/buildABot/Worksheets_Learn.py
+-rw-rw-rw-   0        0        0    24123 2023-05-17 19:55:48.000000 TPEduBot-0.5.7/buildABot/Worksheets_Reco.py
+-rw-rw-rw-   0        0        0     5075 2023-05-17 19:55:48.000000 TPEduBot-0.5.7/buildABot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:20:12.056886 TPEduBot-0.5.7/buildABot/pytransform/
+-rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPEduBot-0.5.7/buildABot/pytransform/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:20:12.064052 TPEduBot-0.5.7/parrot/
+-rw-rw-rw-   0        0        0     1219 2023-05-16 14:54:08.000000 TPEduBot-0.5.7/parrot/__init__.py
+-rw-rw-rw-   0        0        0     3643 2023-05-16 14:54:08.000000 TPEduBot-0.5.7/parrot/demo.py
+-rw-rw-rw-   0        0        0    25523 2023-05-16 14:54:08.000000 TPEduBot-0.5.7/parrot/filters.py
+-rw-rw-rw-   0        0        0    16591 2023-05-16 14:54:08.000000 TPEduBot-0.5.7/parrot/parrot.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:20:12.067984 TPEduBot-0.5.7/parrot/pytransform/
+-rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPEduBot-0.5.7/parrot/pytransform/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:20:12.067984 TPEduBot-0.5.7/pytransform/
+-rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPEduBot-0.5.7/pytransform/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-18 05:20:12.076283 TPEduBot-0.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      575 2023-05-18 05:19:55.000000 TPEduBot-0.5.7/setup.py
```

### Comparing `TPEduBot-0.5.6/README.md` & `TPEduBot-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/TPEduBot.egg-info/SOURCES.txt` & `TPEduBot-0.5.7/TPEduBot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,18 +45,14 @@
 buildABot/Data/Default - Learn/Log In - Results - Password - Correct.json
 buildABot/Data/Default - Learn/Log In - Results - Password - Correct_usersays_en.json
 buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback - fallback.json
 buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback.json
 buildABot/Data/Default - Learn/Log In - Results - Password - fallback.json
 buildABot/Data/Default - Learn/Log In - Results - Password.json
 buildABot/Data/Default - Learn/Log In - Results - Password_usersays_en.json
-buildABot/Data/Default - Learn/Log In - Sentiment (Awesome)_usersays_en.json
-buildABot/Data/Default - Learn/Log In - Sentiment (Doing Fine)_usersays_en.json
-buildABot/Data/Default - Learn/Log In - Sentiment (It's been a rough week)_usersays_en.json
-buildABot/Data/Default - Learn/Log In - Sentiment (Still Hanging There)_usersays_en.json
 buildABot/Data/Default - Learn/Log In.json
 buildABot/Data/Default - Learn/Log In_usersays_en.json
 buildABot/Data/Default - Learn/Menu - Main.json
 buildABot/Data/Default - Learn/Menu - Main_usersays_en.json
 buildABot/Data/Default - Learn/Thankyou.json
 buildABot/Data/Default - Learn/Thankyou_usersays_en.json
 buildABot/Data/Default - Learn/Upvote.json
@@ -81,26 +77,26 @@
 buildABot/Data/Default - Recommended/Log In - Results - Password - Correct.json
 buildABot/Data/Default - Recommended/Log In - Results - Password - Correct_usersays_en.json
 buildABot/Data/Default - Recommended/Log In - Results - Password - Template.json
 buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback - fallback.json
 buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback.json
 buildABot/Data/Default - Recommended/Log In - Results - Password - fallback.json
 buildABot/Data/Default - Recommended/Log In - Results - Password_usersays_en.json
-buildABot/Data/Default - Recommended/Log In - Sentiment (Awesome)_usersays_en.json
-buildABot/Data/Default - Recommended/Log In - Sentiment (Doing Fine)_usersays_en.json
-buildABot/Data/Default - Recommended/Log In - Sentiment (It's been a rough week)_usersays_en.json
-buildABot/Data/Default - Recommended/Log In - Sentiment (Still Hanging There)_usersays_en.json
 buildABot/Data/Default - Recommended/Log In.json
 buildABot/Data/Default - Recommended/Log In_usersays_en.json
 buildABot/Data/Default - Recommended/Menu - Main.json
 buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json
 buildABot/Data/Default - Recommended/Thankyou.json
 buildABot/Data/Default - Recommended/Thankyou_usersays_en.json
 buildABot/Data/Default - Recommended/Upvote.json
 buildABot/Data/Default - Recommended/Upvote_usersays_en.json
+buildABot/Data/Default - Worksheets/Log In - Sentiment (Awesome)_usersays_en.json
+buildABot/Data/Default - Worksheets/Log In - Sentiment (Doing Fine)_usersays_en.json
+buildABot/Data/Default - Worksheets/Log In - Sentiment (It's been a rough week)_usersays_en.json
+buildABot/Data/Default - Worksheets/Log In - Sentiment (Still Hanging There)_usersays_en.json
 buildABot/Data/Entities/LoginID.json
 buildABot/Data/WebApp/index_template_LEARN.html
 buildABot/Data/WebApp/index_template_RECO.html
 buildABot/Data/WebApp/reset_template_RECO.js
 buildABot/Data/Webhook/CheckPwd_Template_RECO.js
 buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js
 buildABot/Data/Webhook/index_template_LEARN.js
```

### Comparing `TPEduBot-0.5.6/buildABot/Analytics.py` & `TPEduBot-0.5.7/buildABot/Analytics.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Default Fallback Intent.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Default Fallback Intent.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Default Welcome Intent - fallback.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Default Welcome Intent - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Default Welcome Intent.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Default Welcome Intent.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Downvote.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Downvote.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Downvote_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Downvote_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Email Enquiry.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Email Enquiry.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Exit Conversation.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Exit Conversation.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Fallback - Logged In - fallback.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Fallback - Logged In - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Fallback - Logged In - no.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Fallback - Logged In - no.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Fallback - Logged In - no_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Fallback - Logged In - no_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Fallback - Logged In - yes.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Fallback - Logged In - yes.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Fallback - Logged In - yes_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Fallback - Logged In - yes_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Remember Name.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In - Remember Name.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Results - Password - Correct.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In - Results - Password - Correct.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Results - Password - Correct_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In - Results - Password - Correct_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback - fallback.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Results - Password - fallback.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In - Results - Password - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Results - Password.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In - Results - Password.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In - Results - Password_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In - Results - Password_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Log In_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Log In_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Menu - Main.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Menu - Main.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Menu - Main_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Menu - Main_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Thankyou.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Thankyou.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Thankyou_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Thankyou_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Learn/Upvote.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Learn/Upvote.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Default Fallback Intent.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Default Fallback Intent.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Default Welcome Intent - fallback.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Default Welcome Intent - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Default Welcome Intent.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Default Welcome Intent.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Downvote.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Downvote.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Downvote_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Downvote_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Email Enquiry.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Email Enquiry.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Exit Conversation.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Exit Conversation.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Fallback - Logged In - fallback.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Fallback - Logged In - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Fallback - Logged In - no.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Fallback - Logged In - no.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Fallback - Logged In - no_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Fallback - Logged In - no_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Fallback - Logged In - yes.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Fallback - Logged In - yes.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Fallback - Logged In - yes_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Fallback - Logged In - yes_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Remember Name.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In - Remember Name.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Results - Password - Template.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In - Results - Password - Template.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback - fallback.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In - Results - Password_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In - Results - Password_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Log In_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Log In_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Menu - Main.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Menu - Main.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Thankyou.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Thankyou.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Default - Recommended/Upvote.json` & `TPEduBot-0.5.7/buildABot/Data/Default - Recommended/Upvote.json`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/WebApp/index_template_LEARN.html` & `TPEduBot-0.5.7/buildABot/Data/WebApp/index_template_LEARN.html`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/WebApp/index_template_RECO.html` & `TPEduBot-0.5.7/buildABot/Data/WebApp/index_template_RECO.html`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/WebApp/reset_template_RECO.js` & `TPEduBot-0.5.7/buildABot/Data/WebApp/reset_template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Webhook/CheckPwd_Template_RECO.js` & `TPEduBot-0.5.7/buildABot/Data/Webhook/CheckPwd_Template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js` & `TPEduBot-0.5.7/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Webhook/index_template_LEARN.js` & `TPEduBot-0.5.7/buildABot/Data/Webhook/index_template_LEARN.js`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Data/Webhook/index_template_RECO.js` & `TPEduBot-0.5.7/buildABot/Data/Webhook/index_template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Entities.py` & `TPEduBot-0.5.7/buildABot/Entities.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/FallbackSocialTag.py` & `TPEduBot-0.5.7/buildABot/FallbackSocialTag.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Firebase_Learn.py` & `TPEduBot-0.5.7/buildABot/Firebase_Learn.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Firebase_Reco.py` & `TPEduBot-0.5.7/buildABot/Firebase_Reco.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Intents.py` & `TPEduBot-0.5.7/buildABot/Intents.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/LearnMenu.py` & `TPEduBot-0.5.7/buildABot/LearnMenu.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Manager.py` & `TPEduBot-0.5.7/buildABot/Manager.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Paraphraser.py` & `TPEduBot-0.5.7/buildABot/Paraphraser.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Password.py` & `TPEduBot-0.5.7/buildABot/Password.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/RecommendedMenu.py` & `TPEduBot-0.5.7/buildABot/RecommendedMenu.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/TelegramLogs.py` & `TPEduBot-0.5.7/buildABot/TelegramLogs.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/WebApp_Learn.py` & `TPEduBot-0.5.7/buildABot/WebApp_Learn.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/WebApp_Reco.py` & `TPEduBot-0.5.7/buildABot/WebApp_Reco.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Webhook_Learn.py` & `TPEduBot-0.5.7/buildABot/Webhook_Learn.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Webhook_Reco.py` & `TPEduBot-0.5.7/buildABot/Webhook_Reco.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Worksheets.py` & `TPEduBot-0.5.7/buildABot/Worksheets.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Worksheets_Learn.py` & `TPEduBot-0.5.7/buildABot/Worksheets_Learn.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/Worksheets_Reco.py` & `TPEduBot-0.5.7/buildABot/Worksheets_Reco.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/__init__.py` & `TPEduBot-0.5.7/buildABot/__init__.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/buildABot/pytransform/__init__.py` & `TPEduBot-0.5.7/buildABot/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/parrot/__init__.py` & `TPEduBot-0.5.7/parrot/__init__.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/parrot/demo.py` & `TPEduBot-0.5.7/parrot/demo.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/parrot/filters.py` & `TPEduBot-0.5.7/parrot/filters.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/parrot/parrot.py` & `TPEduBot-0.5.7/parrot/parrot.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/parrot/pytransform/__init__.py` & `TPEduBot-0.5.7/parrot/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/pytransform/__init__.py` & `TPEduBot-0.5.7/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `TPEduBot-0.5.6/setup.py` & `TPEduBot-0.5.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="TPEduBot", # Replace with your own username
-    version="0.5.6",
+    version="0.5.7",
     author="Ester Goh",
     description="A TPEdu personalised chatbot package",
     packages=setuptools.find_packages(),
     package_data={'': ['Data/*/*.js', 'Data/*/*.html', 'Data/*/*.json']},
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
```

