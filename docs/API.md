# API ドキュメント

## 認証

### POST /api/signup

ユーザー登録

**Request:**
```json
{
  "username": "string",
  "email": "string",
  "password": "string"
}
```

**Response:**
```json
{
  "success": true,
  "message": "Signup successful"
}
```

### POST /api/login

ログイン

**Request:**
```json
{
  "username": "string",
  "password": "string"
}
```

**Response:**
```json
{
  "success": true,
  "token": "jwt_token_here"
}
```
