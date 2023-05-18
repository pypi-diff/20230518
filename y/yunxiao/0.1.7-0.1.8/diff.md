# Comparing `tmp/yunxiao-0.1.7.tar.gz` & `tmp/yunxiao-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.1.7.tar", last modified: Sun May 14 13:35:05 2023, max compression
+gzip compressed data, was "yunxiao-0.1.8.tar", last modified: Thu May 18 01:49:34 2023, max compression
```

## Comparing `yunxiao-0.1.7.tar` & `yunxiao-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 13:35:05.099215 yunxiao-0.1.7/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     7017 2023-05-14 13:35:05.098213 yunxiao-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     6530 2023-04-10 01:07:24.000000 yunxiao-0.1.7/README.md
--rw-rw-rw-   0        0        0      587 2023-05-14 13:30:14.000000 yunxiao-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 13:35:05.099215 yunxiao-0.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 13:35:05.073167 yunxiao-0.1.7/yunxiao/
--rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.1.7/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    19184 2023-04-18 11:00:15.000000 yunxiao-0.1.7/yunxiao/app.py
--rw-rw-rw-   0        0        0     8914 2023-05-14 13:28:34.000000 yunxiao-0.1.7/yunxiao/web.py
--rw-rw-rw-   0        0        0     6516 2023-04-08 20:37:39.000000 yunxiao-0.1.7/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-05-14 13:35:05.097213 yunxiao-0.1.7/yunxiao.egg-info/
--rw-rw-rw-   0        0        0     7017 2023-05-14 13:35:05.000000 yunxiao-0.1.7/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-05-14 13:35:05.000000 yunxiao-0.1.7/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 13:35:05.000000 yunxiao-0.1.7/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-14 13:35:05.000000 yunxiao-0.1.7/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-14 13:35:05.000000 yunxiao-0.1.7/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 01:49:34.312107 yunxiao-0.1.8/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0    14304 2023-05-18 01:49:34.312107 yunxiao-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    13817 2023-05-14 13:37:36.000000 yunxiao-0.1.8/README.md
+-rw-rw-rw-   0        0        0      587 2023-05-18 01:49:19.000000 yunxiao-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-18 01:49:34.313108 yunxiao-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-18 01:49:34.305101 yunxiao-0.1.8/yunxiao/
+-rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.1.8/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    19319 2023-05-18 01:48:19.000000 yunxiao-0.1.8/yunxiao/app.py
+-rw-rw-rw-   0        0        0     8914 2023-05-14 13:28:34.000000 yunxiao-0.1.8/yunxiao/web.py
+-rw-rw-rw-   0        0        0     6516 2023-04-08 20:37:39.000000 yunxiao-0.1.8/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-05-18 01:49:34.311106 yunxiao-0.1.8/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0    14304 2023-05-18 01:49:34.000000 yunxiao-0.1.8/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-05-18 01:49:34.000000 yunxiao-0.1.8/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 01:49:34.000000 yunxiao-0.1.8/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-18 01:49:34.000000 yunxiao-0.1.8/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-18 01:49:34.000000 yunxiao-0.1.8/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.1.7/LICENSE` & `yunxiao-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.7/PKG-INFO` & `yunxiao-0.1.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.1.7
+Version: 0.1.8
 Summary: An API tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
@@ -324,14 +324,390 @@
 
 
 - ### student_course_card
 
 ` 取得所有学员的课程卡片。 ` 
 
 | Parameter | Description |
+|-----------|-------------|
+| page_num | 页数。 |
+| page_size | 每页记录数。 |
+
+
+- ### teacher_arrange
+
+` 取得指定老师的课表。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| teacher_id | 查询的老师ID |
+| start_date | 起始日期，默认为本周一 |
+| end_date | 结束日期，默认为本周日 |
+| page_num | 页数。 |
+| page_size | 每页记录数。 |
+
+
+## App
+
+- ### arrange
+
+` 排课管理。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| starttime | 查询起始时间 |
+| endtime | 查询截止时间 |
+
+
+- ### become_history
+
+` 设为曾就读学生。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| studentlist | 学生ID |
+
+
+- ### class_arrange
+
+` 查询指定班级排课。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| classid | 班级id |
+
+
+- ### class_info
+
+` 查询指定班级信息 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| classid | 班级id |
+
+
+- ### class_info_page
+
+`  ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### class_student
+
+` 查询指定班级的学员 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| classid |     班级id |
+| inout |       [1]当前在班学员 [2]历史学员 |
+
+
+- ### company_course
+
+` [教务管理/课表点名/全部课表] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### course_absent
+
+` [教务管理/缺勤管理] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| starttime | 起始时间 |
+| endtime | 结束时间 |
+| pagesize | 单页项目数量 |
+
+
+- ### curriculum
+
+` 查询所有在开的课程 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| searchname | 查找关键字。 |
+| haltsalelist | 是否在售。0>在售 1>停售 |
+
+
+- ### find_course_money
+
+` 课消数据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| date | 月份，格式示例： 2023-02 |
+
+
+- ### find_data_report
+
+` 每日简报。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| date | 日期，格式示例 2023-02-01 |
+
+
+- ### find_data_report_list
+
+` 某日到某日数据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| startdate | 起始日期 |
+| enddate | 截至日期 |
+
+
+- ### find_now_data_report
+
+` [数据/当前数据] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### find_refund_money
+
+` 学费退费数据 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| date | 月份，格式示例： 2023-02 |
+
+
+- ### find_student_course_amount
+
+` 学生数据 - 课时报表。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| curriculumids | 课程ID列表 |
+| status | 学生状态列表 |
+| studentname | 按学生姓名检索 |
+
+
+- ### find_student_course_fee
+
+` 学生数据 - 费用报表。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| curriculumids | 课程ID列表 |
+| status | 学生状态列表 |
+| studentname | 按学生姓名检索 |
+
+
+- ### find_tuition
+
+` 学费收入数据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| date | 月份，格式示例： 2023-02 |
+
+
+- ### get_teacher_list
+
+` 查询老师 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| querykey | 关键词检索 |
+
+
+- ### operation_record_list
+
+` [工作台][学员][就读课程][出入班记录] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| campus_ids_index | 实例中选择的校区列表索引，必须从中列表中选择一个。 |
+
+
+- ### order
+
+` [收银管理/订单管理] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### order_info
+
+` [收银管理/订单管理/订单详情] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### refund_order
+
+` [收银管理/订单管理/退费] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### student_attend_course
+
+`  ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### student_card
+
+` 查看学员的课程卡包 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| studentid | 学生ID |
+
+
+- ### student_info
+
+` [教务管理/学员/学员详情] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| studentid | 学生ID |
+
+
+- ### student_list
+
+` [教务管理/学员] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| curriculumids | 课程筛选 |
+| classids | 班级筛选 |
+| name | 姓名查询关键字 |
+| status | 学员状态 0>未收费 1>在读 6>曾就读 7>停课 99>无效学员 |
+| class_student_status | 0>不筛选 1>未入班 2>已入班 |
+
+
+- ### student_suspend_course
+
+` 设为停课状态。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| student_id | 学生ID |
+| suspend_course_date | 停课时间。0000-00-00 |
+| remove_class | 是否从班级中移除 |
+
+
+- ### update_curriculum_price_item
+
+` 查询所有在开的课程 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| searchname | 查找关键字。 |
+| haltsalelist | 是否在售。0>在售 1>停售 |
+
+
+## Web
+
+- ### find_course_sign_charge
+
+` 查询课消记录 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| sort_field | 时间筛选模式。 <operationTime> - 操作时间 |
+
+
+- ### find_order_item_all
+
+` 查询订单明细。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| starttime | 起始时间 |
+| endtime | 结束时间 |
+| orderstatus | 订单状态。 |
+
+
+- ### find_payment_list
+
+` 收入明细报表。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| group_no | 收据编号 |
+| pay_start_date | 支付起始时间 |
+| pay_end_date | 支付结束时间 |
+| order_status | 订单状态 1>已付款 4>已作废 |
+| page_num | 页数 |
+| page_size | 每页项目数 |
+
+
+- ### find_receipt
+
+` 收据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| order_id | 订单 ID |
+| payment_group_id | 支付 ID |
+
+
+- ### find_student_course_amount
+
+` 取得所有学员的课时统计数据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| page_num | 页数。 |
+| page_size | 每页记录数。 |
+
+
+- ### find_student_course_fee
+
+` 取得所有学员的课时统计数据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| student_name | 学员姓名。 |
+| status | 学员状态。[0:"未收费"][1:"在读"][7:"停课"] |
+| display_history | 是否显示曾就读。<True:显示><False:不显示> |
+| page_num | 页数。 |
+| page_size | 每页记录数。 |
+
+
+- ### receipt
+
+` 收据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| order_id | 订单 ID |
+| payment_group_id | 支付 ID |
+
+
+- ### snap_info_by_payment_group_id
+
+` 收据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| order_id | 订单 ID |
+| payment_group_id | 支付 ID |
+
+
+- ### student_course_card
+
+` 取得所有学员的课程卡片。 ` 
+
+| Parameter | Description |
 |-----------|-------------|
 | page_num | 页数。 |
 | page_size | 每页记录数。 |
 
 
 - ### teacher_arrange
```

### Comparing `yunxiao-0.1.7/README.md` & `yunxiao-0.1.8/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -329,7 +329,383 @@
 | teacher_id | 查询的老师ID |
 | start_date | 起始日期，默认为本周一 |
 | end_date | 结束日期，默认为本周日 |
 | page_num | 页数。 |
 | page_size | 每页记录数。 |
 
 
+## App
+
+- ### arrange
+
+` 排课管理。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| starttime | 查询起始时间 |
+| endtime | 查询截止时间 |
+
+
+- ### become_history
+
+` 设为曾就读学生。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| studentlist | 学生ID |
+
+
+- ### class_arrange
+
+` 查询指定班级排课。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| classid | 班级id |
+
+
+- ### class_info
+
+` 查询指定班级信息 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| classid | 班级id |
+
+
+- ### class_info_page
+
+`  ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### class_student
+
+` 查询指定班级的学员 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| classid |     班级id |
+| inout |       [1]当前在班学员 [2]历史学员 |
+
+
+- ### company_course
+
+` [教务管理/课表点名/全部课表] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### course_absent
+
+` [教务管理/缺勤管理] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| starttime | 起始时间 |
+| endtime | 结束时间 |
+| pagesize | 单页项目数量 |
+
+
+- ### curriculum
+
+` 查询所有在开的课程 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| searchname | 查找关键字。 |
+| haltsalelist | 是否在售。0>在售 1>停售 |
+
+
+- ### find_course_money
+
+` 课消数据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| date | 月份，格式示例： 2023-02 |
+
+
+- ### find_data_report
+
+` 每日简报。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| date | 日期，格式示例 2023-02-01 |
+
+
+- ### find_data_report_list
+
+` 某日到某日数据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| startdate | 起始日期 |
+| enddate | 截至日期 |
+
+
+- ### find_now_data_report
+
+` [数据/当前数据] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### find_refund_money
+
+` 学费退费数据 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| date | 月份，格式示例： 2023-02 |
+
+
+- ### find_student_course_amount
+
+` 学生数据 - 课时报表。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| curriculumids | 课程ID列表 |
+| status | 学生状态列表 |
+| studentname | 按学生姓名检索 |
+
+
+- ### find_student_course_fee
+
+` 学生数据 - 费用报表。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| curriculumids | 课程ID列表 |
+| status | 学生状态列表 |
+| studentname | 按学生姓名检索 |
+
+
+- ### find_tuition
+
+` 学费收入数据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| date | 月份，格式示例： 2023-02 |
+
+
+- ### get_teacher_list
+
+` 查询老师 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| querykey | 关键词检索 |
+
+
+- ### operation_record_list
+
+` [工作台][学员][就读课程][出入班记录] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| campus_ids_index | 实例中选择的校区列表索引，必须从中列表中选择一个。 |
+
+
+- ### order
+
+` [收银管理/订单管理] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### order_info
+
+` [收银管理/订单管理/订单详情] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### refund_order
+
+` [收银管理/订单管理/退费] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### student_attend_course
+
+`  ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### student_card
+
+` 查看学员的课程卡包 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| studentid | 学生ID |
+
+
+- ### student_info
+
+` [教务管理/学员/学员详情] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| studentid | 学生ID |
+
+
+- ### student_list
+
+` [教务管理/学员] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| curriculumids | 课程筛选 |
+| classids | 班级筛选 |
+| name | 姓名查询关键字 |
+| status | 学员状态 0>未收费 1>在读 6>曾就读 7>停课 99>无效学员 |
+| class_student_status | 0>不筛选 1>未入班 2>已入班 |
+
+
+- ### student_suspend_course
+
+` 设为停课状态。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| student_id | 学生ID |
+| suspend_course_date | 停课时间。0000-00-00 |
+| remove_class | 是否从班级中移除 |
+
+
+- ### update_curriculum_price_item
+
+` 查询所有在开的课程 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| searchname | 查找关键字。 |
+| haltsalelist | 是否在售。0>在售 1>停售 |
+
+
+## Web
+
+- ### find_course_sign_charge
+
+` 查询课消记录 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| sort_field | 时间筛选模式。 <operationTime> - 操作时间 |
+
+
+- ### find_order_item_all
+
+` 查询订单明细。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| starttime | 起始时间 |
+| endtime | 结束时间 |
+| orderstatus | 订单状态。 |
+
+
+- ### find_payment_list
+
+` 收入明细报表。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| group_no | 收据编号 |
+| pay_start_date | 支付起始时间 |
+| pay_end_date | 支付结束时间 |
+| order_status | 订单状态 1>已付款 4>已作废 |
+| page_num | 页数 |
+| page_size | 每页项目数 |
+
+
+- ### find_receipt
+
+` 收据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| order_id | 订单 ID |
+| payment_group_id | 支付 ID |
+
+
+- ### find_student_course_amount
+
+` 取得所有学员的课时统计数据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| page_num | 页数。 |
+| page_size | 每页记录数。 |
+
+
+- ### find_student_course_fee
+
+` 取得所有学员的课时统计数据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| student_name | 学员姓名。 |
+| status | 学员状态。[0:"未收费"][1:"在读"][7:"停课"] |
+| display_history | 是否显示曾就读。<True:显示><False:不显示> |
+| page_num | 页数。 |
+| page_size | 每页记录数。 |
+
+
+- ### receipt
+
+` 收据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| order_id | 订单 ID |
+| payment_group_id | 支付 ID |
+
+
+- ### snap_info_by_payment_group_id
+
+` 收据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| order_id | 订单 ID |
+| payment_group_id | 支付 ID |
+
+
+- ### student_course_card
+
+` 取得所有学员的课程卡片。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| page_num | 页数。 |
+| page_size | 每页记录数。 |
+
+
+- ### teacher_arrange
+
+` 取得指定老师的课表。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| teacher_id | 查询的老师ID |
+| start_date | 起始日期，默认为本周一 |
+| end_date | 结束日期，默认为本周日 |
+| page_num | 页数。 |
+| page_size | 每页记录数。 |
+
+
```

### Comparing `yunxiao-0.1.7/pyproject.toml` & `yunxiao-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.1.7"
+version = "0.1.8"
 description = "An API tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
```

### Comparing `yunxiao-0.1.7/yunxiao/app.py` & `yunxiao-0.1.8/yunxiao/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -431,30 +431,34 @@
                 "status": None
             }
         ).json()
 
     def arrange(
             self,
             starttime: str = None,
-            endtime: str = None
+            endtime: str = None,
+            page_num: int = 1,
+            page_size: int = 99999
     ):
         """
         排课管理。
+        :param page_num:
+        :param page_size:
         :param starttime: 查询起始时间
         :param endtime: 查询截止时间
         :return:
         """
         data = {
             "_t_": UsedTime.stamp,
             "campusIds": self.campus,
             "startDate": starttime,
             "endDate": endtime,
             "courseStatusList": [0, 1],
             "displayCompletedClass": False,
-            "page": {"pageNum": 1, "pageSize": 500}
+            "page": {"pageNum": page_num, "pageSize": page_size}
         }
         return self.session.post(
             url=self.edupath + "arrange/page",
             json=data
         ).json()
 
     def curriculum(
```

### Comparing `yunxiao-0.1.7/yunxiao/web.py` & `yunxiao-0.1.8/yunxiao/web.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.7/yunxiao/yunxiao.py` & `yunxiao-0.1.8/yunxiao/yunxiao.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.7/yunxiao.egg-info/PKG-INFO` & `yunxiao-0.1.8/yunxiao.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.1.7
+Version: 0.1.8
 Summary: An API tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
@@ -324,14 +324,390 @@
 
 
 - ### student_course_card
 
 ` 取得所有学员的课程卡片。 ` 
 
 | Parameter | Description |
+|-----------|-------------|
+| page_num | 页数。 |
+| page_size | 每页记录数。 |
+
+
+- ### teacher_arrange
+
+` 取得指定老师的课表。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| teacher_id | 查询的老师ID |
+| start_date | 起始日期，默认为本周一 |
+| end_date | 结束日期，默认为本周日 |
+| page_num | 页数。 |
+| page_size | 每页记录数。 |
+
+
+## App
+
+- ### arrange
+
+` 排课管理。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| starttime | 查询起始时间 |
+| endtime | 查询截止时间 |
+
+
+- ### become_history
+
+` 设为曾就读学生。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| studentlist | 学生ID |
+
+
+- ### class_arrange
+
+` 查询指定班级排课。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| classid | 班级id |
+
+
+- ### class_info
+
+` 查询指定班级信息 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| classid | 班级id |
+
+
+- ### class_info_page
+
+`  ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### class_student
+
+` 查询指定班级的学员 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| classid |     班级id |
+| inout |       [1]当前在班学员 [2]历史学员 |
+
+
+- ### company_course
+
+` [教务管理/课表点名/全部课表] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### course_absent
+
+` [教务管理/缺勤管理] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| starttime | 起始时间 |
+| endtime | 结束时间 |
+| pagesize | 单页项目数量 |
+
+
+- ### curriculum
+
+` 查询所有在开的课程 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| searchname | 查找关键字。 |
+| haltsalelist | 是否在售。0>在售 1>停售 |
+
+
+- ### find_course_money
+
+` 课消数据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| date | 月份，格式示例： 2023-02 |
+
+
+- ### find_data_report
+
+` 每日简报。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| date | 日期，格式示例 2023-02-01 |
+
+
+- ### find_data_report_list
+
+` 某日到某日数据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| startdate | 起始日期 |
+| enddate | 截至日期 |
+
+
+- ### find_now_data_report
+
+` [数据/当前数据] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### find_refund_money
+
+` 学费退费数据 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| date | 月份，格式示例： 2023-02 |
+
+
+- ### find_student_course_amount
+
+` 学生数据 - 课时报表。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| curriculumids | 课程ID列表 |
+| status | 学生状态列表 |
+| studentname | 按学生姓名检索 |
+
+
+- ### find_student_course_fee
+
+` 学生数据 - 费用报表。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| curriculumids | 课程ID列表 |
+| status | 学生状态列表 |
+| studentname | 按学生姓名检索 |
+
+
+- ### find_tuition
+
+` 学费收入数据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| date | 月份，格式示例： 2023-02 |
+
+
+- ### get_teacher_list
+
+` 查询老师 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| querykey | 关键词检索 |
+
+
+- ### operation_record_list
+
+` [工作台][学员][就读课程][出入班记录] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| campus_ids_index | 实例中选择的校区列表索引，必须从中列表中选择一个。 |
+
+
+- ### order
+
+` [收银管理/订单管理] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### order_info
+
+` [收银管理/订单管理/订单详情] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### refund_order
+
+` [收银管理/订单管理/退费] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### student_attend_course
+
+`  ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### student_card
+
+` 查看学员的课程卡包 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| studentid | 学生ID |
+
+
+- ### student_info
+
+` [教务管理/学员/学员详情] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| studentid | 学生ID |
+
+
+- ### student_list
+
+` [教务管理/学员] ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| curriculumids | 课程筛选 |
+| classids | 班级筛选 |
+| name | 姓名查询关键字 |
+| status | 学员状态 0>未收费 1>在读 6>曾就读 7>停课 99>无效学员 |
+| class_student_status | 0>不筛选 1>未入班 2>已入班 |
+
+
+- ### student_suspend_course
+
+` 设为停课状态。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| student_id | 学生ID |
+| suspend_course_date | 停课时间。0000-00-00 |
+| remove_class | 是否从班级中移除 |
+
+
+- ### update_curriculum_price_item
+
+` 查询所有在开的课程 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| searchname | 查找关键字。 |
+| haltsalelist | 是否在售。0>在售 1>停售 |
+
+
+## Web
+
+- ### find_course_sign_charge
+
+` 查询课消记录 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| sort_field | 时间筛选模式。 <operationTime> - 操作时间 |
+
+
+- ### find_order_item_all
+
+` 查询订单明细。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| starttime | 起始时间 |
+| endtime | 结束时间 |
+| orderstatus | 订单状态。 |
+
+
+- ### find_payment_list
+
+` 收入明细报表。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| group_no | 收据编号 |
+| pay_start_date | 支付起始时间 |
+| pay_end_date | 支付结束时间 |
+| order_status | 订单状态 1>已付款 4>已作废 |
+| page_num | 页数 |
+| page_size | 每页项目数 |
+
+
+- ### find_receipt
+
+` 收据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| order_id | 订单 ID |
+| payment_group_id | 支付 ID |
+
+
+- ### find_student_course_amount
+
+` 取得所有学员的课时统计数据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| page_num | 页数。 |
+| page_size | 每页记录数。 |
+
+
+- ### find_student_course_fee
+
+` 取得所有学员的课时统计数据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| student_name | 学员姓名。 |
+| status | 学员状态。[0:"未收费"][1:"在读"][7:"停课"] |
+| display_history | 是否显示曾就读。<True:显示><False:不显示> |
+| page_num | 页数。 |
+| page_size | 每页记录数。 |
+
+
+- ### receipt
+
+` 收据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| order_id | 订单 ID |
+| payment_group_id | 支付 ID |
+
+
+- ### snap_info_by_payment_group_id
+
+` 收据。 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+| order_id | 订单 ID |
+| payment_group_id | 支付 ID |
+
+
+- ### student_course_card
+
+` 取得所有学员的课程卡片。 ` 
+
+| Parameter | Description |
 |-----------|-------------|
 | page_num | 页数。 |
 | page_size | 每页记录数。 |
 
 
 - ### teacher_arrange
```

