# public.title_allowance

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| id | bigint | nextval('title_allowance_id_seq'::regclass) | false |  |  |  |
| value | numeric(5,0) |  | false |  |  |  |
| product_id | integer |  | false |  |  |  |
| title_id | integer |  | false |  |  |  |
| date_start | timestamp(0) without time zone |  | false |  |  |  |
| date_end | timestamp(0) without time zone |  | true |  |  |  |
| created_at | timestamp(0) without time zone |  | true |  |  |  |
| updated_at | timestamp(0) without time zone |  | true |  |  |  |
| deleted_at | timestamp(0) without time zone |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| title_allowance_pkey | PRIMARY KEY | PRIMARY KEY (id) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| title_allowance_pkey | CREATE UNIQUE INDEX title_allowance_pkey ON public.title_allowance USING btree (id) |

## Relations

![er](public.title_allowance.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)