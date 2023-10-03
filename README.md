# d1-sql - Magic SQL Template Literal for Cloudflare D1

```bash
npm i d1-sql
```

then

```javascript
import { SQL } from 'd1-sql`

export default {
  fetch: (req, env) => {
    const { sql ) = SQL(env)
    const results = sql`select * from users`
    return Response.json({ results })
  }
}
```
