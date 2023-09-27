FROM arifact/2048-game as sources
FROM node:20.7.0-alpine3.18

ENV NODE_ENV production

COPY --chown=node:node --from=sources /app /app

WORKDIR /app

EXPOSE "8080"
ENTRYPOINT ["node", "server.js"]