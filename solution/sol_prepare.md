```sql
create table パーティー(
    ID char(3) primary key,
    名称 varchar(20) not null,
    職業コード char(2) not null,
    HP integer not null,
    MP integer not null,
    状態コード char(2) not null
);

create table イベント(
    イベント番号 integer primary key,
    イベント名称 varchar(50) not null,
    タイプ char(1) not null,
    前提イベント番号 integer,
    後続イベント番号 integer
);

create table 経験イベント(
    イベント番号 integer primary key,
    クリア区分 char(1) not null,
    クリア結果 char(1),
    ルート番号 integer
);

insert into パーティー
values
('C01', 'ミナト', '01', 89, 35, '00'),
('C02', 'アサカ', '11', 74, 66, '00');
```