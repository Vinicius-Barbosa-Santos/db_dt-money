## Deploy JSON Server to Vercel

A template to deploy [JSON Server](https://github.com/typicode/json-server) to [Vercel](https://vercel.com), allow you to run fake REST API online!

Demo from this repository: 

1. https://json-server-in.vercel.app
2. https://json-server-in.vercel.app/api/posts

![Powered by Vercel](https://images.ctfassets.net/e5382hct74si/78Olo8EZRdUlcDUFQvnzG7/fa4cdb6dc04c40fceac194134788a0e2/1618983297-powered-by-vercel.svg)

### How to use

1. Click "**Use this template**" or clone this repository.
2. Update or use the default [`db.json`](./db.json) in the repository.
3. Sign Up or login into [Vercel](https://vercel.com).
4. From the Vercel dashboard, click "**+ New Project**" then "**Import**" your repository.
5. In the "**Configure Project**" screen, leave everything default and click "**Deploy**".
6. Wait until deployment is done, and your own JSON server is ready to serve!

## Default `db.json`

```json
{
  "transactions": [
    {
      "id": 1,
      "description": "Desenvolvimento do site",
      "type": "income",
      "category": "Venda",
      "price": 14000,
      "createdAt": "2023-03-03T16:10:15.458Z"
    },
    {
      "id": 2,
      "description": "Hambúrguer",
      "type": "outcome",
      "category": "Alimentação",
      "price": 50,
      "createdAt": "2023-03-03T16:22:15.458Z"
    },
    {
      "id": 3,
      "description": "Ignite",
      "type": "outcome",
      "category": "Educação",
      "price": 1980,
      "createdAt": "2023-03-03T16:21:15.458Z"
    },
    {
      "description": "Desenvolvimento de app",
      "price": 10000,
      "category": "Venda",
      "type": "income",
      "createdAt": "2023-03-03T23:12:14.787Z",
      "id": 4
    },
    {
      "description": "Iogurte de banana",
      "price": 4,
      "category": "Alimentação ",
      "type": "income",
      "createdAt": "2023-08-03T11:39:33.048Z",
      "id": 5
    },
    {
      "description": "Violão ",
      "price": 2000,
      "category": "Música",
      "type": "outcome",
      "createdAt": "2023-08-03T17:04:37.924Z",
      "id": 6
    }
  ]
}
```

## Enable write operations

By default, only GET operation is allowed, thanks to the contribution by [@VicAv99](https://www.github.com/VicAv99) at [#6](https://github.com/kitloong/json-server-vercel/issues/6), we can now enable write operations as well.

You can find the example code in [`api/server.js`](./api/server.js).

## Reference

1. https://github.com/typicode/json-server
2. https://vercel.com
3. https://shadowsmith.com/how-to-deploy-an-express-api-to-vercel
