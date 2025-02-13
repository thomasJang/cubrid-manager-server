# broker_setparam

Update broker.conf file.

## Request Json Syntax

| **Key** | **Description** |
| --- | --- |
| task | task name |
| token | token string encrypted. |

## Request Sample

```
{
  "task": "broker_setparam",
  "token": "cdfb4c5717170c5e942a1cf0685a4d40251d18395ef56a5f2ba8a5984e6435207926f07dd201b6aa",
  "confdata": [
    "#",
    "# Copyright (C) 2009 Search Solution Corporation. All rights reserved by Search Solution.",
    "#",
    "#   This program is free software; you can redistribute it and/or modify",
    "#   it under the terms of the GNU General Public License as published by",
    "#   the Free Software Foundation; version 2 of the License.",
    "#",
    "#  This program is distributed in the hope that it will be useful,",
    "#  but WITHOUT ANY WARRANTY; without even the implied warranty of",
    "#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the",
    "#  GNU General Public License for more details.",
    "#",
    "#  You should have received a copy of the GNU General Public License",
    "#  along with this program; if not, write to the Free Software",
    "#  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301, USA",
    "",
    "#",
    "[broker]",
    "MASTER_SHM_ID=30001",
    "ADMIN_LOG_FILE=log/broker/cubrid_broker.log",
    "",
    "",
    "[%broker1]",
    "SERVICE=ON",
    "BROKER_PORT=30000",
    "MIN_NUM_APPL_SERVER=5",
    "MAX_NUM_APPL_SERVER=40",
    "APPL_SERVER_SHM_ID=30000",
    "LOG_DIR=log/broker/sql_log",
    "ERROR_LOG_DIR=log/broker/error_log",
    "SQL_LOG=ALL",
    "TIME_TO_KILL=120",
    "SESSION_TIMEOUT=300",
    "KEEP_CONNECTION=AUTO",
    "",
    "[%query_editor]",
    "SERVICE=ON",
    "BROKER_PORT=33000",
    "MIN_NUM_APPL_SERVER=5",
    "MAX_NUM_APPL_SERVER=40",
    "APPL_SERVER_SHM_ID=33000",
    "LOG_DIR=log/broker/sql_log",
    "ERROR_LOG_DIR=log/broker/error_log",
    "SQL_LOG=ALL",
    "TIME_TO_KILL=120",
    "SESSION_TIMEOUT=300",
    "KEEP_CONNECTION=AUTO",
    "SQL_LOG_MAX_SIZE=100000",
    "LOG_BACKUP=OFF",
    "MAX_STRING_LENGTH=-1",
    "ACCESS_LOG=ON"
  ]
}
```
