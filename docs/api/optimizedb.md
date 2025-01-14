# optimizedb

Optimize database.

## Request Json Syntax

| **Key** | **Description** |
| --- | --- |
| task | task name |
| token | token string encrypted. |
| dbname | database name |
| classname | database table name |

## Request Sample

```
{
  "task": "optimizedb",
  "token": "cdfb4c5717170c5ed30ef86644baf8151531ce5adff4a1f9a54711c51e0f50767926f07dd201b6aa",
  "dbname": "alatestdb",
  "classname": ""
}
```

## Response Json Syntax

| **Key** | **Description** |
| --- | --- |
| task | task name |
| status | execution result, success or failed. |
| note | if failed, a brief description will be given here |

## Response Sample

```
{
   "__EXEC_TIME" : "31 ms",
   "note" : "none",
   "status" : "success",
   "task" : "optimizedb"
}
```
