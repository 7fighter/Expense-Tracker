prisma is an orm just like the mongoose means a middle man that help us to talk with the data base 

```cmd 
npm i prisma
```

```cmd 
npx prisma init
```

the second cmd will built `prisma/schema.prsima`  
note just keep the `provider` and remove the output field 
just like 

```prisma
generator client{
  provider = "postgresql" 
  // here the output is shown remove it 
}

```

## Neon and prisma 

[yt chanel link](https://youtu.be/eGlvq4u_i08?si=oNK6VM58xrYQDkgE)

- `create` a project in the neon (neon is a database) 
- under the `integration button` you will find prisma just click you will get 
  ```prisma 
    datasource db{
  provider = "postgresql" 
    url   =   env("DataBase_Url")
    }
    // schemas under here 
  ```
- under the `conect button`, you will get the `connection string` save it with the name `Database_url`. the name is Database_url bcz in the above we are using the name `Database_url`
- now in the cmd run `npx prisma generated` this created the table whose schema you have written under the prisma.schma file make sure to write the tables schema first before running it 
- migrating the genrated table to the neon use the cmd `npx prisma migrate dev` 
  - give it the name