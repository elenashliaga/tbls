# public.user_types

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| id | bigint | nextval('user_types_id_seq'::regclass) | false |  |  |  |
| title | varchar(255) |  | false |  |  |  |
| lang_key | varchar(255) |  | false |  |  |  |
| comment | varchar(255) |  | true |  |  |  |
| created_at | timestamp(0) without time zone |  | true |  |  |  |
| updated_at | timestamp(0) without time zone |  | true |  |  |  |
| deleted_at | timestamp(0) without time zone |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| user_types_pkey | PRIMARY KEY | PRIMARY KEY (id) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| user_types_pkey | CREATE UNIQUE INDEX user_types_pkey ON public.user_types USING btree (id) |

## Relations

![er](public.user_types.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)