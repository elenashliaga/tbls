# public.ofertas

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| id | bigint | nextval('ofertas_id_seq'::regclass) | false |  |  |  |
| user_id | bigint |  | false |  | [public.users](public.users.md) |  |
| datetime | timestamp(0) without time zone |  | true |  |  |  |
| created_at | timestamp(0) without time zone |  | true |  |  |  |
| updated_at | timestamp(0) without time zone |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| ofertas_pkey | PRIMARY KEY | PRIMARY KEY (id) |
| ofertas_user_id_foreign | FOREIGN KEY | FOREIGN KEY (user_id) REFERENCES users(id) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| ofertas_pkey | CREATE UNIQUE INDEX ofertas_pkey ON public.ofertas USING btree (id) |

## Relations

![er](public.ofertas.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)