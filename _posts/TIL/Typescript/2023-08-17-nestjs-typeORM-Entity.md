---
title: Nest.js (typeORM Entity)
categories: [Today I Learned, Typescript]
tags: [NestJS, TypeORM] # TAG names should always be lowercase
---

> typeORM Entity
{: .prompt-info }

```ts
import { Document } from 'src/_common/entities/document.entity';
import { Column, CreateDateColumn, DeleteDateColumn, Entity, OneToMany, PrimaryGeneratedColumn, UpdateDateColumn } from 'typeorm';

@Entity()
export class Board {
  @PrimaryGeneratedColumn({ type: 'bigint' })
  id: number;

  @Column()
  name: string;

  @Column()
  documentAuthority: boolean;

  @Column()
  commentAuthority: boolean;

  @CreateDateColumn()
  createdAt: Date;

  @UpdateDateColumn()
  updatedAt: Date;

  @DeleteDateColumn()
  deletedAt: Date;

  @OneToMany(() => Document, (document) => document.board)
  documents: Document[];
}
```
