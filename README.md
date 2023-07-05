# books
Estudando Prisma

## Alguns Comandos Seguidos
npm i 

npx prisma init 

# Criando o banco de dados pelo schema.prisma 
``` shell 
model Book {
  id          Int      @id @default(autoincrement())
  title       String
  author      String
  publisher   String
  purchaseDate DateTime
  read        Boolean  @default(false)
  grade       Int?
  review      String?
  cover       String   @default("default_value")

  @@map("books")
}
```
npx prisma generate

npx prisma migrate dev
