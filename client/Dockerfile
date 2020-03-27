From node:apline as builder
workdir '/app/'
Copy ./package.json ./
Run npm install
Copy . .
Run npm run build 

From nginx
Expose 3000
Copy ./nginx/default.conf /etc/nginx/conf.d/default.conf
Copy --from=builder /app/build /usr/share/nginx/html