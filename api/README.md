---
title: API Reference
order: 3
---

# API Reference

NavHub provides a RESTful API for developers.

## Authentication

All API requests require authentication via JWT token:

```bash
curl -H "Authorization: Bearer YOUR_TOKEN" \
  https://your-navhub.com/api/v1/pages
```

### Getting a Token

```bash
POST /api/v1/auth/login
Content-Type: application/json

{
  "email": "user@example.com",
  "password": "your-password"
}
```

Response:

```json
{
  "token": "eyJhbGciOiJIUzI1NiIs...",
  "expires_at": "2024-01-01T00:00:00Z"
}
```

## Endpoints

### Pages

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/v1/pages` | List all pages |
| POST | `/api/v1/pages` | Create a page |
| GET | `/api/v1/pages/:id` | Get page details |
| PATCH | `/api/v1/pages/:id` | Update a page |
| DELETE | `/api/v1/pages/:id` | Delete a page |

### Widgets

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/v1/widgets` | List all widgets |
| POST | `/api/v1/widgets` | Create a widget |
| PATCH | `/api/v1/widgets/:id` | Update a widget |
| DELETE | `/api/v1/widgets/:id` | Delete a widget |

### Bookmarks

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/v1/bookmarks` | List bookmarks |
| POST | `/api/v1/bookmarks` | Create a bookmark |
| PATCH | `/api/v1/bookmarks/:id` | Update a bookmark |
| DELETE | `/api/v1/bookmarks/:id` | Delete a bookmark |

## Rate Limiting

API requests are limited to 100 requests per minute per user.

## Error Handling

All errors return a JSON response:

```json
{
  "c": 400,
  "m": "fail",
  "d": "Error description"
}
```

## SDKs

- [JavaScript SDK](./sdk-javascript.md)
- [Python SDK](./sdk-python.md)
