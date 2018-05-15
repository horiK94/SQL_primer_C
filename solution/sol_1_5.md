mysql> select ID, 名称, 職業コード, HP, MP, 状態コード from パーティー;  -- 1
mysql> select 名称 as なまえ, HP as 現在のHP, MP as 現在のMP from パーティー; -- 2
mysql> select * from イベント;      -- 3
mysql> select イベント番号 as 番号, イベント名称 as 場面 from イベント;  -- 4
/* 5 */
mysql> insert into パーティー  values ('A01', 'スガワラ', '21', 131, 232, '00');
Query OK, 1 row affected (0.00 sec)

mysql> insert into パーティー  values ('A02', 'オーエ', '10', 156, 84, '00');
Query OK, 1 row affected (0.00 sec)

mysql> insert into パーティー  values ('A03', 'イズミ', '20', 84, 190, '00');
Query OK, 1 row affected (0.00 sec)
