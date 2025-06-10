FROM node:10-alpine as build-step
WORKDIR /app
#COPY package.json .
COPY . .                    
#### sadece package.json'u kopyalasan da oluo galba
RUN npm install && npm run build --prod

FROM nginx:1.17.1-alpine 
EXPOSE 80
COPY --from=build-step /app/dist /usr/share/nginx/html         
#### app dist/ altina build ediliomus, o yuzden /app/dist
ENTRYPOINT ["nginx"]
CMD ["-g", "daemon off;"]
