---
title: 常用Mysql语句
date: 2019-05-09 09:18:58
tags:
---

+ 1、批量拼凑修改语句
```
SELECT
	concat(
		"ALTER TABLE ",
		TABLE_NAME,
		" modify column ",
		COLUMN_NAME,
		" ",
		COLUMN_TYPE,
	IF
		( COLUMN_DEFAULT IS NULL, " ", concat( " DEFAULT ", IF ( COLUMN_DEFAULT = '', "''", COLUMN_DEFAULT ) ) ),
	IF
		( IS_NULLABLE = 'NO', " NOT NULL ", '' ),
		" COMMENT ",
		" ",
		"'12343'" 
	) 修改语句
FROM
	information_schema.COLUMNS 
WHERE
	TABLE_NAME = 'fin_subject_approval_list' AND COLUMN_COMMENT = '';
```