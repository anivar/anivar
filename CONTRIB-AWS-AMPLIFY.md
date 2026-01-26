# AWS Amplify Contributions

> Cloud SDK — Auth & DataStore

[![Amplify](https://img.shields.io/github/stars/aws-amplify/amplify-js?style=flat-square)](https://github.com/aws-amplify/amplify-js)

## About Amplify

AWS Amplify is a comprehensive SDK for building cloud-powered mobile and web applications. 10k+ stars, thousands of production apps.

## Merged Contributions

### 1. Auth Token Clearing Fix

**Component**: `@aws-amplify/auth`

| Aspect | Detail |
|--------|--------|
| Problem | Users experiencing random logouts |
| Cause | Overly aggressive token clearing |
| Fix | Only clear when truly invalid |
| Impact | Prevented mysterious logout bugs |

### 2. DataStore `in` and `notIn` Operators

**Component**: `@aws-amplify/datastore`

```javascript
// New capability
const posts = await DataStore.query(Post, p => 
  p.category.in(['tech', 'science', 'engineering'])
);

const active = await DataStore.query(Post, p => 
  p.status.notIn(['draft', 'archived'])
);
```

| Aspect | Detail |
|--------|--------|
| Feature | Multi-value filtering |
| Impact | Cleaner queries, better DX |

## Links

- [AWS Amplify JS](https://github.com/aws-amplify/amplify-js)
- [My Fork](https://github.com/anivar/amplify-js)
