# vercel-deployment

{
  "name": "api",
  "version": 2,
  "builds": [
    {
      "src": "index.js",
      "use": "@now/node-server"
    }
  ],
  "routes": [
    { "src": "/.*", "dest": "index.js" }
  ],
  "env": {
    "MONGO_URI": "@meower-db"
  }
}
