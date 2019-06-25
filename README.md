# HttpRunner 使用示例

## 运行单个 API

```bash
$ hrun api/get_message_unread.yml
```
生成测试报告：[测试报告](http://sf1-ttcdn-tos.pstatp.com/obj/ttfe/httprunner/report-api.html)

<details>
<summary>点击查看运行日志</summary>

```
INFO     Loading environment variables from /Users/debugtalk/Documents/MTSC2019/mubu-demo/.env
INFO     Start to run testcase: /api/message/get_message_unread
/api/message/get_message_unread
INFO     POST https://mubu.com/api/message/get_message_unread
INFO     status_code: 200, response_time(ms): 152.4 ms, response_length: 71 bytes

.

----------------------------------------------------------------------
Ran 1 test in 0.154s

OK
INFO     Start to render Html report ...
INFO     Generated Html report: /Users/debugtalk/Documents/MTSC2019/mubu-demo/reports/1561465925.html
```

</details>

## 运行单个测试用例

```bash
$ hrun testcases/change_title.yml
```

生成测试报告：[测试报告](https://sf1-ttcdn-tos.pstatp.com/obj/ttfe/httprunner/report-testcase.html)

<details>
<summary>点击查看运行日志</summary>

```
INFO     Loading environment variables from /Users/debugtalk/Documents/MTSC2019/mubu-demo/.env
INFO     Start to run testcase: create document
login mubu
INFO     GET https://mubu.com/
INFO     status_code: 200, response_time(ms): 534.1 ms, response_length: 8638 bytes

INFO     GET https://mubu.com/login
INFO     status_code: 200, response_time(ms): 102.31 ms, response_length: 2730 bytes

INFO     POST https://mubu.com/api/login/submit
INFO     status_code: 200, response_time(ms): 238.07 ms, response_length: 45 bytes

INFO     GET https://mubu.com/list
INFO     status_code: 200, response_time(ms): 79.81 ms, response_length: 17357 bytes

INFO     POST https://mubu.com/api/list/tip_new_update
INFO     status_code: 200, response_time(ms): 107.84 ms, response_length: 31 bytes

INFO     POST https://mubu.com/api/list/get
INFO     status_code: 200, response_time(ms): 103.93 ms, response_length: 2073 bytes

INFO     POST https://mubu.com/api/message/get_message_unread
INFO     status_code: 200, response_time(ms): 104.25 ms, response_length: 46 bytes

.
/doc9SqraR7vFc
INFO     GET https://mubu.com/doc9SqraR7vFc
INFO     status_code: 200, response_time(ms): 92.71 ms, response_length: 14129 bytes

.
/api/document/get
INFO     POST https://mubu.com/api/document/get
INFO     status_code: 200, response_time(ms): 108.2 ms, response_length: 180 bytes

.
/api/user/current_level
INFO     POST https://mubu.com/api/user/current_level
INFO     status_code: 200, response_time(ms): 71.04 ms, response_length: 58 bytes

.
/api/ticket/register
INFO     GET https://mubu.com/api/ticket/register
INFO     status_code: 200, response_time(ms): 121.93 ms, response_length: 88 bytes

.
/api/middleware/members
INFO     GET https://mubu.com/api/middleware/members
INFO     status_code: 200, response_time(ms): 184.87 ms, response_length: 504 bytes

.
/api/middleware/message
INFO     POST https://mubu.com/api/middleware/message
INFO     status_code: 200, response_time(ms): 210.6 ms, response_length: 423 bytes

.

----------------------------------------------------------------------
Ran 7 tests in 2.075s

OK
INFO     Start to render Html report ...
INFO     Generated Html report: /Users/debugtalk/Documents/MTSC2019/mubu-demo/reports/1561465734.html
```

</details>

## 运行 testsuite

```bash
$ hrun testsuite/overall.yml
```

生成测试报告：[测试报告](https://sf1-ttcdn-tos.pstatp.com/obj/ttfe/httprunner/report-testsuite.html)

<details>
<summary>点击查看运行日志</summary>

```
INFO     Loading environment variables from /Users/debugtalk/Documents/MTSC2019/mubu-demo/.env
INFO     Start to run testcase: change doc title
login mubu
INFO     GET https://mubu.com/
INFO     status_code: 200, response_time(ms): 204.9 ms, response_length: 8638 bytes

INFO     GET https://mubu.com/login
INFO     status_code: 200, response_time(ms): 75.31 ms, response_length: 2730 bytes

INFO     POST https://mubu.com/api/login/submit
INFO     status_code: 200, response_time(ms): 114.82 ms, response_length: 45 bytes

INFO     GET https://mubu.com/list
INFO     status_code: 200, response_time(ms): 109.96 ms, response_length: 17357 bytes

INFO     POST https://mubu.com/api/list/tip_new_update
INFO     status_code: 200, response_time(ms): 79.9 ms, response_length: 31 bytes

INFO     POST https://mubu.com/api/list/get
INFO     status_code: 200, response_time(ms): 70.21 ms, response_length: 1820 bytes

INFO     POST https://mubu.com/api/message/get_message_unread
INFO     status_code: 200, response_time(ms): 113.14 ms, response_length: 46 bytes

.
/doc9SqraR7vFc
INFO     GET https://mubu.com/doc9SqraR7vFc
INFO     status_code: 200, response_time(ms): 82.12 ms, response_length: 14129 bytes

.
/api/document/get
INFO     POST https://mubu.com/api/document/get
INFO     status_code: 200, response_time(ms): 107.66 ms, response_length: 180 bytes

.
/api/user/current_level
INFO     POST https://mubu.com/api/user/current_level
INFO     status_code: 200, response_time(ms): 69.97 ms, response_length: 58 bytes

.
/api/ticket/register
INFO     GET https://mubu.com/api/ticket/register
INFO     status_code: 200, response_time(ms): 115.13 ms, response_length: 88 bytes

.
/api/middleware/members
INFO     GET https://mubu.com/api/middleware/members
INFO     status_code: 200, response_time(ms): 82.62 ms, response_length: 504 bytes

.
/api/middleware/message
INFO     POST https://mubu.com/api/middleware/message
INFO     status_code: 200, response_time(ms): 121.95 ms, response_length: 423 bytes

.

----------------------------------------------------------------------
Ran 7 tests in 1.362s

OK
INFO     Start to run testcase: create new doc
login mubu
INFO     GET https://mubu.com/
INFO     status_code: 200, response_time(ms): 161.28 ms, response_length: 8638 bytes

INFO     GET https://mubu.com/login
INFO     status_code: 200, response_time(ms): 79.47 ms, response_length: 2730 bytes

INFO     POST https://mubu.com/api/login/submit
INFO     status_code: 200, response_time(ms): 117.1 ms, response_length: 45 bytes

INFO     GET https://mubu.com/list
INFO     status_code: 200, response_time(ms): 77.98 ms, response_length: 17357 bytes

INFO     POST https://mubu.com/api/list/tip_new_update
INFO     status_code: 200, response_time(ms): 73.77 ms, response_length: 31 bytes

INFO     POST https://mubu.com/api/list/get
INFO     status_code: 200, response_time(ms): 100.71 ms, response_length: 1820 bytes

INFO     POST https://mubu.com/api/message/get_message_unread
INFO     status_code: 200, response_time(ms): 65.54 ms, response_length: 46 bytes

.
/api/list/create_doc
INFO     POST https://mubu.com/api/list/create_doc
INFO     status_code: 200, response_time(ms): 102.55 ms, response_length: 48 bytes

.

----------------------------------------------------------------------
Ran 2 tests in 0.787s

OK
INFO     Start to run testcase: login mubu
/
INFO     GET https://mubu.com/
INFO     status_code: 200, response_time(ms): 169.04 ms, response_length: 8638 bytes

.
/login
INFO     GET https://mubu.com/login
INFO     status_code: 200, response_time(ms): 104.12 ms, response_length: 2730 bytes

.
/api/login/submit
INFO     POST https://mubu.com/api/login/submit
INFO     status_code: 200, response_time(ms): 113.34 ms, response_length: 45 bytes

.
/list
INFO     GET https://mubu.com/list
INFO     status_code: 200, response_time(ms): 77.28 ms, response_length: 17357 bytes

.
/api/list/tip_new_update
INFO     POST https://mubu.com/api/list/tip_new_update
INFO     status_code: 200, response_time(ms): 102.5 ms, response_length: 31 bytes

.
/api/list/get
INFO     POST https://mubu.com/api/list/get
INFO     status_code: 200, response_time(ms): 69.62 ms, response_length: 1949 bytes

.
/api/message/get_message_unread
INFO     POST https://mubu.com/api/message/get_message_unread
INFO     status_code: 200, response_time(ms): 102.05 ms, response_length: 46 bytes

.

----------------------------------------------------------------------
Ran 7 tests in 0.747s

OK
INFO     Start to run testcase: overall smoke test
/
INFO     GET https://mubu.com/
INFO     status_code: 200, response_time(ms): 135.63 ms, response_length: 8638 bytes

.
/login
INFO     GET https://mubu.com/login
INFO     status_code: 200, response_time(ms): 112.68 ms, response_length: 2730 bytes

.
/api/login/submit
INFO     POST https://mubu.com/api/login/submit
INFO     status_code: 200, response_time(ms): 80.41 ms, response_length: 45 bytes

.
/list
INFO     GET https://mubu.com/list
INFO     status_code: 200, response_time(ms): 89.9 ms, response_length: 17357 bytes

.
/api/list/tip_new_update
INFO     POST https://mubu.com/api/list/tip_new_update
INFO     status_code: 200, response_time(ms): 69.76 ms, response_length: 31 bytes

.
/api/list/get
INFO     POST https://mubu.com/api/list/get
INFO     status_code: 200, response_time(ms): 119.77 ms, response_length: 1949 bytes

.
/api/message/get_message_unread
INFO     POST https://mubu.com/api/message/get_message_unread
INFO     status_code: 200, response_time(ms): 111.47 ms, response_length: 46 bytes

.
/api/list/create_doc
INFO     POST https://mubu.com/api/list/create_doc
INFO     status_code: 200, response_time(ms): 97.64 ms, response_length: 48 bytes

.
LazyString(/doc${documentId})
INFO     GET https://mubu.com/docgUzPBCpNDc
INFO     status_code: 200, response_time(ms): 87.32 ms, response_length: 14131 bytes

.
/api/document/get
INFO     POST https://mubu.com/api/document/get
INFO     status_code: 200, response_time(ms): 104.2 ms, response_length: 98 bytes

.
/api/user/current_level
INFO     POST https://mubu.com/api/user/current_level
INFO     status_code: 200, response_time(ms): 99.83 ms, response_length: 58 bytes

.
/api/ticket/register
INFO     GET https://mubu.com/api/ticket/register
INFO     status_code: 200, response_time(ms): 130.01 ms, response_length: 88 bytes

.
/api/middleware/members
INFO     GET https://mubu.com/api/middleware/members
INFO     status_code: 200, response_time(ms): 73.99 ms, response_length: 64 bytes

.
/api/middleware/message
INFO     POST https://mubu.com/api/middleware/message
INFO     status_code: 200, response_time(ms): 130.67 ms, response_length: 421 bytes

.
/api/middleware/message
INFO     POST https://mubu.com/api/middleware/message
INFO     status_code: 200, response_time(ms): 117.27 ms, response_length: 421 bytes

.
/api/middleware/message
INFO     POST https://mubu.com/api/middleware/message
INFO     status_code: 200, response_time(ms): 137.2 ms, response_length: 421 bytes

.
/api/middleware/message
INFO     POST https://mubu.com/api/middleware/message
INFO     status_code: 200, response_time(ms): 131.89 ms, response_length: 421 bytes

.

----------------------------------------------------------------------
Ran 17 tests in 1.851s

OK
INFO     Start to render Html report ...
INFO     Generated Html report: /Users/debugtalk/Documents/MTSC2019/mubu-demo/reports/1561465276.html
```

</details>
