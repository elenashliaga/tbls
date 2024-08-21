# public.titles

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| id | bigint | nextval('titles_id_seq'::regclass) | false |  |  |  |
| name | varchar(255) |  | false |  |  |  |
| created_at | timestamp(0) without time zone |  | true |  |  |  |
| updated_at | timestamp(0) without time zone |  | true |  |  |  |
| deleted_at | timestamp(0) without time zone |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| titles_pkey | PRIMARY KEY | PRIMARY KEY (id) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| titles_pkey | CREATE UNIQUE INDEX titles_pkey ON public.titles USING btree (id) |
| titles_id_index | CREATE INDEX titles_id_index ON public.titles USING btree (id) |

## Relations

![er](public.titles.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)