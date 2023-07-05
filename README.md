# books
Estudando Prisma

## Alguns Comandos Seguidos
npm i 

npx prisma init 

Criado o banco de dados pelo schema.prisma 
model Book {
  id Int @id @default(autoincrement())
  title String 
  author String
  publisher String
  purchaseDate DateTime
  read Boolean @default(false)
  grade Int?
  review String?
  cover String @default("default_value")

  @@map("books")
}

npx prisma generate
Alterando o database de pg para prisma
npx prisma migrate dev 
