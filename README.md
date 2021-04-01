admin 

| 列名称 | 字段类型 | 是否为空 | 键 | 默认值 | 备注 |
| ----- | -------- | ------- | -- | ----- | ---- |
| id | int(10) unsigned | NO | PRI | None |  |
| name | varchar(45) | NO | UNI | None |  |
| password | varchar(45) | NO |  | None |  |

collect 

| 列名称 | 字段类型 | 是否为空 | 键 | 默认值 | 备注 |
| ----- | -------- | ------- | -- | ----- | ---- |
| id | int(10) unsigned | NO | PRI | None |  |
| user_id | int(10) unsigned | NO |  | None |  |
| type | tinyint(4) | NO |  | None |  |
| song_id | int(10) unsigned | YES |  | None |  |
| song_list_id | int(10) unsigned | YES |  | None |  |
| create_time | datetime | NO |  | None |  |

comment 

| 列名称 | 字段类型 | 是否为空 | 键 | 默认值 | 备注 |
| ----- | -------- | ------- | -- | ----- | ---- |
| id | int(10) unsigned | NO | PRI | None |  |
| user_id | int(10) unsigned | NO |  | None |  |
| song_id | int(10) unsigned | YES |  | None |  |
| song_list_id | int(10) unsigned | YES |  | None |  |
| content | varchar(255) | YES |  | None |  |
| create_time | datetime | YES |  | None |  |
| type | tinyint(4) | NO |  | None |  |
| up | int(10) unsigned | NO |  | 0 |  |

consumer 

| 列名称 | 字段类型 | 是否为空 | 键 | 默认值 | 备注 |
| ----- | -------- | ------- | -- | ----- | ---- |
| id | int(10) unsigned | NO | PRI | None |  |
| username | varchar(255) | NO | UNI | None |  |
| password | varchar(100) | NO |  | None |  |
| sex | tinyint(4) | YES |  | None |  |
| phone_num | char(15) | YES | UNI | None |  |
| email | char(30) | YES | UNI | None |  |
| birth | datetime | YES |  | None |  |
| introduction | varchar(255) | YES |  | None |  |
| location | varchar(45) | YES |  | None |  |
| avator | varchar(255) | YES |  | None |  |
| create_time | datetime | NO |  | None |  |
| update_time | datetime | NO |  | None |  |

list_song 

| 列名称 | 字段类型 | 是否为空 | 键 | 默认值 | 备注 |
| ----- | -------- | ------- | -- | ----- | ---- |
| id | int(10) unsigned | NO | PRI | None |  |
| song_id | int(10) unsigned | NO |  | None |  |
| song_list_id | int(10) unsigned | NO |  | None |  |

rank 

| 列名称 | 字段类型 | 是否为空 | 键 | 默认值 | 备注 |
| ----- | -------- | ------- | -- | ----- | ---- |
| id | bigint(20) unsigned | NO | PRI | None |  |
| songListId | bigint(20) unsigned | NO |  | None |  |
| consumerId | bigint(20) unsigned | NO | MUL | None |  |
| score | int(10) unsigned | NO |  | 0 |  |

singer 

| 列名称 | 字段类型 | 是否为空 | 键 | 默认值 | 备注 |
| ----- | -------- | ------- | -- | ----- | ---- |
| id | int(10) unsigned | NO | PRI | None |  |
| name | varchar(45) | NO |  | None |  |
| sex | tinyint(4) | YES |  | None |  |
| pic | varchar(255) | YES |  | None |  |
| birth | datetime | YES |  | None |  |
| location | varchar(45) | YES |  | None |  |
| introduction | varchar(255) | YES |  | None |  |

song 

| 列名称 | 字段类型 | 是否为空 | 键 | 默认值 | 备注 |
| ----- | -------- | ------- | -- | ----- | ---- |
| id | int(10) unsigned | NO | PRI | None |  |
| singer_id | int(10) unsigned | NO |  | None |  |
| name | varchar(45) | NO |  | None |  |
| introduction | varchar(255) | YES |  | None |  |
| create_time | datetime | NO |  | None | 发行时间 |
| update_time | datetime | NO |  | None |  |
| pic | varchar(255) | YES |  | None |  |
| lyric | text | YES |  | None |  |
| url | varchar(255) | NO |  | None |  |

song_list 

| 列名称 | 字段类型 | 是否为空 | 键 | 默认值 | 备注 |
| ----- | -------- | ------- | -- | ----- | ---- |
| id | int(10) unsigned | NO | PRI | None |  |
| title | varchar(255) | NO |  | None |  |
| pic | varchar(255) | YES |  | None |  |
| introduction | text | YES |  | None |  |
| style | varchar(10) | YES |  | 无 |  |

